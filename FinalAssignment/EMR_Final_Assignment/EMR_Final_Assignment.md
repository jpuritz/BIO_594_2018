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

| Name      | Run Type   |  Library Source	| Library Type	      | Adaptor |	Number of Reads |	Number of Bases	| Average Quality |	% Duplicate |
|-----------|------------|------------------|---------------------|---------|-----------------|-----------------|-----------------|-------------|
| CL-1      | PAIRED_END |  gDNA            | 	Shotgun (PCR free)|	LuciGen	| 30,878,164      |	9325205528.00	  | 38              |	6.708       |
| CL-3	    | PAIRED_END |  gDNA            |   Shotgun (PCR free)|	LuciGen	| 48,204,914      |	14557884028.00	| 38	            | 7.365       |
| CL-4	    | PAIRED_END |  gDNA            | 	Shotgun (PCR free)|	LuciGen	|	28,692,872      |	8665247344.00   | 38	            | 6.788       |   
| CL-5	    | PAIRED_END |  gDNA            | 	Shotgun (PCR free)|	LuciGen	|	25,912,588      |	7825601576.00   | 37	            | 6.623       |
| CL-6	    | PAIRED_END |  gDNA            | 	Shotgun (PCR free)|	LuciGen	|	33,328,299      |	10065146298.00	| 38	            | 6.39        |
| CLP-1	    | PAIRED_END |  gDNA            | 	Shotgun (PCR free)|	LuciGen	|	30,660,758      |	8523690724.00	  | 37	            | 4.581       |
| CLP-2	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	33,352,682      |	9272045596.00	  | 38	            | 4.918       |
| CLP-3	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	43,855,756      |	12191900168.00	| 37	            |	4.894       |
| CLP-4	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	34,783,163      |	9669719314.00	  | 37	            |	5.323       |
| CLP-5	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	37,871,333      |	10528230574.00	| 38	            |	5.002       |
| CLP-6	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	36,786,280      |	10226585840.00	| 37	            |	6.199       |
| CS-1	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	34,226,714      |	9515026492.00	  | 38	            |	5.929       |
| CS-2	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	29,122,012      |	8095919336.00	  | 37	            |	5.535       |
| CS-3	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	29,876,081      |	8305550518.00	  | 38	            |	5.696       |
| CS-5	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	30,041,328      |	8351489184.00	  | 38	            |	5.521       |
| CS-6	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	32,002,481      |	9664749262.00	  | 37	            |	7.269       |
| CS-7	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	32,783,702      |	9113869156.00	  | 38	            |	5.613       |
| HC-1	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	38,646,818      |	11671339036.00	| 38	            |	8.318       |
| HC-3	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	31,556,239      |	9529984178.00	  | 38	            |	7.612       |
| HC-4	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	39,877,222      |	12042921044.00  |	38	            |	7.606       |
| HC-5	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	36,535,596      |	10156895688.00	| 38	            |	5.065       |
| HC-6	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	28,024,130      |	8463287260.00	  | 38	            |	6.819       |
| HC-7	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	50,348,381      |	13996849918.00	| 37	            |	5.841       |
| HC-VA-1	  | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	36,814,199      |	10234347322.00	| 37	            |	6.051       |
| HC-VA-2	  | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	35,187,075      |	9782006850.00	  | 37	            |	6.042       |
| HC-VA-3	  | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	31,604,568      |	8786069904.00	  | 38	            |	4.807       |
| HC-VA-4	  | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	31,515,900      |	8761420200.00	  | 38	            |	5.973       |
| HC-VA-6	  | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	35,426,923      |	9848684594.00   |	37	            |	6.284       |
| HI-1	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	39,293,670      |	11866688340.00	| 38	            |	7.201       |
| HI-2	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	59,177,432      |	17871584464.00	| 38	            |	8.012       |
| HI-3	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	42,116,311      |	12719125922.00	| 38	            |	7.662       |
| HI-4	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	38,708,892      |	11690085384.00	| 38	            |	7.583       |
| HI-5	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	52,019,244      |	15709811688.00	| 38	            |	7.675       |
| HI-6	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	39,366,994      |	11888832188.00	| 38	            |	7.289       |
| LM-1_pool	| PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	29,307,831      |	8147577018.00	  | 37	            |	6.53        |
| LM-3	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	40,743,407      |	11326667146.00	| 38	            |	5.121       |
| LM-4	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	72,516,832      |	20159679296.00	| 38	            |	5.517       |
| LM-7	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	39,108,440      |	10872146320.00	| 38	            |	5.058       |
| LM-8	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	36,375,900      |	10112500200.00	| 38	            |	4.925       |
| SL-1	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	44,573,789      |	13461284278.00	| 38	            |	6.735       |
| SL-2	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	29,619,024      |	8944945248.00	  | 38	            |	6.44        |
| SL-3	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	46,847,209      |	14147857118.00	| 38	            |	7.176       |
| SL-4	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	30,848,151      |	9316141602.00	  | 38	            |	6.614       |
| SL-5	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	49,922,036      |	15076454872.00	| 38	            |	7.224       |
| SL-6	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	38,193,328      |	11534385056.00	| 38	            |	6.76        |
| SM-10	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	41,831,639      |	12633154978.00	| 38	            |	7.644       |
| SM-11	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	31,690,949      |	9570666598.00	  | 38	            |	6.868       |
| SM-12	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	35,796,533      |	10810552966.00	| 38	            |	7.461       |
| SM-7	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	47,538,272      |	14356558144.00	| 38	            |	8.639       |
| SM-8	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	35,781,255      |	10805939010.00	| 38	            |	7.666       |
| SM-9	    | PAIRED_END | 	gDNA            | 	Shotgun (PCR free)|	LuciGen	|	35,628,014      |	10759660228.00	| 38	            |	6.895       |

#### Step 1: Download and acquire the Data

All sequence data has been downloaded onto KITT by JP. To access the data a symbolic link will be created using the following commands.

```
ln -s /home/Shared_Data/*.F.fq.gz .
ln -s /home/Shared_Data/*.R.fq.gz .
ln -s /home/Shared_Data/short_lib/*.F.fq.gz .
ln -s /home/Shared_Data/short_lib/*.R.fq.gz .

```

#### Step 2: Check sum of Genome Quebec Data
Use wget command supplied by GenomeQuebec to  automatically download all data, generate checksum file, and perform checksum

```
wget -O - "https://genomequebec.mcgill.ca/nanuqMPS/readsetList?projectId=15565&tech=HiSeq" --no-cookies --no-check-certificate --post-data 'j_username=username&j_password=password' | wget --no-cookies --no-check-certificate --post-data 'j_username=username&j_password=password' -ci -
```


#### Step 3:
1. Read counts
-
2. Read quality

