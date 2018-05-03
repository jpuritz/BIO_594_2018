# Final Assignment
## Erin M. Roberts

### Goal: Determine Neutral Population Structure of the eastern oyster *C. virginica* from 14 populations from 4  biogeographic populations on the East coast of the United States.

#### Data set and Additional Files Necessary to perform the analyses
1. HiSeq Data Sets sequenced on an Illumina HiSeq X Ten PE150, sequenced without PCR concentration. The full sequence
set has been limited to only natural populations from high and low salinity from wild populations. This decreases the data set to the following 9 populations:

| Population Name       | Region         | Location Sampled                           | Ecotype       | Wild/Selected |
|-----------------------|----------------|--------------------------------------------|---------------|---------------|
|1. Laguna Madre (LM)   | Gulf of Mexico | Port Mansfield, TX                         | NA            | Wild          |
|2. Hope Creek (HC)     | Delaware Bay   | Hope Creek, NJ                             | Low salinity  | Wild          |
|3. Cape Shore (CS)     | Delaware Bay   | Cape Shore, NJ                             | High salinity | Wild          |
|4. Sherman Marsh (SM)  | Maine          | Sherman Marsh/Sheepscot River, ME          | Low salinity  | Wild          |    
|5. Hog Island (HI)     | Maine          | Hog Island, Damariscotta River Estuary, ME | High salinity | Wild          |
|6. Sister Lake (SL)    | Louisiana      | Caillou Lake, LA                           | NA            | Wild          |
|7. Calcasieu Lake (CL) | Louisiana      | Grand Isle, LA                             | NA            | Wild          |
|8. Chlora's Point (CLP)| Chesapeake Bay | Choptank River- Chesapeake Bay, VA         | Low salinity  | Wild          |
|9. Hummock Cove (HC-VA)| Chesapeake Bay | Chesapeake Bay, VA                         | High salinity | Wild          |


2. HiSeq Read Set Sequencing Metadata


| Name	  | Run Type	| Library Source| Library Type	    | Adaptor	| Read # 	| Number of Bases	| Average Quality | Percent Duplicate |
|---------|-----------|---------------|-------------------|---------|---------|-----------------|-----------------|-------------------|
|CS-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34226714	|9515026492	      |38	              | 5.929             |
|CS-2	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36064101	|10891358502	    |37	              | 6.62              |
|CS-2	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|29122012	|8095919336	      |37	              | 5.535             |
|CS-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34267784	|10348870768	    |38	              | 6.786             |
|CS-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|29876081	|8305550518	      |38	              | 5.696             |
|CS-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|37958616	|11463502032	    |38	              | 6.66              |
|CS-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|30041328	|8351489184	      |38	              | 5.521             |
|CS-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|32002481	|9664749262	      |37	              | 7.269             |
|CS-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34888554	|10536343308	    |38	              | 6.659             |
|CS-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|32783702	|9113869156	      |38	              | 5.613             |
|HC-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|38646818	|11671339036	    |38	              | 8.318             |
|HC-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|38646818	|11671339036	    |38	              | 8.318             |
|HC-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31556239	|9529984178	      |38	              | 7.612             |
|HC-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31556239	|9529984178	      |38	              | 7.612             |
|HC-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39877222	|12042921044	    |38	              | 7.606             |
|HC-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39877222	|12042921044	    |38	              | 7.606             |
|HC-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|45016816	|13595078432	    |37	              | 7.035             |
|HC-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36535596	|10156895688	    |38	              | 5.065             |
|HC-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|45016816	|13595078432	    |37	              | 7.035             |
|HC-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36535596	|10156895688	    |38	              | 5.065             |
|HC-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|28024130	|8463287260	      |38	              | 6.819             |
|HC-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|28024130	|8463287260	      |38	              | 6.819             |
|HC-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|77299611	|23344482522	    |37	              | 7.158             |
|HC-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|50348381	|13996849918	    |37	              | 5.841             |
|HC-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|77299611	|23344482522	    |37	              | 7.158             |
|HC-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|50348381	|13996849918	    |37	              | 5.841             |
|HC-VA-1	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42970224	|12977007648	    |37	              | 7.839             |
|HC-VA-1	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36814199	|10234347322	    |37	              | 6.051             |
|HC-VA-1	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42970224	|12977007648	    |37	              | 7.839             |
|HC-VA-1	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36814199	|10234347322	    |37	              | 6.051             |
|HC-VA-2	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|41451075	|12518224650	    |37	              | 7.733             |
|HC-VA-2	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35187075	|9782006850	      |37	              | 6.042             |
|HC-VA-2	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|41451075	|12518224650	    |37	              | 7.733             |
|HC-VA-2	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35187075	|9782006850	      |37	              | 6.042             |
|HC-VA-3	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31945464	|9647530128	      |37	              | 5.78              |
|HC-VA-3	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31604568	|8786069904	      |38	              | 4.807             |
|HC-VA-3	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31945464	|9647530128	      |37	              | 5.78              |
|HC-VA-3	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31604568	|8786069904	      |38	              | 4.807             |
|HC-VA-4	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34803290	|10510593580	    |38	              | 6.292             |
|HC-VA-4	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|32573378	|9055399084	      |38	              | 5.213             |
|HC-VA-4	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34803290	|10510593580	    |38	              | 6.292             |
|HC-VA-4	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|32573378	|9055399084	      |38	              | 5.213             |
|HC-VA-5	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39877905	|12043127310	    |38	              | 7.672             |
|HC-VA-5	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31515900	|8761420200	      |38	              | 5.973             |
|HC-VA-5	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39877905	|12043127310	    |38	              | 7.672             |
|HC-VA-5	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31515900	|8761420200	      |38	              | 5.973             |
|HC-VA-6	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42747638	|12909786676	    |37	              | 8.127             |
|HC-VA-6	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35426923	|9848684594	      |37	              | 6.284             |
|HC-VA-6	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42747638	|12909786676	    |37	              | 8.127             |
|HC-VA-6	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35426923	|9848684594	      |37	              | 6.284             |
|HI-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39293670	|11866688340	    |38	              | 7.201             |
|HI-2	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|59177432	|17871584464	    |38	              | 8.012             |
|HI-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42116311	|12719125922	    |38	              | 7.662             |
|HI-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|38708892	|11690085384	    |38	              | 7.583             |
|HI-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|52019244	|15709811688	    |38	              | 7.675             |
|HI-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39366994	|11888832188	    |38	              | 7.289             |
|LM-1_pool|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|33484657	|10112366414	    |37	              | 8.285             |
|LM-1_pool|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|29307831	|8147577018	      |37	              | 6.53              |
|LM-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|46243120	|13965422240	    |37	              | 6.294             |
|LM-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|40743407	|11326667146	    |38	              | 5.121             |
|LM-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|86188161	|26028824622	    |37	              | 6.666             |
|LM-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|72516832	|20159679296	    |38	              | 5.517             |
|LM-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|37559493	|11342966886	    |38	              | 6.095             |
|LM-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39108440	|10872146320	    |38	              | 5.058             |
|LM-8	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|33186635	|10022363770	    |38	              | 5.956             |
|LM-8	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36375900	|10112500200	    |38	              | 4.925             |
|SL-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|44573789	|13461284278	    |38	              | 6.735             |
|SL-2	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|29619024	|8944945248	      |38	              | 6.44              |
|SL-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|46847209	|14147857118	    |38	              | 7.176             |
|SL-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|30848151	|9316141602	      |38	              | 6.614             |
|SL-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|49922036	|15076454872	    |38	              | 7.224             |
|SL-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|38193328	|11534385056	    |38	              | 6.76              |
|SM-10	  |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|41831639	|12633154978	    |38	              | 7.644             |
|SM-11	  |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31690949	|9570666598	      |38	              | 6.868             |
|SM-12	  |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35796533	|10810552966	    |38	              | 7.461             |
|SM-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|47538272	|14356558144	    |38	              | 8.639             |
|SM-8	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35781255	|10805939010	    |38	              | 7.666             |
|SM-9	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35628014	|10759660228	    |38	              | 6.895             |

#### Step 1: Download and acquire the Data

All sequence data has been downloaded onto KITT by JP. To access the data a symbolic link will be created using the following commands.

```
# Link to only the natural population files
cd /home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files

declare -a forward_array=(/home/Shared_Data/LM*.F.fq.gz /home/Shared_Data/HC_?.F.fq.gz /home/Shared_Data/CS*.F.fq.gz /home/Shared_Data/SM*.F.fq.gz /home/Shared_Data/HI*.F.fq.gz /home/Shared_Data/SL*.F.fq.gz /home/Shared_Data/CL_*.F.fq.gz /home/Shared_Data/CLP*.F.fq.gz /home/Shared_Data/HC_VA*.F.fq.gz)

declare -a reverse_array=(/home/Shared_Data/LM*.R.fq.gz /home/Shared_Data/HC_?.R.fq.gz /home/Shared_Data/CS*.R.fq.gz /home/Shared_Data/SM*.R.fq.gz /home/Shared_Data/HI*.R.fq.gz /home/Shared_Data/SL*.R.fq.gz /home/Shared_Data/CL_*.R.fq.gz /home/Shared_Data/CLP*.R.fq.gz /home/Shared_Data/HC_VA*.R.fq.gz)

for i in ${forward_array[@]}; do
  ln -s ${i} /home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
done

for i in ${reverse_array[@]}; do
  ln -s ${i} /home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
done

#check if I have the correct number of sequence Sets
ls *.fq.gz | wc -l # 106

```

#### Step 2: Check Sum of Genome Quebec Data
Use wget command supplied by GenomeQuebec to  automatically download all data, generate checksum file, and perform checksum.

```
wget -O - "https://genomequebec.mcgill.ca/nanuqMPS/readsetList?projectId=15565&tech=HiSeq" --no-cookies --no-check-certificate --post-data 'j_username=username&j_password=password' | wget --no-cookies --no-check-certificate --post-data 'j_username=username&j_password=password' -ci -
```


#### Step 3: Initial Raw Data Assessment and Characterization
1. Read counts

Read counts are provided in metadata file and checked using checksum.

2. Read quality of each sample group

Use FASTQC to create FASTQC report with:
  a. Basic statistics
  b. Per base sequence quality scores
  c. Per sequence quality scores
  d. Per base GC content
  e. Per sequence GC content
  f. Per sequence GC content

  ```
# Upload FASTQC environment using conda create
conda create -n natural_pop_files fastqc

# Activate the environment
source activate natural_pop_files

# Generate sequence quality report for each population using command fastqc
declare -a pop_array=(./LM*.F.fq.gz ./HC_?.F.fq.gz ./CS*.F.fq.gz ./SM*.F.fq.gz ./HI*.F.fq.gz ./SL*.F.fq.gz ./CL_*.F.fq.gz ./CLP*.F.fq.gz ./HC_VA*.F.fq.gz)

for i in ${pop_array[@]}; do
  fastqc ${i}
  echo "finished ${i}" $date
done

declare -a pop_R_array=(./LM*.R.fq.gz ./HC_?.R.fq.gz ./CS*.R.fq.gz ./SM*.R.fq.gz ./HI*.R.fq.gz ./SL*.R.fq.gz ./CL_*.R.fq.gz ./CLP*.R.fq.gz ./HC_VA*.R.fq.gz)

for i in ${pop_R_array[@]}; do
  fastqc ${i}
  echo "finished ${i}" $date
done

# Faster approach if all files are in the same folder and can disown the process source

for i in *.fq.qz; do
  fastqc $i
done

# Put process into the background using
^Z
bg
disown -a

# Check that all files have been completed by comparing arrays with bash
declare -a total_array=(./LM*.F.fq.gz ./HC_?.F.fq.gz ./CS*.F.fq.gz ./SM*.F.fq.gz ./HI*.F.fq.gz ./SL*.F.fq.gz ./CL_*.F.fq.gz ./CLP*.F.fq.gz ./HC_VA*.F.fq.gz ./LM*.R.fq.gz ./HC_?.R.fq.gz ./CS*.R.fq.gz ./SM*.R.fq.gz ./HI*.R.fq.gz ./SL*.R.fq.gz ./CL_*.R.fq.gz ./CLP*.R.fq.gz ./HC_VA*.R.fq.gz)
for i in ${total_array[@]}; do
  echo ${i} | sed 's/.fq.gz/_fastqc.html/g' >> total_array.txt
done
declare -a total_array=($(cat total_array.txt))
declare -a html_array=(./*.html)
echo ${total_array[@]} ${html_array[@]} | tr ' ' '\n' | sort | uniq -u #any left over are those that weren't converted to fastqc
# Failed to process file HI_2.R.fq.gz. This file is excluded from FASTQC analysis

# use MultiQC to put together all Files
#make new folder with all Fastqc files
mkdir fastqc_results
mv *.zip ./fastqc_results
cd fastqc_results
conda install -c bioconda multiqc
multiqc .

# Export file to local folder so you can open it up with .html
cd /Users/erinroberts/Documents/PHD_coursework_TA/Puritz_pop_gen
scp -P 2292 eroberts@kitt.uri.edu:/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files/fastqc_results/multiqc_report.html .
```

### MultiQC Results

1. GC content: The GC content was either 35% or 36% across all reads.
2. % failed: None failed the QC report
3. % Duplicates: The highest percent duplicates was 12.5%. Most were lower than this.
4. Mean Quality Score: 105/105 Samples Passed
This graph depicts the mean quality score at each position across a read.
![Mean Quality Score](https://github.com/jpuritz/BIO_594_2018/blob/master/FinalAssignment/EMR_Final_Assignment/Mean_quality_histogram_natural_pops_5_3_18.png "This graph depicts the mean quality score at each position across a read.")
5. Per Sequence Quality Score: 105/105 Samples Passed
This graph depicts the number of reads with average quality scores.
![Per Sequence Quality Score](https://github.com/jpuritz/BIO_594_2018/blob/master/FinalAssignment/EMR_Final_Assignment/Per_sequence_quality_scores_natural_pops_5_3_18.png "This graph depicts the number of reads with average quality scores.")
6. Per Sequence GC Content
This graph depicts the average GC contents of reads and is roughly normally distributed.
![Per Sequence GC Content](https://github.com/jpuritz/BIO_594_2018/blob/master/FinalAssignment/EMR_Final_Assignment/Per_sequence_GC_content_natural_pops_5_3_18.png "This graph depicts the average GC contents of reads and is roughly normally distributed")

Overall the sequence quality is high and we will proceed with further analysis. 


#### Step 4: Bioinformatic Processing

1. Adaptor trimming using fastqc-mcf
The user manual for this tool can be found here: https://github.com/ExpressionAnalysis/ea-utils/blob/wiki/FastqMcf.md

The adapters used for this project for multiplexing on a Hiseq 2000 were as follows:

>Hi_seq_Adaptor_Read_1
AGATCGGAAGAGCACACGTCTGAACTCCAGTCAC
>Hi_seq_Adaptor_Read_2
AGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGT

These sequences were input into a file called Hi_seq_adaptors.fa.


Install the software fastqc-mcf (from the ea-utils package)
```
#install ea-utils
conda install -c bioconda ea-utils
```
Run the following script to perform read trimming of HiSeq 2000 adapter, trim low quality ends of reads with a Phred score of less than 20 and remove whole reads with an average score of less than 10.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls $F/*.F.fq.gz | sed 's/.F.fq.gz//g'))

for file in ${array1[@]};do
/home/eroberts/miniconda3/bin/fastq-mcf \
$F/Hi_seq_adaptors.fa\
$F/${file}.F.fq.gz \
$F/${file}.R.fq.gz \
-l 100 \
-q 20 \
-w 5 \
-x 10 \
-u \
-P 33 \
-o $F/${file}.F.cleaned.fq.gz \
-o $F/${file}.R.cleaned.fq.gz &> $F/${file}.trimmed
done

# o =output
# l = minumum remaining sequence Length
# q = quality threshold causing base removal at the end of reads
# w = window size for for quality trimming
# -x = 'N' bad read percentage causing cycle removal

```

# Step 5. Read Mapping to Reference using BWA-MEM
BWA-MEM is recommended for longer sequences that range from 70bp to 1Mbp. It is recommended over BWA-SW and BWA-backtrak because it is faster and more accurate.

The reference file being used is the eastern oyster reference mRNA from NCBI: GCF_002022765.2_C_virginica-3.0_rna.fna. Using this file means that any aligned genes will have the gene information attached.

1. Set up a reference index using samtools faidx

```
# copy genome into folder from bluewaves
scp erin_roberts@bluewaves:/data3/marine_diseases_lab/shared/GCA_002022765.4_C_virginica-3.0_genomic.fna .
# create a reference index
samtools faidx GCF_002022765.2_C_virginica-3.0_rna.fna

```
Create a bwa index for use by BWA and then use bwa mem to generate sam records for each read and samtools to sort the bam file.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls $F/*.F.fq.gz | sed 's/.F.fq.gz//g'))

bwa index GCF_002022765.2_C_virginica-3.0_rna.fna

for i in ${array1[@]}; do
  bwa mem GCF_002022765.2_C_virginica-3.0_genomic.fna ${i}.F.fq.gz ${i}.R.fq.gz  -t 8 -a -M -B 3 -O 5 -R "@RG\tID:${i}\tSM:${i}\tPL:Illumina" 2> bwa.${i}.log | samtools view -@4 -q 1 -SbT GCF_002022765.2_C_virginica-3.0_genomic.fna - > ${i}.bam
  samtools sort -@8 $.bam -o ${i}.bam && samtools index ${i}.bam
done
```

# 3. Mark and filter out any potential duplicate reads using PICARD
Because libraries were generated without a PCR prep, there should not be duplicate reads. However, this serves as a check of this.

```
# Download the PICARD tool
wget https://github.com/broadinstitute/picard/releases/download/2.17.8/picard.jar

# Mark and output duplicates

F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls $F/*.bam| sed 's/.bam//g'))

for i in ${array1[@]; do
  java -Xms4g -jar picard.jar MarkDuplicatesWithMateCigar I=${i}.bam O=${i}md.bam M=${i}_dup_metrics.txt MINIMUM_DISTANCE=300
done
```
Now we are able to remove duplicates as well as any secondary alignments, mappings with a quality score of less than ten, and reads with more than 80 bp clipped. Finally we can create a BAM index from our fully processed files.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls $F/*md.bam))

for i in ${array1[@]; do
  samtools view -@8 -h -F 0x100 -q 10 -F 0x400 ${i}md.bam | mawk '$6 !~/[8-9].[SH]/ && $6 !~ /[1-9][0-9].[SH]/'| samtools view -@8 -b > ${i}.F.bam
  samtools index ${i}.F.bam
done

```
The command below can then be used to check that reads have been filtered out.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls $F/*.bam| sed 's/.bam//g'))

for i in ${array1[@]; do
  paste <(samtools view -c ${i}md.bam) <(samtools view -c ${i}.F.bam )
done
```

# 4. Calculate depth per bp along the reference using samtools

The final filtered bam files have now been generated and we can check the sequencing depth per base pair. The output is a text file with three columns. The first column lists the chromosome, the second column is the base pair and the third column is the depth at that base pair.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=(ls $F/*.F.bam)
for i in ${array1[@]; do
  samtools depth -aa ${i}.F.bam > ${i}.genome.depth
done
```

# 5. Perform Variant Calling with FreeBayes

Now that our final bam files have been generated we can call variants using the program FreeBayes.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=(ls $F/*.F.bam)
for i
freebayes -f GCF_002022765.2_C_virginica-3.0_rna.fna


# for the PCAdapt code look at Week 7 lecture code

# Works used for reference:
http://clavius.bc.edu/~erik/CSHL-advanced-sequencing/freebayes-tutorial.html
https://github.com/ekg/alignment-and-variant-calling-tutorial

