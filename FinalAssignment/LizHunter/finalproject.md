# **Trimming, Assembly, Sorting** #

## FastQC Quality Check ##

``` #!/bin/bash
#SBATCH -J Neph
#SBATCH -t 4-00:00:00
#SBATCH -N 1
#SBATCH -n 16

module load FastQC/0.11.5-Java-1.8.0_92

fastqc *.gz
```

## Trimmomatic ##
```
#!/bin/bash
#SBATCH -J Nephtrim
#SBATCH -t 4-00:00:00
#SBATCH -N 1
#SBATCH -n 16

module load Trimmomatic/0.36-Java-1.8.0_92

java -jar $EBROOTTRIMMOMATIC/trimmomatic-0.36.jar PE -threads 8 -phred33 XRICL_20160311_K00134_IL100067075_S24_L005_R1.fastq.gz XRICL_20160311_K00134_IL100067075_S24_L005_R2.fastq.gz nephPR1.fq.gz nephUPR1.fq.gz nephPR2.fq.gz nephUPR2.fq.gz ILLUMINACLIP:TruSeq3-PE.fa:2:30:10 HEADCROP: 13 LEADING:4 TRAILING:4 SLIDINGWINDOW:4:20 MINLEN:25
```
```
TrimmomaticPE: Started with arguments:
  -threads 8 -phred33 XRICL_20160311_K00134_IL100067075_S24_L005_R1.fastq.gz XRICL_20160311_K00134_IL100067075_S24_L005_R2.fastq.gz nephPR1.fq.gz nephUPR1.fq.gz nephPR2.fq.gz nephUPR2.fq.gz ILLUMINACLIP:TruSeq3-PE.fa:2:30:10 HEADCROP:13 LEADING:4 TRAILING:4 SLIDINGWINDOW:4:20 MINLEN:25
 Using PrefixPair: 'TACACTCTTTCCCTACACGACGCTCTTCCGATCT' and 'GTGACTGGAGTTCAGACGTGTGCTCTTCCGATCT'
 ILLUMINACLIP: Using 1 prefix pairs, 0 forward/reverse sequences, 0 forward only sequences, 0 reverse only sequences
 Input Read Pairs: 55316212 Both Surviving: 39916756 (72.16%) Forward Only Surviving: 14602794 (26.40%) Reverse Only Surviving: 333261 (0.60%) Dropped: 463401 (0.84%)
 TrimmomaticPE: Completed successfully

```
*rechecked quality with FastQC

## Trinity Assembly ##
```
#!/bin/bash
#SBATCH -J CardioTrinity
#SBATCH -t 5-00:00:00
#SBATCH --mem=250G
#SBATCH -N 1
#SBATCH --exclusive
#SBATCH --mail-type=END
#SBATCH --mail-user=lizhunter@my.uri.edu

module load Trinity/2.4.0-foss-2016b
Bowtie2/2.2.9-foss-2016b
SAMtools/1.5-foss-2017a

Trinity \
--seqType fq \
--left cardioPR1.fq.gz \
--right cardioPR2.fq.gz \
--SS_lib_type FR \
--max_memory 250G \
--CPU 20 \
--output ~/data3/lanelab/liz/BIO594/Cardio/Trinity

```
## Binning ##
### Prokaryotes/Eukaryotes###
```
#count sequences
grep ">" $1 | wc -l trinity.fasta

#split into batches
awk 'BEGIN {n_seq=0;} /^>/ {if(n_seq%100==0){file=sprintf("%d.fa",n_seq);} print >> file; n_seq++; next;} { print >> file; close(file)}' < trinity.fasta

#rename sequentially
n=1; for x in *.fa; do mv $x  $n.fa; n=$(($n+1)); done

#run a blast array
blastx -query "SLURM_ARRAY_TASK_ID".fa -db refseq_protein -outfmt 6 -max_target_seqs 1 -max_hsps 1 -taxid -out "SLURM_ARRAY_TASK_ID".out
cat *.out nephall.txt

#sort blast results by kingdom with regular expressions in text wrangler
grep "Prokaryotes" nephall.txt > prokaryotes.txt
grep "Eukaryotes" nephall.txt > eukaryotes.txt

#Pull sequence IDs
(T.+\|m\.\d+)\t.+\n
Replace: \1\n

#Pull Sequences Using Header File
grep -A1 -w -f headers.txt trinity.fasta

#generated a database of ascidians and apicomplexan transcriptomes
cat *.txt asciapi.fasta
makeblastdb -in asciapi.fasta -parse_seqids -dbtype nucl -taxid
blastx -query "SLURM_ARRAY_TASK_ID".fa -db asciapi.fasta -outfmt 6 -max_target_seqs 1 -max_hsps 1 -taxid -out "SLURM_ARRAY_TASK_ID".out
cat *.out > asciapiblast.fasta

#blast results sorted with regular expressions, sequence IDs sorted out, and the actually sequences pulled as above

```
(in an ideal world with more time, would have remapped all raw reads to these bins with Bowtie then reassembled with trinity)

## Translate with Transdecoder##
```
TransDecoder.LongOrfs -t nephtrinity.fasta
TransDecoder.Predict -t longest_orfs.cds
```

## Final Read Counts ##
- Nephromyces 60,223
- Cardiosporidium 15,541

# **Analysis** #

## BUSCO Transcriptome Analysis ##
#### Running BUSCO ####

```
#!/bin/bash
#SBATCH -J busco
#SBATCH -t 01:00:00
#SBATCH -N 1
#SBATCH -n 16

module load busco/2.0
module load blast
module load HMMER/3.1b2-foss-2016b
python ../run_BUSCO.py -i /data3/lanelab/liz/BIO594/Cardio/Trinity/cardiotrinity.fasta -o cardiobusco -l /data3/lanelab/liz/BIO594/alveolata_stramenophiles_ensembl -m tran
```

#### Generation of R code  ####
```
conda create -n python36 python=3.6 anaconda

python BUSCO_plot.py -wd /Users/AlgaeLab/Desktop/LIZ/BUSCO/plot_data
```

#### Busco Transcriptome Graphing (R) ####

```
# BUSCO summary figure
# @author Mathieu Seppey <mathieu.seppey@unige.ch>
# @version 2.0
# @since BUSCO 2.0
#
# Copyright (C) 2016 E. Zdobnov lab
#
# BUSCO is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version. See <http://www.gnu.org/licenses/>
#
# BUSCO is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.

# Load the required libraries
library(ggplot2)
library("grid")

# !!! CONFIGURE YOUR PLOT HERE !!!
# Output
my_output <- paste("/Users/AlgaeLab/Desktop/LIZ/BUSCO/plot_data/","busco_figure.png",sep="/")
my_width <- 20
my_height <- 15
my_unit <- "cm"

# Colors
my_colors <- c("#56B4E9", "#3492C7", "#F0E442", "#F04442")
# Bar height ratio
my_bar_height <- 0.75

# Legend
my_title <- "BUSCO Assessment Results"

# Font
my_family <- "sans"
my_size_ratio <- 1

# !!! SEE YOUR DATA HERE !!!
# Your data as generated by python, remove or add more
my_species <- c('cardio', 'cardio', 'cardio', 'cardio', 'neph', 'neph', 'neph', 'neph')
my_species <- factor(my_species)
my_species <- factor(my_species,levels(my_species)[c(length(levels(my_species)):1)]) # reorder your species here just by changing the values in the vector :
my_percentage <- c(15.8, 33.3, 0.0, 50.9, 6.4, 39.3, 1.3, 53.0)
my_values <- c(37, 78, 0, 119, 15, 92, 3, 124)

######################################
######################################
######################################
# Code to produce the graph
labsize = 1
if (length(levels(my_species)) > 10){
 labsize = 0.66
}
print("Plotting the figure ...")
category <- c(rep(c("S","D","F","M"),c(1)))
category <-factor(category)
category = factor(category,levels(category)[c(4,1,2,3)])
df = data.frame(my_species,my_percentage,my_values,category)

figure <- ggplot() +

  geom_bar(aes(y = my_percentage, x = my_species, fill = category), data = df, stat="identity", width=my_bar_height) +
  coord_flip() +
  theme_gray(base_size = 8) +
  scale_y_continuous(labels = c("0","20","40","60","80","100"), breaks = c(0,20,40,60,80,100)) +
  scale_fill_manual(values = my_colors,labels =c(" Complete (C) and single-copy (S)  ",
                                                 " Complete (C) and duplicated (D)",
                                                 " Fragmented (F)  ",
                                                 " Missing (M)")) +
  ggtitle(my_title) +
  xlab("") +
  ylab("\n%BUSCOs") +

  theme(plot.title = element_text(family=my_family, colour = "black", size = rel(2.2)*my_size_ratio, face = "bold")) +
  theme(legend.position="top",legend.title = element_blank()) +
  theme(legend.text = element_text(family=my_family, size = rel(1.2)*my_size_ratio)) +
  theme(panel.background = element_rect(color="#FFFFFF", fill="white")) +
  theme(panel.grid.minor = element_blank()) +
  theme(panel.grid.major = element_blank()) +
  theme(axis.text.y = element_text(family=my_family, colour = "black", size = rel(1.66)*my_size_ratio)) +
  theme(axis.text.x = element_text(family=my_family, colour = "black", size = rel(1.66)*my_size_ratio)) +
  theme(axis.line = element_line(size=1*my_size_ratio, colour = "black")) +
  theme(axis.ticks.length = unit(.85, "cm")) +
  theme(axis.ticks.y = element_line(colour="white", size = 0)) +
  theme(axis.ticks.x = element_line(colour="#222222")) +
  theme(axis.ticks.length = unit(0.4, "cm")) +
  theme(axis.title.x = element_text(family=my_family, size=rel(1.2)*my_size_ratio)) +

  guides(fill = guide_legend(override.aes = list(colour = NULL))) +
  guides(fill=guide_legend(nrow=2,byrow=TRUE))

  for(i in rev(c(1:length(levels(my_species))))){
    detailed_values <- my_values[my_species==my_species[my_species==levels(my_species)[i]]]
    total_buscos <- sum(detailed_values)
    figure <- figure +
    annotate("text", label=paste("C:", detailed_values[1] + detailed_values[2], " [S:", detailed_values[1], ", D:", detailed_values[2], "], F:", detailed_values[3], ", M:", detailed_values[4], ", n:", total_buscos, sep=""),
             y=3, x = i, size = labsize*4*my_size_ratio, colour = "black", hjust=0, family=my_family)
  }

ggsave(figure, file=my_output, width = my_width, height = my_height, unit = my_unit)
print("Done")

```

![](https://i.imgur.com/bWLkupJ.png)

## Orthofinder ##

Pull transcriptomes from eupath.db
- Toxoplasma gondii M64
- Plasmodium falciparum 3D7
- Cryptopsporidium parvum
- Chromera velia

Combined with assembled transcriptomes
- Nephromyces isolate
- Cardiosporidium cionae

```
conda install -c bioconda orthofinder

mkdir Orthofinder
mv *.fasta /Orthofinder

orthofinder -f orthofinder/ -t 5

```
OrthoFinder assigned 70927 genes (64.8% of total) to 6422 orthogroups. Fifty percent of all genes were in orthogroups with 9 or more genes (G50 was 9) and were contained in the largest 2742 orthogroups (O50 was 2742). There were 1341 orthogroups with all species present and 4 of these consisted entirely of single-copy genes.
#### Tree generated by OrthoFinder ####

![](https://i.imgur.com/AbdSZWH.png)

## GOSlim Analysis ##

#sort Orthogroups.GeneCount.csv for orthologs contained in all groups (not just single copy)

```
#Remove rows when there is a 0 in any column
Find and replace with nothing: ^OG(.+)\t0t(.+)

#Remove blank lines
grep '[^[:blank:]]' < orthos.fasta > orthos2.fasta

#Pull headers only
Find: ^OG(\d+)\t(.+)
Replace: OG\1

#Pull sequences IDs from main ortho file
grep -F -w -f orthos3.tsv Orthogroups.tsv > sharedseq.tsv

#Sort for single (model) organism - used Toxoplasma
grep "Toxo" sharedseq.tsv > toxoorthogroups.txt
```

#Search genes on eupath.db and download GOterms
#Agbase to convert from GOterms to GOslim

![](https://i.imgur.com/Is9Tbd0.png)

## Virulence Factor Database ##
1. List of virulence factors from Kegg infectious disease pathway modules
2. Sequences for virulence factors found & downloaded from eupath.db
3. List of all common virulence factors used as a blast database for the two assembled transcriptomes

```
#make database
makeblastdb -in virulencefactors.txt -parse_seqids -dbtype prot

#run local blast
blastp -query trinity.fasta -db virulencefactors.fasta -outfmt 6 -max_target_seqs 3 > nephvirulence.fasta

#delete to header
Find: (T.+\|m\.\d+)\t.+\n
Replace: \1\n

#pull sequences from translated protein file
grep -A1 -w -f nephvirulence2.fasta nephvirulenceseq.fasta

#delete duplicates
mothur uniq_seq

#split into batches of 100 sequences
mkdir nephvirulence
awk 'BEGIN {n_seq=0;} /^>/ {if(n_seq%100==0){file=sprintf("%d.fa",n_seq);} print >> file; n_seq++; next;} { print >> file; close(file)}' < ../nephvirulenceseq.fasta

#rename sequentially (1-296)
n=1; for x in *.fa; do mv $x  $n.fa; n=$(($n+1)); done

#array blast on bluewaves
#!/bin/bash
#SBATCH -J blast
#SBATCH -t 10:00:00
#SBATCH -N 1
#SBATCH -n 16
#SBATCH --array=1-296

module load blast

blastp -db /data3/shared/ncbi-refseq_protein/refseq_protein.36 \
-query "$SLURM_ARRAY_TASK_ID".fa \
-out "$SLURM_ARRAY_TASK_ID".out \
-outfmt '6 qseqid sseqid' \
-max_target_seqs 1 \
-num_threads 16

#pull GI numbers
Find: .+gi\|(\d+)\|.+\n
Replace: \1\n

#split into smaller files
split -l 2500 nephblast.txt

#run on NCBI batch entrez
```
(this last piece ended up giving a ton of noise and not anything worth using, need to find a better way to filter these results, perhaps a smaller more specific blast database)
