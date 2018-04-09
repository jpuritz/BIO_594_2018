# Name :Evelyn Takyi

## Date: 04/08/2018
### Week8

[etakyi@KITT Week8]$ cd Evelyn/
[etakyi@KITT Evelyn]$ ls
[etakyi@KITT Evelyn]$ ln-s /home/BIO594/Exercises/Week_7and8/simulated/*.fq.gz .
bash: ln-s: command not found...
[etakyi@KITT Evelyn]$ ln -s /home/BIO594/Exercises/Week_7and8/simulated/*.fq.gz .
[etakyi@KITT Evelyn]$ conda create -n week8 ddocent

CondaValueError: prefix already exists: /home/etakyi/miniconda3/envs/week8

[etakyi@KITT Evelyn]$ source activate week8
(week8) [etakyi@KITT Evelyn]$ ls
PopA_001.F.fq.gz  PopA_011.F.fq.gz  PopB_001.F.fq.gz  PopB_011.F.fq.gz  PopC_001.F.fq.gz  PopC_011.F.fq.gz  PopD_001.F.fq.gz  PopD_011.F.fq.gz
PopA_001.R.fq.gz  PopA_011.R.fq.gz  PopB_001.R.fq.gz  PopB_011.R.fq.gz  PopC_001.R.fq.gz  PopC_011.R.fq.gz  PopD_001.R.fq.gz  PopD_011.R.fq.gz
PopA_002.F.fq.gz  PopA_012.F.fq.gz  PopB_002.F.fq.gz  PopB_012.F.fq.gz  PopC_002.F.fq.gz  PopC_012.F.fq.gz  PopD_002.F.fq.gz  PopD_012.F.fq.gz
PopA_002.R.fq.gz  PopA_012.R.fq.gz  PopB_002.R.fq.gz  PopB_012.R.fq.gz  PopC_002.R.fq.gz  PopC_012.R.fq.gz  PopD_002.R.fq.gz  PopD_012.R.fq.gz
PopA_003.F.fq.gz  PopA_013.F.fq.gz  PopB_003.F.fq.gz  PopB_013.F.fq.gz  PopC_003.F.fq.gz  PopC_013.F.fq.gz  PopD_003.F.fq.gz  PopD_013.F.fq.gz
PopA_003.R.fq.gz  PopA_013.R.fq.gz  PopB_003.R.fq.gz  PopB_013.R.fq.gz  PopC_003.R.fq.gz  PopC_013.R.fq.gz  PopD_003.R.fq.gz  PopD_013.R.fq.gz
PopA_004.F.fq.gz  PopA_014.F.fq.gz  PopB_004.F.fq.gz  PopB_014.F.fq.gz  PopC_004.F.fq.gz  PopC_014.F.fq.gz  PopD_004.F.fq.gz  PopD_014.F.fq.gz
PopA_004.R.fq.gz  PopA_014.R.fq.gz  PopB_004.R.fq.gz  PopB_014.R.fq.gz  PopC_004.R.fq.gz  PopC_014.R.fq.gz  PopD_004.R.fq.gz  PopD_014.R.fq.gz
PopA_005.F.fq.gz  PopA_015.F.fq.gz  PopB_005.F.fq.gz  PopB_015.F.fq.gz  PopC_005.F.fq.gz  PopC_015.F.fq.gz  PopD_005.F.fq.gz  PopD_015.F.fq.gz
PopA_005.R.fq.gz  PopA_015.R.fq.gz  PopB_005.R.fq.gz  PopB_015.R.fq.gz  PopC_005.R.fq.gz  PopC_015.R.fq.gz  PopD_005.R.fq.gz  PopD_015.R.fq.gz
PopA_006.F.fq.gz  PopA_016.F.fq.gz  PopB_006.F.fq.gz  PopB_016.F.fq.gz  PopC_006.F.fq.gz  PopC_016.F.fq.gz  PopD_006.F.fq.gz  PopD_016.F.fq.gz
PopA_006.R.fq.gz  PopA_016.R.fq.gz  PopB_006.R.fq.gz  PopB_016.R.fq.gz  PopC_006.R.fq.gz  PopC_016.R.fq.gz  PopD_006.R.fq.gz  PopD_016.R.fq.gz
PopA_007.F.fq.gz  PopA_017.F.fq.gz  PopB_007.F.fq.gz  PopB_017.F.fq.gz  PopC_007.F.fq.gz  PopC_017.F.fq.gz  PopD_007.F.fq.gz  PopD_017.F.fq.gz
PopA_007.R.fq.gz  PopA_017.R.fq.gz  PopB_007.R.fq.gz  PopB_017.R.fq.gz  PopC_007.R.fq.gz  PopC_017.R.fq.gz  PopD_007.R.fq.gz  PopD_017.R.fq.gz
PopA_008.F.fq.gz  PopA_018.F.fq.gz  PopB_008.F.fq.gz  PopB_018.F.fq.gz  PopC_008.F.fq.gz  PopC_018.F.fq.gz  PopD_008.F.fq.gz  PopD_018.F.fq.gz
PopA_008.R.fq.gz  PopA_018.R.fq.gz  PopB_008.R.fq.gz  PopB_018.R.fq.gz  PopC_008.R.fq.gz  PopC_018.R.fq.gz  PopD_008.R.fq.gz  PopD_018.R.fq.gz
PopA_009.F.fq.gz  PopA_019.F.fq.gz  PopB_009.F.fq.gz  PopB_019.F.fq.gz  PopC_009.F.fq.gz  PopC_019.F.fq.gz  PopD_009.F.fq.gz  PopD_019.F.fq.gz
PopA_009.R.fq.gz  PopA_019.R.fq.gz  PopB_009.R.fq.gz  PopB_019.R.fq.gz  PopC_009.R.fq.gz  PopC_019.R.fq.gz  PopD_009.R.fq.gz  PopD_019.R.fq.gz
PopA_010.F.fq.gz  PopA_020.F.fq.gz  PopB_010.F.fq.gz  PopB_020.F.fq.gz  PopC_010.F.fq.gz  PopC_020.F.fq.gz  PopD_010.F.fq.gz  PopD_020.F.fq.gz
PopA_010.R.fq.gz  PopA_020.R.fq.gz  PopB_010.R.fq.gz  PopB_020.R.fq.gz  PopC_010.R.fq.gz  PopC_020.R.fq.gz  PopD_010.R.fq.gz  PopD_020.R.fq.gz
(week8) [etakyi@KITT Evelyn]$ dDocent
dDocent 2.2.25 

Contact jpuritz@gmail.com with any problems 

 
Checking for required software

All required software is installed!

dDocent run started Wed Apr 4 10:50:04 EDT 2018 

80 individuals are detected. Is this correct? Enter yes or no and press [ENTER]
yes
Proceeding with 80 individuals
dDocent detects 80 processors available on this system.
Please enter the maximum number of processors to use for this analysis.
80
dDocent detects 503G maximum memory available on this system.
Please enter the maximum memory to use for this analysis. The size can be postfixed with 
K, M, G, T, P, k, m, g, t, or p which would multiply the size with 1024, 1048576, 1073741824, 
1099511627776, 1125899906842624, 1000, 1000000, 1000000000, 1000000000000, or 1000000000000000 respectively.
For example, to limit dDocent to ten gigabytes, enter 10G or 10g
10g

Do you want to quality trim your reads?
Type yes or no and press [ENTER]?
yes

Do you want to perform an assembly?
Type yes or no and press [ENTER].
yes
What type of assembly would you like to perform?  Enter SE for single end, PE for paired-end, RPE for paired-end sequencing for RAD protocols with random shearing, or OL for paired-end sequencing that has substantial overlap.
Then press [ENTER]
PE
Reads will be assembled with Rainbow
CD-HIT will cluster reference sequences by similarity. The -c parameter (% similarity to cluster) may need to be changed for your taxa.
Would you like to enter a new c parameter now? Type yes or no and press [ENTER]
no
Proceeding with default 0.9 value.
Do you want to map reads?  Type yes or no and press [ENTER]
yes
BWA will be used to map reads.  You may need to adjust -A -B and -O parameters for your taxa.
Would you like to enter a new parameters now? Type yes or no and press [ENTER]
no
Proceeding with default values for BWA read mapping.
Do you want to use FreeBayes to call SNPs?  Please type yes or no and press [ENTER]
yes

Please enter your email address.  dDocent will email you when it is finished running.
Don't worry; dDocent has no financial need to sell your email address to spammers.
evelyn-takyi@my.uri.edu


dDocent will require input during the assembly stage.  Please wait until prompt says it is safe to move program to the background.
Trimming reads and simultaneously assembling reference sequences

                                                                                                                        
                      Number of Unique Sequences with More than X Coverage (Counted within individuals)                 
                                                                                                                        
  105000 +-+---------+-----------+-----------+-----------+----------+-----------+-----------+-----------+---------+-+   
         +           +           +           +           +          +           +           +           +           +   
         *****                                                                                                      |   
  100000 +-+  *                                                                                                   +-+   
         |     ******                                                                                               |   
         |           ******                                                                                         |   
         |                 ******                                                                                   |   
   95000 +-+                     ************                                                                     +-+   
         |                                   ******                                                                 |   
         |                                         ******                                                           |   
   90000 +-+                                             ******                                                   +-+   
         |                                                     *****                                                |   
         |                                                          ******                                          |   
   85000 +-+                                                              ******                                  +-+   
         |                                                                      ******                              |   
         |                                                                            ******                        |   
   80000 +-+                                                                                ******                +-+   
         |                                                                                        ******            |   
         |                                                                                              ******      |   
         |                                                                                                    ******|   
   75000 +-+                                                                                                      +-*   
         |                                                                                                          |   
         +           +           +           +           +          +           +           +           +           +   
   70000 +-+---------+-----------+-----------+-----------+----------+-----------+-----------+-----------+---------+-+   
         2           4           6           8           10         12          14          16          18          20  
                                                          Coverage                                                      
                                                                                                                        
Please choose data cutoff.  In essence, you are picking a minimum (within individual) coverage level for a read (allele) to be used in the reference assembly
4 

                                                                                                                        
                               Number of Unique Sequences present in more than X Individuals                            
                                                                                                                        
  3500 +-+-----------+------------+-------------+-------------+------------+-------------+------------+-----------+-+   
       +             +            +             +             +            +             +            +             +   
       |                                                                                                            |   
       |                                                                                                            |   
       |    *                                                                                                       |   
  3000 +-+   *                                                                                                    +-+   
       |      *                                                                                                     |   
       |       ***                                                                                                  |   
       |                                                                                                            |   
  2500 +-+        ***                                                                                             +-+   
       |                                                                                                            |   
       |             **                                                                                             |   
       |               ***                                                                                          |   
       |                  ***                                                                                       |   
  2000 +-+                   ***                                                                                  +-+   
       |                        **                                                                                  |   
       |                          ********                                                                          |   
       |                                  ******                                                                    |   
  1500 +-+                                      ********                                                          +-+   
       |                                                **************                                              |   
       |                                                              ****************                              |   
       |                                                                              *******************           |   
       +             +            +             +             +            +             +            +  ************   
  1000 +-+-----------+------------+-------------+-------------+------------+-------------+------------+-----------+-+   
       0             5            10            15            20           25            30           35            40  
                                                   Number of Individuals                                                
                                                                                                                        
Please choose data cutoff.  Pick point right before the assymptote. A good starting cutoff might be 10% of the total number of individuals
5
At this point, all configuration information has been entered and dDocent may take several hours to run.
It is recommended that you move this script to a background operation and disable terminal input and output.
All data and logfiles will still be recorded.
To do this:
Press control and Z simultaneously
Type 'bg' without the quotes and press enter
Type 'disown -h' again without the quotes and press enter

Now sit back, relax, and wait for your analysis to finish.
TrimmomaticSE: Started with arguments: -threads 80 -phred33 uniq.fq uniq.fq1 ILLUMINACLIP:/home/etakyi/miniconda3/envs/week8/bin/TruSeq2-PE.fa:2:30:10 MINLEN:153
Using PrefixPair: 'AATGATACGGCGACCACCGAGATCTACACTCTTTCCCTACACGACGCTCTTCCGATCT' and 'CAAGCAGAAGACGGCATACGAGATCGGTCTCGGCATTCCTGCTGAACCGCTCTTCCGATCT'
Using Long Clipping Sequence: 'AGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGTAGATCTCGGTGGTCGCCGTATCATT'
Using Long Clipping Sequence: 'AGATCGGAAGAGCGGTTCAGCAGGAATGCCGAGACCGATCTCGTATGCCGTCTTCTGCTTG'
Using Long Clipping Sequence: 'TTTTTTTTTTAATGATACGGCGACCACCGAGATCTACAC'
Using Long Clipping Sequence: 'TTTTTTTTTTCAAGCAGAAGACGGCATACGA'
Using Long Clipping Sequence: 'CAAGCAGAAGACGGCATACGAGATCGGTCTCGGCATTCCTGCTGAACCGCTCTTCCGATCT'
Using Long Clipping Sequence: 'AATGATACGGCGACCACCGAGATCTACACTCTTTCCCTACACGACGCTCTTCCGATCT'
ILLUMINACLIP: Using 1 prefix pairs, 6 forward/reverse sequences, 0 forward only sequences, 0 reverse only sequences
Input Reads: 2303 Surviving: 2303 (100.00%) Dropped: 0 (0.00%)
TrimmomaticSE: Completed successfully
 ____  _____    _    ____ 
|  _ \| ____|  / \  |  _ \
| |_) |  _|   / _ \ | |_) |
|  __/| |___ / ___ \|  _ <
|_|   |_____/_/   \_\_| \_\

PEAR v0.9.6 [January 15, 2015]

Citation - PEAR: a fast and accurate Illumina Paired-End reAd mergeR
Zhang et al (2014) Bioinformatics 30(5): 614-620 | doi:10.1093/bioinformatics/btt593

Forward reads file.................: ref.F.fq
Reverse reads file.................: ref.R.fq
PHRED..............................: 33
Using empirical frequencies........: YES
Statistical method.................: OES
Maximum assembly length............: 999999
Minimum assembly length............: 255
p-value............................: 0.001000
Quality score threshold (trimming).: 0
Minimum read size after trimming...: 1
Maximal ratio of uncalled bases....: 1.000000
Minimum overlap....................: 10
Scoring method.....................: Scaled score
Threads............................: 80

Allocating memory..................: 200,000,000 bytes
Computing empirical frequencies....: DONE
  A: 0.254631
  C: 0.245843
  G: 0.245899
  T: 0.253627
  0 uncalled bases
Assemblying reads: 100%

Assembled reads ...................: 0 / 1,000 (0.000%)
Discarded reads ...................: 0 / 1,000 (0.000%)
Not assembled reads ...............: 1,000 / 1,000 (100.000%)
Assembled reads file...............: overlap.assembled.fastq
Discarded reads file...............: overlap.discarded.fastq
Unassembled forward reads file.....: overlap.unassembled.forward.fastq
Unassembled reverse reads file.....: overlap.unassembled.reverse.fastq
================================================================
Program: CD-HIT, V4.7 (+OpenMP), Jul 11 2017, 18:04:58
Command: cd-hit-est -i totalover.fasta -o
         reference.fasta.original -M 0 -T 0 -c 0.9

Started: Wed Apr  4 10:52:08 2018
================================================================
                            Output                              
----------------------------------------------------------------
total number of CPUs in the system is 80
Actual number of CPUs to be used: 80

total seq: 1000
longest and shortest : 222 and 204
Total letters: 204356
Sequences have been sorted

Approximated minimal memory consumption:
Sequence        : 0M
Buffer          : 80 X 12M = 968M
Table           : 2 X 16M = 33M
Miscellaneous   : 4M
Total           : 1006M

Table limit with the given memory limit:
Max number of representatives: 248606
Max number of word counting entries: 9453957

# comparing sequences from          0  to       1000
.---------- new table with     1000 representatives

     1000  finished       1000  clusters

Apprixmated maximum memory consumption: 1007M
writing new database
writing clustering information
program completed !

Total CPU time 1.35
[bwa_index] Pack FASTA... 0.00 sec
[bwa_index] Construct BWT for the packed sequence...
[bwa_index] 0.03 seconds elapse.
[bwa_index] Update BWT... 0.00 sec
[bwa_index] Pack forward-only FASTA... 0.00 sec
[bwa_index] Construct SA from BWT and Occ... 0.02 sec
[main] Version: 0.7.17-r1188
[main] CMD: bwa index reference.fasta
[main] Real time: 0.100 sec; CPU: 0.060 sec
Using BWA to map reads.
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
[bam_sort_core] merging from 0 files and 80 in-memory blocks...
Creating alignment intervals
Using FreeBayes to call SNPs
Using VCFtools to parse TotalRawSNPS.vcf for SNPs that are called in at least 90% of individuals
(week8) [etakyi@KITT Evelyn]$ ls``

```
`Total raw snps = 3077   269371 11044653`
## Filtering of SNPs
vcftools --vcf TotalRawSNPs.vcf --max-missing 0.5 --maf 0.001 --minQ 20 --recode --recode-INFO-all --out TRS
After filtering, kept 2992 out of a possible 3018 Sites
vcftools --vcf TRS.recode.vcf --minDP 5 --recode --recode-INFO-all --out TRSdp5
After filtering, kept 2992 out of a possible 2992 Sites
pop_missing_filter.sh TRSdp5.recode.vcf ../popmap 0.05 1 TRSdp5p05
After filtering, kept 2820 out of a possible 2992 Sites
This script will automatically filter a FreeBayes generated VCF file using criteria related to site depth,
quality versus depth, strand representation, allelic balance at heterzygous individuals, and paired read representation.
The script assumes that loci and individuals with low call rates (or depth) have already been removed. 

Contact Jon Puritz (jpuritz@gmail.com) for questions and see script comments for more details on particular filters 

Number of sites filtered based on allele balance at heterozygous loci, locus quality, and mapping quality / Depth
 688 of 2820 

Number of additional sites filtered based on overlapping forward and reverse reads
 0 of 2132 

Is this from a mixture of SE and PE libraries? Enter yes or no.
no
Number of additional sites filtered based on properly paired status
 0 of 2132 

Number of sites filtered based on high depth and lower than 2*DEPTH quality score
 286 of 2132 


                                                                                                                        
                                             Histogram of mean depth per site                                           
                                                                                                                        
  250 +-+-+---+---+---+---+---+---+--+---+---+---+---+---+---+---+---+---+---+---+---+---+--+---+---+---+---+---+-+-+   
      +   +   +   +   +   +   +   +  +   +   +   +   +   +   +   +   +   +   +   +   +   +  +   +   +   +   +   +   +   
      |                                     **            'meandepthpersite' using (bin($1,binwidth)):(1.0) ******* |   
      |                                     **                                                                      |   
      |                                     ***                                                                     |   
  200 +-+                                  ****                                                                   +-+   
      |                                   *****                                                                     |   
      |                                   *****                                                                     |   
      |                                   *****                                                                     |   
  150 +-+                                *******                                                                  +-+   
      |                                  *******                                                                    |   
      |                                  *******                                                                    |   
      |                                  ********                                                                   |   
      |                                  ********                                                                   |   
  100 +-+                                ********                                                                 +-+   
      |                                  ********                                                                   |   
      |                                  ********                                                                   |   
      |                                **********                                                                   |   
   50 +-+                              **********                                                                 +-+   
      |                               ************                                                                  |   
      |                              **************                                                                 |   
      |                              ***************                                                                |   
      +   +   +   +   +   +   +   +  ****************+   +   +   +   +   +   +   +   +   +  +   +   +   +   +   +   +   
    0 +-+-+---+---+---+---+---+---+********************--+---+---+---+---+---+---+---+---+--+---+---+---+---+---+-+-+   
      10  15  20  25  30  35  40  45 50  55  60  65  70  75  80  85  90  95 100 105 110 11 120 125 130 135 140 145 150  
                                                        Mean Depth                                                      
                                                                                                                        
If distrubtion looks normal, a 1.645 sigma cutoff (~90% of the data) would be 5171.172995
The 95% cutoff would be 64
Would you like to use a different maximum mean depth cutoff than 64, yes or no
no
Number of sites filtered based on maximum mean depth
 233 of 2132 

Total number of sites filtered
 967 of 2820 

Remaining sites
 1853 

Filtered VCF file is called Output_prefix.FIL.recode.vcf

Filter stats stored in TRSdp5p05.filterstats.
After filtering, kept 1605 out of a possible 1985 Sites
Kept 1605 of a possible 1605 loci (filtered 0 loci)
vcftools --vcf SNP.TRSdp5p05FHWE.recode.vcf --maf 0.05 --recode --recode-INFO-all --out SNP.TRSdp5p05FHWEmaf05
After filtering, kept 857 out of a possible 1605 Sites

```

```
## Converting from VCF to other Output_prefix
BayeScan2.1_linux64bits SNP.TRSdp5p05FHWEBS -nbp 30 -thin 20 > bss.log
(week8) [etakyi@KITT filter]$ 12% 13% 14% 15% 16% 17% 18% 19% 20% 21% 22% 23% 24% 25% 26% 27% 28% 29% 30% 31% 32% 33% 34% 35% 36% 37% 38% 39% 40% 41% 42% 43% 44% 45% 46% 47% 48% 49% 50% 51% 52% 53% 54% 55% 56% 57% 58% 59% 60% 61% 62% 63% 64% 65% 66% 67% 68% 69% 70% 71% 72% 73% 74% 75% 76% 77% 78% 79% 80% 81% 82% 83% 84% 85% 86% 87% 88% 89% 90% 91% 92% 93% 94% 95% 96% 97% 98% 99% 
Calculation...
1% 2% 3% 4% 5% 6% 7% 8% 9% 10% 11% 12% 13% 14% 15% 16% 17% 18% 19% 20% 21% 22% 23% 24% 25%
### running bayescan at the background'
### running pcadapt
R
library(pcadapt)
reading file into pcadapt
> filename <- read.pcadapt("SNP.TRSdp5p05FHWE2A.recode.vcf", type = "vcf" )
No variant got discarded.
Summary:

	- input file:				SNP.TRSdp5p05FHWE2A.recode.vcf
	- output file:				SNP.TRSdp5p05FHWE2A.recode.pcadapt

	- number of individuals detected:	80
	- number of loci detected:		854
  x <- pcadapt(input = filename, K = 20)
Reading file /home/etakyi/repos/BIO_594_2018/Exercises/Week8/Evelyn/filter/SNP.TRSdp5p05FHWE2A.recode.pcadapt...
Number of SNPs: 854
Number of individuals: 80
> plot(x, option = "screeplot")
> plot(x, option = "screeplot")
> plot(x, option = "screeplot")
> plot(x, option = "screeplot", K = 10)
> plot(x, option = "screeplot")
> poplist.names <- c(rep("POPA", 20),rep("POPB", 20),rep("POPC", 20), rep("POPD",20))
> plot(x, option = "scores", pop = poplist.names)
> plot(x, option = "scores", i = 2, j = 3, pop = poplist.names)
> plot(x, option = "scores", i = 3, j = 4, pop = poplist.names)
> x <- pcadapt(filename, K = 3)
Reading file /home/etakyi/repos/BIO_594_2018/Exercises/Week8/Evelyn/filter/SNP.TRSdp5p05FHWE2A.recode.pcadapt...
Number of SNPs: 854
Number of individuals: 80
> 
> summary(x)
                Length Class  Mode   
scores           240   -none- numeric
singular.values    3   -none- numeric
zscores         2562   -none- numeric
loadings        2562   -none- numeric
maf              854   -none- numeric
missing          854   -none- numeric
stat             854   -none- numeric
gif                1   -none- numeric
chi2.stat        854   -none- numeric
pvalues          854   -none- numeric
> plot(x , option = "manhattan")
> plot(x , option = "manhattan")
> plot(x , option = "manhattan")
> plot(x, option = "qqplot", threshold = 0.1)
> plot(x, option = "stat.distribution")
> library(qvalue)
> qval <- qvalue(x$pvalues)$qvalues
> alpha <- 0.1
> outliers <- which(qval < alpha)
> outliers
 [1]  21  41  42 469 470 619 620 621 622 623 624 625 689 831

''' Testing for library effects''
poplist.names <- c(rep("LIB1", 40),rep("LIB2", 40))
> x <- pcadapt(input = filename, K = 20)
Reading file /home/etakyi/repos/BIO_594_2018/Exercises/Week8/Evelyn/filter/SNP.TRSdp5p05FHWE2A.recode.pcadapt...
Number of SNPs: 854
Number of individuals: 80
> plot(x, option = "scores", pop = poplist.names)
> plot(x, option = "scores", i = 2, j = 3, pop = poplist.names)
> x <- pcadapt(filename, K = 2)
Reading file /home/etakyi/repos/BIO_594_2018/Exercises/Week8/Evelyn/filter/SNP.TRSdp5p05FHWE2A.recode.pcadapt...
Number of SNPs: 854
Number of individuals: 80
> 
> summary(x)
                Length Class  Mode   
scores           160   -none- numeric
singular.values    2   -none- numeric
zscores         1708   -none- numeric
loadings        1708   -none- numeric
maf              854   -none- numeric
missing          854   -none- numeric
stat             854   -none- numeric
gif                1   -none- numeric
chi2.stat        854   -none- numeric
pvalues          854   -none- numeric
> plot(x , option = "manhattan")
> plot(x, option = "qqplot", threshold = 0.1)
> plot(x, option = "stat.distribution")
> qval <- qvalue(x$pvalues)$qvalues
> alpha <- 0.1
> outliers <- which(qval < alpha)
> outliers
[1]  41  42 469 470 496 689
'''Running BayeScan2
less bs.log 
(week8) [etakyi@KITT filter]$ R
source("plot_R.r")
> plot_bayescan("SNP.TRSdp5p05FH_fst.txt")
$outliers
[1] 472 473

$nb_outliers
[1] 2
''' Removing outliers 
 mawk '!/#/' SNP.TRSdp5p05FHWEmaf05.recode.vcf | wc -l
 paste <(seq 1 857) <( mawk '!/#/' SNP.TRSdp5p05FHWEmaf05.recode.vcf | cut -f1,2) 
 vcftools --vcf SNP.TRSdp5p05FHWEmaf05.recode.vcf --exclude-positions visuals  --recode-INFO-all --recode --out SNP.TRSdp5p05FHWEmaf05B

VCFtools - 0.1.14
(C) Adam Auton and Anthony Marcketta 2009

Parameters as interpreted:
	--vcf SNP.TRSdp5p05FHWEmaf05.recode.vcf
	--exclude-positions visuals
	--recode-INFO-all
	--out SNP.TRSdp5p05FHWEmaf05B
	--recode

After filtering, kept 80 out of 80 Individuals
Outputting VCF file...
After filtering, kept 855 out of a possible 857 Sites
Run Time = 1.00 seconds
'''Rerun bayescan to detect the removal of outliers  (neutral SNPs)
java -jar /usr/local/bin/PGDSpider2-cli.jar -inputfile SNP.TRSdp5p05FHWEmaf05B.recode.vcf  -outputfile SNP.TRSdp5p05FHWEBSF -spid BSsnp.spid
WARN  21:51:28 - PGDSpider configuration file not found! Loading default configuration.
initialize convert process...
read input file...
read input file done.
write output file...
write output file done.
BayeScan2.1_linux64bits SNP.TRSdp5p05FHWEBSF -nbp 30 -thin 20 > BS.log
BayeScan2.1_linux64bits SNP.TRSdp5p05FHWEBSF -nbp 30 -thin 20 > BS.log
plot_bayescan("SNP.TRSdp5p05FHW_fst.txt")
$outliers
integer(0)

$nb_outliers
[1] 0

```
## PCA plot 
library(adegenet)
Loading required package: ade4

   /// adegenet 2.1.1 is loaded ////////////

   > overview: '?adegenet'
   > tutorials/doc/questions: 'adegenetWeb()' 
   > bug reports/feature requests: adegenetIssues()


> library(vcfR)

   *****       ***   vcfR   ***       *****
   This is vcfR 1.7.0 
     browseVignettes('vcfR') # Documentation
     citation('vcfR') # Citation
   *****       *****      *****       *****

> my_vcf <- read.vcfR("SNP.TRSdp5p05FHWEmaf05B.recode.vcf")
Scanning file to determine attributes.
File attributes:
  meta lines: 63
  header line: 64
  variant count: 855
  column count: 89
Meta line 63 read in.
All meta lines processed.
gt matrix initialized.
Character matrix gt created.
  Character matrix gt rows: 855
  Character matrix gt cols: 89
  skip: 0
  nrows: 855
  row_num: 0
Processed variant: 855
All variants processed
> my_genind <- vcfR2genind(my_vcf)
> strata<- read.table("strata", header=TRUE)
> strata_df <- data.frame(strata)
> strata(my_genind) <- strata_df
> setPop(my_genind) <- ~Population
X <- tab(my_genind, freq = TRUE, NA.method = "mean")
> pca1 <- dudi.pca(X, scale = FALSE, scannf = FALSE, nf = 3)
> barplot(pca1$eig[1:50], main = "PCA eigenvalues", col = heat.colors(50))
> s.class(pca1$li, pop(my_genind))
> title("PCA of simulated dataset\naxes 1-2")
> add.scatter.eig(pca1$eig[1:20], 3,1,2)
> 
> col <- funky(15) 
> s.class(pca1$li, pop(my_genind),xax=1,yax=2, col=col, axesell=FALSE, cstar=0, cpoint=3, grid=FALSE)
DAPC
dapc1 <- dapc(my_genind, grp$grp)
Choose the number PCs to retain (>=1): 40
Choose the number discriminant functions to retain (>=1): 2
> scatter(dapc1,col=col,bg="white", solid=1)

```
## for real data
run BayeScan

java -jar /usr/local/bin/PGDSpider2-cli.jar -inputfile SNP.DP3g98maf01_85INDoutFIL.NO2a.HWE.FIL.recode.vcf  -outputfile SNP.TRSdp5p05FHWEBayEnv.txt -spid SNPBayEnv.spid
log4j:ERROR setFile(null,true) call failed.

## I keep getting an error.

```
