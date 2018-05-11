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
sh -c 'for file in "CL_1" "CL_2" "CL_3" "CL_4" "CL_5" "CL_6" "CLP_1" "CLP_2" "CLP_3" "CLP_4" "CLP_5" "CLP_6" "CS_1" "CS_2" "CS_3" "CS_5" "CS_6" "CS_7" "HC_1" "HC_3" "HC_4" "HC_5" "HC_6" "HC_7" "HC_VA_1" "HC_VA_2" "HC_VA_3" "HC_VA_4" "HC_VA_5" "HC_VA_6" "HI_1" "HI_2" "HI_3" "HI_4" "HI_5" "HI_6" "LM_1_pool" "LM_3" "LM_4" "LM_7" "LM_8" "SL_1" "SL_2" "SL_3" "SL_4" "SL_5" "SL_6" "SM_10" "SM_11" "SM_12" "SM_7" "SM_8" "SM_9"
do
echo "start ${file} $(date)"
/home/eroberts/miniconda3/bin/fastq-mcf \
/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files/Hi_seq_adaptors.fa \
/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files/${file}.F.fq.gz \
/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files/${file}.R.fq.gz \
-l 100 \
-q 20 \
-w 5 \
-x 10 \
-u \
-P 33 \
-o /home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files/${file}.F.cleaned.fq.gz \
-o /home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files/${file}.R.cleaned.fq.gz &> /home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files/${file}.log
echo "${file} done $(date)"
done'

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
# create a reference index in samtools
samtools faidx GCA_002022765.4_C_virginica-3.0_genomic.fna

```
Create a bwa index for use by BWA and then use bwa mem to generate sam records for each read and samtools to sort the bam file.

Put the following code into a bash script and run the bash script to execute.
$ nano bwa.sh
$ bash bwa.sh
```
#!/bin/bash
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls *.F.cleaned.fq.gz | sed 's/.F.cleaned.fq.gz//g'))

#bwa index GCA_002022765.4_C_virginica-3.0_genomic.fna
echo "done index $(date)"

for i in ${array1[@]}; do
  bwa mem $F/GCA_002022765.4_C_virginica-3.0_genomic.fna ${i}.F.cleaned.fq.gz ${i}.R.cleaned.fq.gz -t 8 -a -M -B 3 -O 5 -R "@RG\tID:${i}\tSM:${i}\tPL:Illumina" 2> bwa.${i}.log | samtools view -@4 -q 1 -SbT $F/GCA_002022765.4_C_virginica-3.0_genomic.fna - > ${i}.bam
  echo "done ${i}"
done

array2=($(ls *.bam | sed 's/.bam//g'))

#now sort the bam files with samtools sort
for i in ${array2[@]}; do
  samtools sort -@8 ${i}.bam -o ${i}.bam && samtools index ${i}.bam
done
```

# STEP 6. Mark and filter out any potential duplicate reads using PICARD
Because libraries were generated without a PCR prep, there should not be duplicate reads. However, this serves as a check of this.

```
# Download the PICARD tool
wget https://github.com/broadinstitute/picard/releases/download/2.17.8/picard.jar

# Mark and output duplicates

F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls *.bam| sed 's/.bam//g'))

for i in ${array1[@]}; do
  java -Xms4g -jar picard.jar MarkDuplicatesWithMateCigar I=${i}.bam O=${i}.md.bam M=${i}_dup_metrics.txt MINIMUM_DISTANCE=300
done
```
Now we are able to remove duplicates as well as any secondary alignments, mappings with a quality score of less than ten, and reads with more than 80 bp clipped. Finally we can create a BAM index from our fully processed files.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls *.md.bam | sed 's/.md.bam//g'))

for i in ${array1[@]; do
  samtools view -@8 -h -F 0x100 -q 10 -F 0x400 ${i}.md.bam | mawk '$6 !~/[8-9].[SH]/ && $6 !~ /[1-9][0-9].[SH]/'| samtools view -@8 -b > ${i}.F.bam
  samtools index ${i}.F.bam
done

```
The command below can then be used to check that reads have been filtered out.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=($(ls *.md.bam | sed 's/.md.bam//g'))

for i in ${array1[@]; do
  paste <(samtools view -c ${i}.md.bam) <(samtools view -c ${i}.F.bam )
done
```

# STEP 7. Calculate depth per bp along the reference using samtools

The final filtered bam files have now been generated and we can check the sequencing depth per base pair. The output is a text file with three columns. The first column lists the chromosome, the second column is the base pair and the third column is the depth at that base pair.

```
F=/home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
array1=(ls *.F.bam | sed 's/.F.bam//g')
for i in ${array1[@]; do
  samtools depth -aa ${i}.F.bam > ${i}.genome.depth
done
```

# STEP 8. Perform Variant Calling with FreeBayes,

Now that our final .bam files have been generated we can call variants using the program FreeBayes. Variants can be called for files individually or jointly.

```
cd home/eroberts/repos/BIO_594_2018/FinalAssignment/EMR_Final_Assignment/natural_pop_files
#give FreeBayes a list of all the input files and call them jointly
ls *.F.bam > bamlist.txt
freebayes -f GCF_002022765.2_C_virginica-3.0_rna.fna -L bamlist.txt >  total_SNPs_ALLPOP.vcf

```

# STEP 9. Filter SNPs using VCFTools

The following steps were adapted from an excellent protocol developed by Jon Puritz. For more detailed information please see [http://ddocent.com/filtering/](http://ddocent.com/filtering/)

1. First we will use VCFTools to filter out any variants that have not been successfully genotyped to more than 50% of individuals ( `--max-missing 0.5`), those with a minor allele count of 3 (`--mac 3)`), and those with a quality score below 30 (`--minQ 30`)  

```
vcftools --vcf total_ALLPOP.vcf --max-missing 0.5 --mac 3 --minQ 20 --recode --recode-INFO-all --out total_ALLPOP.g5mac3

```

2. Getting rid of these first will help speed up this next command, which applies a minimum mean depth and a minimum depth for a genotype call. Genotypes will be called if they have atleast three reads.

```
vcftools --vcf total_ALLPOP.firstfilter.recode.vcf --minDP 3 --recode --recode-INFO-all --out total_ALLPOP.g5mac3dp3
```

3. Now we can remove individuals that have a lot of missing data.

```
# The output of this file will be called out.imiss
vcftools --vcf total_ALLPOP.g5mac3dp3.recode.vcf --missing-indv

```
4. We can now plot a histogram of individuals that are missing a lot of data using the following command (taken from http://ddocent.com/filtering/ by Jon Puritz).

```
mawk '!/IN/' out.imiss | cut -f5 > totalmissing
gnuplot << \EOF
set terminal dumb size 120, 30
set autoscale
unset label
set title "Histogram of % missing data per individual"
set ylabel "Number of Occurrences"
set xlabel "% of missing data"
#set yr [0:100000]
binwidth=0.01
bin(x,width)=width*floor(x/width) + binwidth/2.0
plot 'totalmissing' using (bin($1,binwidth)):(1.0) smooth freq with boxes
pause -1
EOF
```
5. We can create a list with more than 50% missing data using the following mawk command.
```
mawk '$5 > 0.5' out.imiss | cut -f1 > lowDP.indv
```
6. This can then be piped into VCFtools so that the low coverage individuals can be removed.
```
vcftools --vcf total_ALLPOP.g5mac3dp3.recode.vcf --remove lowDP.indv --recode --recode-INFO-all --out total_ALLPOP.g5mac3dp3dplm

```
7. Next, we need to restrict the data to those variants that are called in a high percentage of individuals using a genotype call rate of 95% (`--max-missing 0.95`) and then filter based on the mean depth of genotypes of 20% (`--min-meanDP 20`).
```
vcftools --vcf total_ALLPOP.g5mac3dp3dplm.recode.vcf --max-missing 0.95 --maf 0.05 --recode --recode-INFO-all --out total_ALLPOPDP3g95maf05 --min-meanDP 20
```

8. Finally, because we are analyzing several individuals, we need to apply a population specific filter. To do this we first need to create what's called a "popmap" file. This file contains two tab separated columns. Lets create one based on our data.

```
array2=($(ls *.F.cleaned.fq.gz | sed 's/.F.cleaned.fq.gz//g'))

for i in ${array2[@]}; do
  echo -e "${i}:${i}" | awk  '{gsub(":","\t",$0); print;}' >> popmap
done
awk '{split($2,a,/_/);$2=a[1]}1' popmap > popmap_final  
sed 's/ /\t/g' popmap_final > popmap_final_TD

#note: manually added _VA to HC_VA lines using nano
```
8a. Now we need to create 9 lists that have the individual names of each population. We can do this with the following commands that can be used for whatever the unique names of your populations might be.

```
cut -f 2 popmap_final_TD | sort | uniq > unique.txt

#!/bin/bash
while read -r i; do
  echo $i > $i.keep
done < unique.txt

```  
8b. We can use these files to estimate the missing data for loci in each population using vcftools.

```
array3=($(ls *.keep | sed 's'/.keep//')
for i in ${array3[@]}; do
  vcftools --vcf total_ALLPOP.DP3g95maf05.recode.vcf --keep ${i}.keep --missing-site --out ${i}
done
```
8c. The output of the above commands outputs files called `*.lmiss` whose last column lists the percentage of missing data for that locus. We can merge all of these files to create a list of loci that have 10% missing data or more to remove.

```
cat CL.lmist CLP.lmiss CS.lmiss HC.lmiss HC_VA.lmiss HI.lmiss LM.lmiss SL.lmiss SM.lmiss | mawk '!/CHR/' | mawk '$6 > 0.1' | cut -f1,2 >> badloci

```
8d. Finally, we can pipe this back into VCFTools to remove any of those bad loci

```
vcftools --vcf total_ALLPOP.DP3g95maf05.recode.vcf --exclude-positions badloci --recode --recode-INFO-all --out total_ALLPOP.DP3g95p5maf05

```
9. Next we can apply a filter that remove sites that have reads from both strands. The filter command is going to keep loci that have over 100 times more forward alternate reads than reverse alternate reads and 100 times more forward reference reads than reverse reference reads along with the reciprocal.

```
vcffilter -f "SAF / SAR > 100 & SRF / SRR > 100 | SAR / SAF > 100 & SRR / SRF > 100" -s total_ALLPOP.DP3g95p5maf05.recode.vcf > total_ALLPOP.DP3g95p5maf05.fil1.vcf

# To investigate how many reads were remove we can see how many lines remain
mawk '!/#/' total_ALLPOP.DP3g95p5maf05.fil1.vcf | wc -l

```
10. Apply a filter to account for high coverage causing an inflated locus quality score

Heng Li found that in whole genome samples, high coverage can lead to inflated locus quality scores. Based on this, Jon Purtiz suggests the following filter to remove any locus that has a quality score below 1/4 of the depth. Because we are not working with RADseq data, we will not implement the second filter he suggest to recalculate mean depth.

```
vcffilter -f "QUAL / DP > 0.25" total_ALLPOP.DP3g95p5maf05.fil1.vcf > total_ALLPOP.DP3g95p5maf05.fil2.vcf
```

11. Apply a filter for HWE

Hardy Weinberg equilibrium is also another excellent filter to remove erroneous variant calls. To do this I will implement a script written by Chris Hollenbeck

```
curl -L -O https://github.com/jpuritz/dDocent/raw/master/scripts/filter_hwe_by_pop.pl
chmod +x filter_hwe_by_pop.pl
```
We can first filter by population specific HWE. To do this we need to convert our variant calls to SNPS using vcflib. The following command will do that for us.

```
vcfallelicprimitives total_ALLPOP.DP3g95p5maf05.fil2.vcf --keep-info --keep-geno > SNP.total_ALLPOP.DP3g95p5maf05.fil2.prim.vcf
```

Next, the command below will split the variant calls into SNP and indel genotypes.
```
vcftools --vcf SNP.total_ALLPOP.DP3g95p5maf05.fil2.prim.vcf --remove-indels --recode --recode-INFO-all --out SNP.DP3g95p5maf05
```

Now we can apply a SNP filter. We will choose to use the default Hardy Weinberg p-value of 0.001.

```
./filter_hwe_by_pop.pl -v SNP.DP3g95p5maf05.recode.vcf -p popmap_final_TD -o SNP.DP3g95p5maf05.HWE -h 0.001
```

We now have our final filtered SNP calls that we are confident about!

# STEP 12: Analyses to characterize neutral genomic variations

1. Calculate the total number of variants and the number of variants within each population

We can do this by using vcf-annotate with --fill-type
```
zcat SNP.DP3g95p5maf05.recode.vcf | vcf-annotate --fill-type | grep -oP "TYPE=\w+" | sort | uniq -c > VCF_filltype

grep "snp" VCF_filltype > SNP_VCF_filltype
```

To calculate the number of unique variants we can use vcf-contrast from VCFTools. This argument is useful for looking at differences between groups of samples.
```
# the -n option will only print novel alleles
#the sort option will sort the  sites by the confidence of the site being different from the child (-k5,5nr)
vcf-contrast -n +Child -Mother,Father -d 10 -f | vcf-query -f '%CHROM %POS\t%INFO/NOVELTY\t%INFO/NOVELAL\t%INFO/NOVELGT[\t%SAMPLE %GTR %PL]\n' | sort -k3,3nr | head

```

2. Calculating allele frequencies and the percentage of exclusive variants

2a. Calculate allele frequency
```
# To get the frequency of each allele over all individuals in a VCF file, you can use the -freq argument
vcftools --vcf SNP.DP3g95p5maf05.recode.vcf --freq --out allele_freq_all

# To calculate for individual populations

array3=($(ls *.keep | sed 's'/.keep//')
for i in ${array3[@]}; do
  vcftools --vcf SNP.DP3g95p5maf05.recode.vcf--freq --keep ${i}.keep --out ${i}.allele_freq
done

```
2b. Exclusive variants are defined as those that are polymorphic in only one population.
We will do this using the vcftools module vcf-compare

```
#compare the vcf files using the -g option to also output summary stats
vcf-compare -H -g A.vcf.gz B.vcf.gz C.vcf.gz
```

3. Calculate the level of nucleotide diversity using VCFTools

-3a: Calculate for each population separately
In order to reduce the computational intensity the sliding window has been set to 10,000.
```
array3=($(ls *.keep | sed 's'/.keep//')
for i in ${array3[@]}; do
  vcftools --vcf SNP.DP3g95p5maf05.recode.vcf  --keep ${i}.keep --window-pi 100000 --out = ${i.ND}
done
```

-3b: Use R to calculate a mean pi for all individuals

```
install.packages("fields")
library(fields)
binstats <- stats.bin(dat$POS,dat$PI,N=100)
matplot( binstats$centers, t(binstats$stats[ c("mean", "median","Q1", "Q3"),]), type="l",lty=c(1,2,2,2), col=c('red','blue','green','purple'), ylab="Pi diversity")
```

4. Calculate pairwise linkage disequilibrium in VCFTools across populations

The following code will calculate the pairwise linkage disequilibrium for each population by calling the argument `--hap-r2`.
I will use the argument --weir-fst-pop followed by a file listing the individuals in each population to compare all nine populations. In ordr to reduce the computational intensity the sliding window has been set to only compare sites within 50,000 base pairs of one another. We will also set the minimum R-squared value to be 0.001.

```
vcftools --vcf SNP.DP3g95p5maf05.recode.vcf --hap-r2 --ld-window-bp 500000 --out ld_window_50000 --min-r2 0.001
```

# STEP 13: Calculate the Fst across different populations

Now we will calculate the Fst statistic between individuals of different populations to get a measure of population differentiation.
```
vcftools --vcf SNP.DP3g95p5maf05.recode.vcf --weir-fst-pop CL.txt --weir-fst-pop CLP.txt --weir-fst-pop CS.txt --weir-fst-pop HC.txt --weir-fst-pop HC_VA.txt --weir-fst-pop HI.txt --weir-fst-pop LM.txt --weir-fst-pop SL.txt --weir-fst-pop SM.txt --out Fst_all_pop


```

# STEP 14: Assess genetic structure by using a PCA through the package adegenet

To carry out the code below, we need to first create a "strata" file that has three columns. The first column is the name of the individual, the second is the population, and the third is the library. We have the first two columns already in our popmap_final_TD file (though with no headings).

We can add on the library type (libraryA) with the following commands

```
#create file with repeated word with same number of lines as popmap file
printf 'LibA\n%.0s' {1..54}

#paste the two together
paste popmap_final_TD libfile > strata

```
Now we can add plot our data using adegenet in R. 

```
library(adegenet)
library(vcfR)
library(hierfstat)
library(ape)

#loading in the vcf file
oyster_vcf <- read.vcfR("SNP.DP3g95p5maf05.recode.vcf")

# the genind object store allelic data for individuals as integer allele counts
oyster_genind <- vcfR2genind(oyster_vcf)
strata<- read.table("strata", header=TRUE)
strata_df <- data.frame(strata)
strata(oyster_genind) <- strata_df

setPop(oyster_genind) <- ~Population

#Test Population Structure
fstat(oyster_genind)

oyster.pairwiseFst <- pairwise.fst(oyster_genind, res.type="matrix")

#We can use these genetic distance values to calculate a tree using ape
oyster.tree <- nj(oyster.pairwiseFst)
plot(oyster.tree, type="unr", tip.col=funky(nPop(oyster_genind)), font=2)
annot <- round(oyster.tree$edge.length,2)
edgelabels(annot[annot>0], which(annot>0), frame="n")
add.scale.bar()

```


# STEP 15: Use PCAdapt to visualize sample clustering my population location

We will now use PCAdapt to plot clustering of populations in R.

```
R
library(pcadapt)
variants <- read.pcadapt("SNP.DP3g95p5maf05.recode.vcf", type = "vcf")

#In this first step pick a minimum number of possible PCs, we'll go high with 20
PCs <- pcadapt(input = filename, K = 20)

#Now we will plot the percentage of variance explained by each PC using a screeplot
plot(PCs, option = "screeplot")

#plot for the fist ten
plot(PCs, option = "screeplot", K = 10)

# Create list with population designations
poplist.names <- c(rep("CL", 20),rep("CLP", 20),rep("CS", 20), rep("HC,20)),
rep("HC_VA", 20), rep("HI", 20), rep("LM", 20), rep("SL", 20), rep("SM", 20))

#Display individual scores on each of the PCs and produce a score plot
plot(PCs, option = "scores", pop = poplist.names)
#try 2 and 3
plot(PCs, option = "scores", i = 2, j = 3, pop = poplist.names)
#try 3 and 4
plot(PCs, option = "scores", i = 2, j = 3, pop = poplist.names)

# redo with appropriate number of PCs
PC2<- pcadapt(variants, K=3)

#output the summary statistics
summary(PC2)

#putatively investigate outliers with a Manhattan plot
plot(PC2, option="manhattan")

```

# Works used for reference:
### References
Benjelloun, Badr, et al. "Characterizing neutral genomic diversity and selection signatures in indigenous populations of Moroccan goats (Capra hircus) using WGS data." Frontiers in genetics 6 (2015): 107.
Gómez-Chiarri, M., W. C. Warren, X. Guo, and D. Proestou. 2015. Developing tools for the study of molluscan immunity: The sequencing of the genome of the eastern oyster, Crassostrea virginica. Fish Shellfish Immunol. 46:2–4.

http://clavius.bc.edu/~erik/CSHL-advanced-sequencing/freebayes-tutorial.html
https://github.com/ekg/alignment-and-variant-calling-tutorial
https://hbctraining.github.io/In-depth-NGS-Data-Analysis-Course/sessionVI/lessons/02_variant-calling.html
https://ucdavis-bioinformatics-training.github.io/2017-August-Variant-Analysis-Workshop/wednesday/variant_calling.html
http://ddocent.com/filtering/
http://angus.readthedocs.io/en/2016/pop_gen_tutorial.html
https://github.com/alexharkess
http://www.mountainmanmaier.com/software/pop_genom/#search-for-outliers-with-pcadapt
https://vcftools.github.io/documentation.html
http://vcftools.sourceforge.net/perl_module.html#vcf-isec
http://adegenet.r-forge.r-project.org/files/PRstats/practical-MVAintro.1.0.pdf

