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

|Name	    |Run Type	  |Library Source	|Library Type	      |Adaptor	|Read # 	|Number of Bases	|Average Quality 	|Average Quality |	Percent Duplicate|
|---------|-----------|---------------|-------------------|--------------------------------------------|---------------|---------------|
|CS-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34226714	|9515026492	      |38	|38|	5.929|
|CS-2	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36064101	|10891358502	    |37	|37|	6.62|
|CS-2	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|29122012	|8095919336	      |37	|37|	5.535|
|CS-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34267784	|10348870768	    |38	|38|	6.786|
|CS-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|29876081	|8305550518	      |38	|38|	5.696|
|CS-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|37958616	|11463502032	    |38	|38|	6.66|
|CS-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|30041328	|8351489184	      |38	|38|	5.521|
|CS-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|32002481	|9664749262	      |37	|37|	7.269|
|CS-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34888554	|10536343308	    |38	|38|	6.659|
|CS-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|32783702	|9113869156	      |38	|38|	5.613|
|HC-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|38646818	|11671339036	    |38	|38|	8.318|
|HC-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|38646818	|11671339036	    |38	|38|	8.318|
|HC-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31556239	|9529984178	      |38	|38|	7.612|
|HC-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31556239	|9529984178	      |38	|38|	7.612|
|HC-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39877222	|12042921044	|38	|38|	7.606|
|HC-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39877222	|12042921044	|38	|38|	7.606|
|HC-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|45016816	|13595078432	|37	|37|	7.035|
|HC-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36535596	|10156895688	|38	|38|	5.065|
|HC-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|45016816	|13595078432	|37	|37|	7.035|
|HC-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36535596	|10156895688	|38	|38|	5.065|
|HC-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|28024130	|8463287260	|38	|38|	6.819|
|HC-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|28024130	|8463287260	|38	|38|	6.819|
|HC-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|77299611	|23344482522	|37	|37|	7.158|
|HC-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|50348381	|13996849918	|37	|37|	5.841|
|HC-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|77299611	|23344482522	|37	|37|	7.158|
|HC-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|50348381	|13996849918	|37	|37|	5.841|
|HC-VA-1	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42970224	|12977007648	|37	|37|	7.839|
|HC-VA-1	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36814199	|10234347322	|37	|37|	6.051|
|HC-VA-1	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42970224	|12977007648	|37	|37|	7.839|
|HC-VA-1	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36814199	|10234347322	|37	|37|	6.051|
|HC-VA-2	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|41451075	|12518224650	|37	|37|	7.733|
|HC-VA-2	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35187075	|9782006850	|37	|37|	6.042|
|HC-VA-2	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|41451075	|12518224650	|37	|37|	7.733|
|HC-VA-2	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35187075	|9782006850	|37	|37|	6.042|
|HC-VA-3	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31945464	|9647530128	|37	|37|	5.78|
|HC-VA-3	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31604568	|8786069904	|38	|38|	4.807|
|HC-VA-3	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31945464	|9647530128	|37	|37|	5.78|
|HC-VA-3	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31604568	|8786069904	|38	|38|	4.807|
|HC-VA-4	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34803290	|10510593580	|38	|38|	6.292|
|HC-VA-4	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|32573378	|9055399084	|38	|38|	5.213|
|HC-VA-4	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|34803290	|10510593580	|38	|38|	6.292|
|HC-VA-4	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|32573378	|9055399084	|38	|38|	5.213|
|HC-VA-5	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39877905	|12043127310	|38	|38|	7.672|
|HC-VA-5	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31515900	|8761420200	|38	|38|	5.973|
|HC-VA-5	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39877905	|12043127310	|38	|38|	7.672|
|HC-VA-5	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31515900	|8761420200	|38	|38|	5.973|
|HC-VA-6	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42747638	|12909786676	|37	|37|	8.127|
|HC-VA-6	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35426923	|9848684594	|37	|37|	6.284|
|HC-VA-6	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42747638	|12909786676	|37	|37|	8.127|
|HC-VA-6	|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35426923	|9848684594	|37	|37|	6.284|
|HI-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39293670	|11866688340	|38	|38|	7.201|
|HI-2	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|59177432	|17871584464	|38	|38|	8.012|
|HI-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|42116311	|12719125922	|38	|38|	7.662|
|HI-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|38708892	|11690085384	|38	|38|	7.583|
|HI-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|52019244	|15709811688	|38	|38|	7.675|
|HI-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39366994	|11888832188	|38	|38|	7.289|
|LM-1_pool|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|33484657	|10112366414	|37	|37|	8.285|
|LM-1_pool|PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|29307831	|8147577018	|37	|37|	6.53|
|LM-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|46243120	|13965422240	|37	|37|	6.294|
|LM-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|40743407	|11326667146	|38	|38|	5.121|
|LM-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|86188161	|26028824622	|37	|37|	6.666|
|LM-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|72516832	|20159679296	|38	|38|	5.517|
|LM-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|37559493	|11342966886	|38	|38|	6.095|
|LM-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|39108440	|10872146320	|38	|38|	5.058|
|LM-8	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|33186635	|10022363770	|38	|38|	5.956|
|LM-8	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|36375900	|10112500200	|38	|38|	4.925|
|SL-1	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|44573789	|13461284278	|38	|38|	6.735|
|SL-2	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|29619024	|8944945248	|38	|38|	6.44|
|SL-3	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|46847209	|14147857118	|38	|38|	7.176|
|SL-4	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|30848151	|9316141602	|38	|38|	6.614|
|SL-5	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|49922036	|15076454872	|38	|38|	7.224|
|SL-6	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|38193328	|11534385056	|38	|38|	6.76|
|SM-10	  |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|41831639	|12633154978	|38	|38|	7.644|
|SM-11	  |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|31690949	|9570666598	|38	|38|	6.868|
|SM-12	  |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35796533	|10810552966	|38	|38|	7.461|
|SM-7	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|47538272	|14356558144	|38	|38|	8.639|
|SM-8	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35781255	|10805939010	|38	|38|	7.666|
|SM-9	    |PAIRED_END	|gDNA	          |Shotgun (PCR free)	|LuciGen	|35628014	|10759660228	|38	|38|	6.895|

#### Step 1: Download and acquire the Data

All sequence data has been downloaded onto KITT by JP. To access the data a symbolic link will be created using the following commands.

```
ln -s /home/Shared_Data/*.F.fq.gz .
ln -s /home/Shared_Data/*.R.fq.gz .
ln -s /home/Shared_Data/short_lib/*.F.fq.gz .
ln -s /home/Shared_Data/short_lib/*.R.fq.gz .

```

# Data will be re-downloaded to update those "short lib sequences" which were the following:  

/home/Shared_Data/short_lib/CLP_1.F.fq.gz
/home/Shared_Data/short_lib/CLP_2.F.fq.gz
/home/Shared_Data/short_lib/CLP_3.F.fq.gz
/home/Shared_Data/short_lib/CLP_4.F.fq.gz
/home/Shared_Data/short_lib/CLP_5.F.fq.gz
/home/Shared_Data/short_lib/CLP_6.F.fq.gz
/home/Shared_Data/short_lib/CS_1.F.fq.gz
/home/Shared_Data/short_lib/CS_2.F.fq.gz
/home/Shared_Data/short_lib/CS_3.F.fq.gz
/home/Shared_Data/short_lib/CS_5.F.fq.gz
/home/Shared_Data/short_lib/CS_7.F.fq.gz
/home/Shared_Data/short_lib/HC_5.F.fq.gz
/home/Shared_Data/short_lib/HC_7.F.fq.gz
/home/Shared_Data/short_lib/HC_VA_1.F.fq.gz
/home/Shared_Data/short_lib/HC_VA_2.F.fq.gz
/home/Shared_Data/short_lib/HC_VA_3.F.fq.gz
/home/Shared_Data/short_lib/HC_VA_4.F.fq.gz
/home/Shared_Data/short_lib/HC_VA_5.F.fq.gz
/home/Shared_Data/short_lib/HC_VA_6.F.fq.gz
/home/Shared_Data/short_lib/LM_1_pool.F.fq.gz
/home/Shared_Data/short_lib/LM_3.F.fq.gz
/home/Shared_Data/short_lib/LM_4.F.fq.gz
/home/Shared_Data/short_lib/LM_7.F.fq.gz
/home/Shared_Data/short_lib/LM_8.F.fq.gz



#### Step 2: Check Sum of Genome Quebec Data
Use wget command supplied by GenomeQuebec to  automatically download all data, generate checksum file, and perform checksum.

```
wget -O - "https://genomequebec.mcgill.ca/nanuqMPS/readsetList?projectId=15565&tech=HiSeq" --no-cookies --no-check-certificate --post-data 'j_username=username&j_password=password' | wget --no-cookies --no-check-certificate --post-data 'j_username=username&j_password=password' -ci -
```


#### Step 3: Initial Raw Data Assessment and Characterization
1. Read counts
- Read counts are provided in metadata file and checked using checksum.

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
conda create -n EMR_Final_Assigment fastqc

# Activate the environment
source activate EMR_Final_Assignment

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

#Check that all files have been completed by comparing arrays with bash
declare -a total_array=(./LM*.F.fq.gz ./HC_?.F.fq.gz ./CS*.F.fq.gz ./SM*.F.fq.gz ./HI*.F.fq.gz ./SL*.F.fq.gz ./CL_*.F.fq.gz ./CLP*.F.fq.gz ./HC_VA*.F.fq.gz ./LM*.R.fq.gz ./HC_?.R.fq.gz ./CS*.R.fq.gz ./SM*.R.fq.gz ./HI*.R.fq.gz ./SL*.R.fq.gz ./CL_*.R.fq.gz ./CLP*.R.fq.gz ./HC_VA*.R.fq.gz)
declare -a html_array=(./*.html)
echo ${total_array[@]} ${html_array[@]} | tr ' ' '\n' | sort | uniq -u

# Put process into the background using
^Z
bg
disown -a

# use MultiQC to put together all Files
#make new folder with all Fastqc files
mkdir fastqc_results
cd fastqc_results
conda install -c bioconda multiqc

multiqc .
# Export file to folder so you can open it up with .html

```

Overall the summary statistics indicate _________.


#### Step 4: Bioinformatic Processing

1. Adaptor trimming 




2. Read trimming for quality 



3. Read Mapping to Reference using BWA memory






