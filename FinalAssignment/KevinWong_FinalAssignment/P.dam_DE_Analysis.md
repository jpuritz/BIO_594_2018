# *P. damicornis* TGA transcriptome analysis
Author: Kevin Wong  
Last updated: May 7, 2018

Data uploaded and analyzed on KITT (made by J. Puritz)

### Uploading raw data to KITT
```
scp -r -P 2292 /Volumes/NGS_DATA/Hawaii_Pdam/Pdam_Summer_2011/Pdam_2011_Raw/ kwong@kitt.uri.edu:/home/kwong/Final_Project/raw
```

### Uploading reference P.dam transcriptome to KITT
```
scp -P 2292 P_damicornis_transcriptome_Seneca2015.fasta kwong@kitt.uri.edu:Final_Project/raw
```

### Getting all files into one directory
```
cd raw
mkdir allraw
cd Pdam_2011_Raw/
grep -rl --null --include '*.fastq.gz' . | xargs -0r cp -t ../allraw
```

### Checking the files downloaded correctly (cksum)
```
scp -P 2292 Hawaii_Pacuta_checksum.md5 kwong@kitt.uri.edu:Final_Project/raw/allraw
md5sum *.fastq.gz > Hawaii_Pacuta_checksum2.md5
cksum Hawaii_Pacuta_checksum.md5 Hawaii_Pacuta_checksum2.md5
```

49167847 **4879** Hawaii_Pacuta_checksum.md5  
485158896 **4880** Hawaii_Pacuta_checksum2.md5 #slightly off

```
md5sum -c Hawaii_Pacuta_checksum2.md5

```
1026_CGATGT_L003_R1_001.fastq.gz: OK  
1026_CGATGT_L003_R1_002.fastq.gz: OK  
1026_CGATGT_L003_R2_001.fastq.gz: OK  
1026_CGATGT_L003_R2_002.fastq.gz: OK  
1028_TGACCA_L003_R1_001.fastq.gz: OK  
1028_TGACCA_L003_R1_002.fastq.gz: OK  
1028_TGACCA_L003_R2_001.fastq.gz: OK  
1028_TGACCA_L003_R2_002.fastq.gz: OK  
1030_ACAGTG_L003_R1_001.fastq.gz: OK  
1030_ACAGTG_L003_R2_001.fastq.gz: OK  
1032_GCCAAT_L003_R1_001.fastq.gz: OK  
1032_GCCAAT_L003_R2_001.fastq.gz: OK  
1034_CAGATC_L003_R1_001.fastq.gz: OK  
1034_CAGATC_L003_R2_001.fastq.gz: OK  
1036_CTTGTA_L003_R1_001.fastq.gz: OK  
1036_CTTGTA_L003_R1_002.fastq.gz: OK  
1036_CTTGTA_L003_R2_001.fastq.gz: OK  
1036_CTTGTA_L003_R2_002.fastq.gz: OK  
1038_AGTCAA_L003_R1_001.fastq.gz: OK  
1038_AGTCAA_L003_R1_002.fastq.gz: OK  
1038_AGTCAA_L003_R2_001.fastq.gz: OK  
1038_AGTCAA_L003_R2_002.fastq.gz: OK  
1040_AGTTCC_L003_R1_001.fastq.gz: OK  
1040_AGTTCC_L003_R1_002.fastq.gz: OK  
1040_AGTTCC_L003_R2_001.fastq.gz: OK  
1040_AGTTCC_L003_R2_002.fastq.gz: OK  
1042_ATGTCA_L003_R1_001.fastq.gz: OK  
1042_ATGTCA_L003_R2_001.fastq.gz: OK  
1044_CCGTCC_L003_R1_001.fastq.gz: OK  
1044_CCGTCC_L003_R2_001.fastq.gz: OK  
H10_CCGTCC_L003_R1_001.fastq.gz: OK  
H10_CCGTCC_L003_R1_002.fastq.gz: OK  
H10_CCGTCC_L003_R2_001.fastq.gz: OK  
H10_CCGTCC_L003_R2_002.fastq.gz: OK  
H11_GTCCGC_L003_R1_001.fastq.gz: OK  
H11_GTCCGC_L003_R1_002.fastq.gz: OK  
H11_GTCCGC_L003_R2_001.fastq.gz: OK  
H11_GTCCGC_L003_R2_002.fastq.gz: OK  
H12_GTGAAA_L003_R1_001.fastq.gz: OK  
H12_GTGAAA_L003_R2_001.fastq.gz: OK  
H1_CGATGT_L003_R1_001.fastq.gz: OK  
H1_CGATGT_L003_R1_002.fastq.gz: OK  
H1_CGATGT_L003_R2_001.fastq.gz: OK  
H1_CGATGT_L003_R2_002.fastq.gz: OK  
H2_TGACCA_L003_R1_001.fastq.gz: OK  
H2_TGACCA_L003_R1_002.fastq.gz: OK  
H2_TGACCA_L003_R2_001.fastq.gz: OK  
H2_TGACCA_L003_R2_002.fastq.gz: OK  
H3_ACAGTG_L003_R1_001.fastq.gz: OK  
H3_ACAGTG_L003_R1_002.fastq.gz: OK  
H3_ACAGTG_L003_R2_001.fastq.gz: OK  
H3_ACAGTG_L003_R2_002.fastq.gz: OK  
H4_GCCAAT_L003_R1_001.fastq.gz: OK  
H4_GCCAAT_L003_R1_002.fastq.gz: OK  
H4_GCCAAT_L003_R2_001.fastq.gz: OK  
H4_GCCAAT_L003_R2_002.fastq.gz: OK  
H5_CAGATC_L003_R1_001.fastq.gz: OK  
H5_CAGATC_L003_R1_002.fastq.gz: OK  
H5_CAGATC_L003_R2_001.fastq.gz: OK  
H5_CAGATC_L003_R2_002.fastq.gz: OK  
H6_CTTGTA_L003_R1_001.fastq.gz: OK  
H6_CTTGTA_L003_R1_002.fastq.gz: OK  
H6_CTTGTA_L003_R2_001.fastq.gz: OK  
H6_CTTGTA_L003_R2_002.fastq.gz: OK  
H7_AGTCAA_L003_R1_001.fastq.gz: OK  
H7_AGTCAA_L003_R1_002.fastq.gz: OK  
H7_AGTCAA_L003_R2_001.fastq.gz: OK  
H7_AGTCAA_L003_R2_002.fastq.gz: OK  
H8_AGTTCC_L003_R1_001.fastq.gz: OK  
H8_AGTTCC_L003_R2_001.fastq.gz: OK  
H9_ATGTCA_L003_R1_001.fastq.gz: OK  
H9_ATGTCA_L003_R1_002.fastq.gz: OK  
H9_ATGTCA_L003_R2_001.fastq.gz: OK  
H9_ATGTCA_L003_R2_002.fastq.gz: OK  

```
md5sum -c Hawaii_Pacuta_checksum.md5
```
1026_CGATGT_L003_R1_001.fastq.gz: OK  
1026_CGATGT_L003_R1_002.fastq.gz: OK  
1026_CGATGT_L003_R2_001.fastq.gz: OK  
1026_CGATGT_L003_R2_002.fastq.gz: OK  
1028_TGACCA_L003_R1_001.fastq.gz: OK  
1028_TGACCA_L003_R1_002.fastq.gz: OK  
1028_TGACCA_L003_R2_001.fastq.gz: OK  
1028_TGACCA_L003_R2_002.fastq.gz: OK  
1030_ACAGTG_L003_R1_001.fastq.gz: OK  
1030_ACAGTG_L003_R2_001.fastq.gz: OK  
1032_GCCAAT_L003_R1_001.fastq.gz: OK  
1032_GCCAAT_L003_R2_001.fastq.gz: OK  
1034_CAGATC_L003_R1_001.fastq.gz: OK  
1034_CAGATC_L003_R2_001.fastq.gz: OK  
1036_CTTGTA_L003_R1_001.fastq.gz: OK  
1036_CTTGTA_L003_R1_002.fastq.gz: OK  
1036_CTTGTA_L003_R2_001.fastq.gz: OK  
1036_CTTGTA_L003_R2_002.fastq.gz: OK  
1038_AGTCAA_L003_R1_001.fastq.gz: OK  
1038_AGTCAA_L003_R1_002.fastq.gz: OK  
1038_AGTCAA_L003_R2_001.fastq.gz: OK  
1038_AGTCAA_L003_R2_002.fastq.gz: OK  
1040_AGTTCC_L003_R1_001.fastq.gz: OK  
1040_AGTTCC_L003_R1_002.fastq.gz: OK  
1040_AGTTCC_L003_R2_001.fastq.gz: OK  
1040_AGTTCC_L003_R2_002.fastq.gz: OK  
1042_ATGTCA_L003_R1_001.fastq.gz: OK  
1042_ATGTCA_L003_R2_001.fastq.gz: OK  
1044_CCGTCC_L003_R1_001.fastq.gz: OK  
1044_CCGTCC_L003_R2_001.fastq.gz: OK  
H1_CGATGT_L003_R1_001.fastq.gz: OK  
H1_CGATGT_L003_R1_002.fastq.gz: OK  
H1_CGATGT_L003_R2_001.fastq.gz: OK  
H1_CGATGT_L003_R2_002.fastq.gz: OK  
H2_TGACCA_L003_R1_001.fastq.gz: OK  
H2_TGACCA_L003_R1_002.fastq.gz: OK  
H2_TGACCA_L003_R2_001.fastq.gz: OK  
H2_TGACCA_L003_R2_002.fastq.gz: OK  
H3_ACAGTG_L003_R1_001.fastq.gz: OK  
H3_ACAGTG_L003_R1_002.fastq.gz: OK  
H3_ACAGTG_L003_R2_001.fastq.gz: OK  
H3_ACAGTG_L003_R2_002.fastq.gz: OK  
H4_GCCAAT_L003_R1_001.fastq.gz: OK  
H4_GCCAAT_L003_R1_002.fastq.gz: OK  
H4_GCCAAT_L003_R2_001.fastq.gz: OK  
H4_GCCAAT_L003_R2_002.fastq.gz: OK  
H5_CAGATC_L003_R1_001.fastq.gz: OK  
H5_CAGATC_L003_R1_002.fastq.gz: OK  
H5_CAGATC_L003_R2_001.fastq.gz: OK  
H5_CAGATC_L003_R2_002.fastq.gz: OK  
H6_CTTGTA_L003_R1_001.fastq.gz: OK  
H6_CTTGTA_L003_R1_002.fastq.gz: OK  
H6_CTTGTA_L003_R2_001.fastq.gz: OK  
H6_CTTGTA_L003_R2_002.fastq.gz: OK  
H7_AGTCAA_L003_R1_001.fastq.gz: OK  
H7_AGTCAA_L003_R1_002.fastq.gz: OK  
H7_AGTCAA_L003_R2_001.fastq.gz: OK  
H7_AGTCAA_L003_R2_002.fastq.gz: OK  
H8_AGTTCC_L003_R1_001.fastq.gz: OK  
H8_AGTTCC_L003_R2_001.fastq.gz: OK  
H9_ATGTCA_L003_R1_001.fastq.gz: OK  
H9_ATGTCA_L003_R1_002.fastq.gz: OK  
H9_ATGTCA_L003_R2_001.fastq.gz: OK  
H9_ATGTCA_L003_R2_002.fastq.gz: OK  
H10_CCGTCC_L003_R1_001.fastq.gz: OK  
H10_CCGTCC_L003_R1_002.fastq.gz: OK  
H10_CCGTCC_L003_R2_001.fastq.gz: OK  
H10_CCGTCC_L003_R2_002.fastq.gz: OK  
H11_GTCCGC_L003_R1_001.fastq.gz: OK  
H11_GTCCGC_L003_R1_002.fastq.gz: OK  
H11_GTCCGC_L003_R2_001.fastq.gz: OK  
H11_GTCCGC_L003_R2_002.fastq.gz: OK  
H12_GTGAAA_L003_R1_001.fastq.gz: OK  
H12_GTGAAA_L003_R2_001.fastq.gz: OK  

The differences in checksums was most likely due to the differences in sample orders

### Concatenating extended files (find a better way to do this)
```
e.g.
cat 1026_CGATGT_L003_R1_001.fastq.gz 1026_CGATGT_L003_R1_002.fastq.gz > 1026_CGATGT_L003_R1_003.fastq.gz` #combining files that were split during sequencing
```
### Checking lengths of files to make sure they added correctly  
`wc -l 1026_CGATGT_L003_R1_001.fastq.gz`  
**1830499** 1026_CGATGT_L003_R1_001.fastq.gz  
`wc -l 1026_CGATGT_L003_R1_002.fastq.gz`  
**237763** 1026_CGATGT_L003_R1_002.fastq.gz  
`1026_CGATGT_L003_R1_003.fastq.gz`  
**2068262** 1026_CGATGT_L003_R1_003.fastq.gz  

It all adds up!

### Moving full reads to a different folder
```
mkdir fullreads
cp *3.fastq.gz fullreads/
cp 1030_ACAGTG_L003_R1_001.fastq.gz 1030_ACAGTG_L003_R2_001.fastq.gz 1032_GCCAAT_L003_R1_001.fastq.gz 1032_GCCAAT_L003_R2_001.fastq.gz 1034_CAGATC_L003_R1_001.fastq.gz 1034_CAGATC_L003_R2_001.fastq.gz 1042_ATGTCA_L003_R1_001.fastq.gz 1042_ATGTCA_L003_R2_001.fastq.gz 1044_CCGTCC_L003_R1_001.fastq.gz 1044_CCGTCC_L003_R2_001.fastq.gz H12_GTGAAA_L003_R1_001.fastq.gz H12_GTGAAA_L003_R2_001.fastq.gz H8_AGTTCC_L003_R1_001.fastq.gz H8_AGTTCC_L003_R2_001.fastq.gz fullreads/
```

### Count of raw reads

```
zgrep -c "@H" *.fastq.gz
```
1026_CGATGT_L003_R1_003.fastq.gz:4884127  
1026_CGATGT_L003_R2_003.fastq.gz:4754576  
1028_TGACCA_L003_R1_003.fastq.gz:5035517  
1028_TGACCA_L003_R2_003.fastq.gz:4902968  
1030_ACAGTG_L003_R1_001.fastq.gz:4193223  
1030_ACAGTG_L003_R2_001.fastq.gz:4084027  
1032_GCCAAT_L003_R1_001.fastq.gz:3897399  
1032_GCCAAT_L003_R2_001.fastq.gz:3790985  
1034_CAGATC_L003_R1_001.fastq.gz:3849003  
1034_CAGATC_L003_R2_001.fastq.gz:3748845  
1036_CTTGTA_L003_R1_003.fastq.gz:4623003  
1036_CTTGTA_L003_R2_003.fastq.gz:4499987  
1038_AGTCAA_L003_R1_003.fastq.gz:5102743  
1038_AGTCAA_L003_R2_003.fastq.gz:4965929  
1040_AGTTCC_L003_R1_003.fastq.gz:5975468  
1040_AGTTCC_L003_R2_003.fastq.gz:5816311  
1042_ATGTCA_L003_R1_001.fastq.gz:3709868  
1042_ATGTCA_L003_R2_001.fastq.gz:3609501  
1044_CCGTCC_L003_R1_001.fastq.gz:3270810  
1044_CCGTCC_L003_R2_001.fastq.gz:3177058  
H10_CCGTCC_L003_R1_003.fastq.gz:5580974  
H10_CCGTCC_L003_R2_003.fastq.gz:5487505  
H11_GTCCGC_L003_R1_003.fastq.gz:5013559  
H11_GTCCGC_L003_R2_003.fastq.gz:4927802  
H12_GTGAAA_L003_R1_001.fastq.gz:3788475  
H12_GTGAAA_L003_R2_001.fastq.gz:3727500  
H1_CGATGT_L003_R1_003.fastq.gz:5133333  
H1_CGATGT_L003_R2_003.fastq.gz:5056440  
H2_TGACCA_L003_R1_003.fastq.gz:5207771  
H2_TGACCA_L003_R2_003.fastq.gz:5127577  
H3_ACAGTG_L003_R1_003.fastq.gz:6927017  
H3_ACAGTG_L003_R2_003.fastq.gz:6821448  
H4_GCCAAT_L003_R1_003.fastq.gz:4458181  
H4_GCCAAT_L003_R2_003.fastq.gz:4389753  
H5_CAGATC_L003_R1_003.fastq.gz:4790041  
H5_CAGATC_L003_R2_003.fastq.gz:4717823  
H6_CTTGTA_L003_R1_003.fastq.gz:4687294  
H6_CTTGTA_L003_R2_003.fastq.gz:4616590  
H7_AGTCAA_L003_R1_003.fastq.gz:4725314  
H7_AGTCAA_L003_R2_003.fastq.gz:4654177  
H8_AGTTCC_L003_R1_001.fastq.gz:3417223  
H8_AGTTCC_L003_R2_001.fastq.gz:3364990  
H9_ATGTCA_L003_R1_003.fastq.gz:5118994  
H9_ATGTCA_L003_R2_003.fastq.gz:5044500  


### Quality control of raw sequencing reads (FASTQC)
https://github.com/s-andrews/FastQC
```
mkdir fastqc_results
cd fastqc_results
conda install -c bioconda fastqc
fastqc ../*fastq.gz .
mv *fastqc.* fastqc_results/
```

### Using Multiqc to summarize FastQC results
https://github.com/ewels/MultiQC
```
pip install multiqc
conda install -c bioconda multiqc
multiqc .
scp -P 2292 kwong@kitt.uri.edu:/home/kwong/Final_Project/raw/allraw/fullreads/fastqc_results/multiqc_report.html /Users/kevinwong/Documents/Projects/P.damicornis_Transcriptome_Analysis/Output/

```

### Trimming and cleaning reads

https://github.com/ExpressionAnalysis/ea-utils/blob/wiki/FastqMcf.md

```
mkdir cleaned_reads
cd cleaned_reads
conda install -c bioconda ea-utils
```

```
sh -c 'for file in "1026_CGATGT_L003" "1028_TGACCA_L003" "1030_ACAGTG_L003" "1032_GCCAAT_L003" "1034_CAGATC_L003" "1036_CTTGTA_L003" "1038_AGTCAA_L003" "1040_AGTTCC_L003" "1042_ATGTCA_L003" "1044_CCGTCC_L003" "H10_CCGTCC_L003" "H11_GTCCGC_L003" "H12_GTGAAA_L003" "H1_CGATGT_L003" "H2_TGACCA_L003" "H3_ACAGTG_L003" "H4_GCCAAT_L003" "H5_CAGATC_L003" "H6_CTTGTA_L003" "H7_AGTCAA_L003" "H8_AGTTCC_L003" "H9_ATGTCA_L003"
do
/home/kwong/miniconda3/bin/fastq-mcf \
/home/kwong/Final_Project/raw/allraw/fullreads/adapters.fa \
/home/kwong/Final_Project/raw/allraw/fullreads/${file}_R1_00?.fastq.gz \
/home/kwong/Final_Project/raw/allraw/fullreads/${file}_R2_00?.fastq.gz \
-l 100 \
-q 20 \
-w 5 \
-x 10 \
-u \
-P 33 \
-o /home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads/${file}_R1_cleaned.fastq.gz \
-o /home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads/${file}_R2_cleaned.fastq.gz &> /home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads/${file}.log
done'
```

### Count Clean reads

`zgrep -c "@H" *.fastq.gz`

1026_CGATGT_L003_R1_cleaned.fastq.gz:2239902  
1026_CGATGT_L003_R2_cleaned.fastq.gz:2185036  
1028_TGACCA_L003_R1_cleaned.fastq.gz:2346641  
1028_TGACCA_L003_R2_cleaned.fastq.gz:2289291  
1030_ACAGTG_L003_R1_cleaned.fastq.gz:1830341  
1030_ACAGTG_L003_R2_cleaned.fastq.gz:1785926  
1032_GCCAAT_L003_R1_cleaned.fastq.gz:1669559  
1032_GCCAAT_L003_R2_cleaned.fastq.gz:1628623  
1034_CAGATC_L003_R1_cleaned.fastq.gz:1726975  
1034_CAGATC_L003_R2_cleaned.fastq.gz:1686096  
1036_CTTGTA_L003_R1_cleaned.fastq.gz:2167733  
1036_CTTGTA_L003_R2_cleaned.fastq.gz:2113553  
1038_AGTCAA_L003_R1_cleaned.fastq.gz:2303252  
1038_AGTCAA_L003_R2_cleaned.fastq.gz:2246060  
1040_AGTTCC_L003_R1_cleaned.fastq.gz:2503620  
1040_AGTTCC_L003_R2_cleaned.fastq.gz:2442529  
1042_ATGTCA_L003_R1_cleaned.fastq.gz:1569298  
1042_ATGTCA_L003_R2_cleaned.fastq.gz:1530977  
1044_CCGTCC_L003_R1_cleaned.fastq.gz:1289573  
1044_CCGTCC_L003_R2_cleaned.fastq.gz:1255946  
H10_CCGTCC_L003_R1_cleaned.fastq.gz:2868521  
H10_CCGTCC_L003_R2_cleaned.fastq.gz:2823436  
H11_GTCCGC_L003_R1_cleaned.fastq.gz:2501740  
H11_GTCCGC_L003_R2_cleaned.fastq.gz:2463568  
H12_GTGAAA_L003_R1_cleaned.fastq.gz:1949967  
H12_GTGAAA_L003_R2_cleaned.fastq.gz:1921436  
H1_CGATGT_L003_R1_cleaned.fastq.gz:2902137  
H1_CGATGT_L003_R2_cleaned.fastq.gz:2860528  
H2_TGACCA_L003_R1_cleaned.fastq.gz:2877404  
H2_TGACCA_L003_R2_cleaned.fastq.gz:2835861  
H3_ACAGTG_L003_R1_cleaned.fastq.gz:3817939  
H3_ACAGTG_L003_R2_cleaned.fastq.gz:3762242  
H4_GCCAAT_L003_R1_cleaned.fastq.gz:2445380  
H4_GCCAAT_L003_R2_cleaned.fastq.gz:2410625  
H5_CAGATC_L003_R1_cleaned.fastq.gz:2628635  
H5_CAGATC_L003_R2_cleaned.fastq.gz:2591411  
H6_CTTGTA_L003_R1_cleaned.fastq.gz:2392095  
H6_CTTGTA_L003_R2_cleaned.fastq.gz:2359532  
H7_AGTCAA_L003_R1_cleaned.fastq.gz:2600520  
H7_AGTCAA_L003_R2_cleaned.fastq.gz:2565283  
H8_AGTTCC_L003_R1_cleaned.fastq.gz:1855368  
H8_AGTTCC_L003_R2_cleaned.fastq.gz:1830315  
H9_ATGTCA_L003_R1_cleaned.fastq.gz:2708022  
H9_ATGTCA_L003_R2_cleaned.fastq.gz:2674454  

### Quality control of cleaned sequencing reads (FASTQC)
https://github.com/s-andrews/FastQC
```
mkdir fastqc_results_clean
cd fastqc_results_clean
fastqc ../*fastq.gz .
mv *fastqc.* fastqc_results_clean/
```

### Using Multiqc to summarize cleaned FastQC results
https://github.com/ewels/MultiQC
```
multiqc .
mv multiqc_report.html multiqc_report_clean.html
scp -P 2292 kwong@kitt.uri.edu:/home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads/fastqc_results_clean/multiqc_report_clean.html /Users/kevinwong/Documents/Projects/P.damicornis_Transcriptome_Analysis/Output/
```

### Aligning reads to reference transcriptome (Script from E. Roberts)
https://github.com/erinroberts/apoptosis_data_pipeline/blob/master/Streamlined%20Pipeline%20Tutorial/Apoptosis_Pipeline_Tutorial_with_Reduced_Dataset.Rmd

`conda install -c bioconda hisat2`  
`nano HISAT2.sh`
```
#!/bin/bash

#Specify working directory
F=/home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads

hisat2-build -f $F/P_damicornis_transcriptome_Seneca2015.fasta $F/P_damicornis_transcriptome_Seneca2015_edited
#-f indicates that the reference input files are FASTA files

#Aligning paired end reads
array1=($(ls $F/*_R1_cleaned.fastq.gz))

for i in ${array1[@]}; do
	hisat2 --dta -x $F/P_damicornis_transcriptome_Seneca2015_edited  -1 ${i} -2 $(echo ${i}|sed s/_R1_cleaned/_R2_cleaned/) -S ${i}.sam
	echo "HISAT2 PE ${i}" $(date)
done
```
`bash HISAT2.sh`

e.g. OUTPUT
```
2041595 reads; of these:
  2041595 (100.00%) were paired; of these:
    453679 (22.22%) aligned concordantly 0 times
    920168 (45.07%) aligned concordantly exactly 1 time
    667748 (32.71%) aligned concordantly >1 times
    ----
    453679 pairs aligned concordantly 0 times; of these:
      24418 (5.38%) aligned discordantly 1 time
    ----
    429261 pairs aligned 0 times concordantly or discordantly; of these:
      858522 mates make up the pairs; of these:
        543750 (63.34%) aligned 0 times
        192951 (22.47%) aligned exactly 1 time
        121821 (14.19%) aligned >1 times
86.68% overall alignment rate
HISAT2 PE /home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads/1026_CGATGT_L003_R1_cleaned.fastq.gz Wed Apr 25 14:17:22 EDT 2018
```

### Convert SAM to BAM using SAMTools (Script from E. Roberts)
https://github.com/erinroberts/apoptosis_data_pipeline/blob/master/Streamlined%20Pipeline%20Tutorial/Apoptosis_Pipeline_Tutorial_with_Reduced_Dataset.Rmd

`conda install samtools`

`nano sambam.sh`

```
#!/bin/bash

#SAMTOOLS sort to convert the SAM file into a BAM file to be used with StringTie
#SHOULD NOT PERFORM FILTERING ON HISAT2 OUTPUT
F=/home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads

array3=($(ls $F/*.sam))
	for i in ${array3[@]}; do
		samtools sort ${i} > ${i}.bam #Stringtie takes as input only sorted bam files
		echo "${i}_bam"
	done

#Get bam file statistics for percentage aligned with flagstat
# to get more detailed statistics use $ samtools stats ${i}
array4=($(ls $F/*.bam))
	for i in ${array4[@]}; do
		samtools flagstat ${i} > ${i}.bam.stats #get % mapped
	#to extract more detailed summary numbers
		samtools stats ${i} | grep ^SN | cut -f 2- > ${i}.bam.fullstat
		echo "STATS DONE" $(date)
	done
```
`bash sambam.sh`

### Assemble reads to reference using Stringtie (Script from E. Roberts)
https://github.com/erinroberts/apoptosis_data_pipeline/blob/master/Streamlined%20Pipeline%20Tutorial/Apoptosis_Pipeline_Tutorial_with_Reduced_Dataset.Rmd

`conda install -c bioconda stringtie `

`nano stringtie.sh`

```
#!/bin/bash

#This script takes bam files from HISAT (processed by SAMtools) and performs StringTie assembly and quantification and converts
# data into a format that is readable as count tables for DESeq2 usage

F=/home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads

# StringTie to assemble transcripts for each sample with the GFF3 annotation file
array1=($(ls $F/*.bam))

for i in ${array1[@]}; do
	stringtie -o ${i}.gtf -l $(echo ${i}|sed "s/\..*//") ${i}
	echo "${i}"
done
	# command structure: $ stringtie <options> -G <reference.gtf or .gff> -o outputname.gtf -l prefix_for_transcripts input_filename.bam
	# -o specifies the output name
	# -G specifies you are aligning with an option GFF or GTF file as well to perform novel transcript discovery
	# -l Sets <label> as the prefix for the name of the output transcripts. Default: STRG
	# don't use -e here if you want it to assemble any novel transcripts

#StringTie Merge, will merge all GFF files and assemble transcripts into a non-redundant set of transcripts, after which re-run StringTie with -e
#create mergelist.txt in nano, names of all the GTF files created in the last step with each on its own line
ls *.gtf > P_dam_mergelist.txt

#check to sure one file per line
cat P_dam_mergelist.txt

#Run StringTie merge, merge transcripts from all samples (across all experiments, not just for a single experiment)

stringtie --merge -o $F/P_dam_stringtie_merged.gtf $F/P_dam_mergelist.txt
#-A here creates a gene table output with genomic locations and compiled information that I will need later to fetch gene sequences (need annotation file)
#FROM MANUAL: "If StringTie is run with the -A <gene_abund.tab> option, it returns a file containing gene abundances. "
#-G is a flag saying to use the .gff annotation file

#Re-estimate transcript abundance after merge step
	for i in ${array1[@]}; do
		stringtie -e -G $F/P_dam_stringtie_merged.gtf -o $(echo ${i}|sed "s/\..*//").merge.gtf ${i}
		echo "${i}"
	done
	# input here is the original set of alignment files
	# here -G refers to the merged GTF files
	# -e creates more accurate abundance estimations with input transcripts, needed when converting to DESeq2 tables

echo "DONE" $(date)
```

`bash stringtie.sh`

### Prepare StringTie output for DESeq2

`wget https://ccb.jhu.edu/software/stringtie/dl/prepDE.py`  
`conda install python=2.7`

`nano prepDESeq2.sh`

```
#!/bin/bash

F=/home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads

array2=($(ls *R1_cleaned.merge.gtf))

for i in ${array2[@]}; do
	echo "$(echo ${i}|sed "s/\_R1_cleaned..*//") $F/${i}" >> $F/Pdam_sample_list.txt
done

python $F/prepDE.py -i $F/Pdam_sample_list.txt

echo "STOP" $(date)
```

`bash prepDESeq2.sh`

#### Uploading sample information to KITT

```
scp -r -P 2292 /Users/kevinwong/Documents/Projects/P.damicornis_Transcriptome_Analysis/Data/Pdam_2011_sample_info.csv kwong@kitt.uri.edu:/home/kwong/Final_Project/raw/allraw/fullreads/cleaned_reads/P_Dam_Transcriptome
```

## Using remote RStudio to perform DESeq2 Analysis
* In web browser: http://kitt.uri.edu:8787/ and log into KITT
* All of the following commands will be executed in RStudio
* Scripts are modified from E. Roberts and H. Putnam

#### Load in packages
```
#call the DESeq2 library
source("http://bioconductor.org/biocLite.R")
biocLite("BiocUpgrade")
biocLite("DESeq2")
library("DESeq2")
#install.packages("fdrtool")
library(fdrtool)
#install.packages("dplyr")
library(dplyr)
#install.packages("tidyr")
library(tidyr)
#install.packages("reshape2")
library(reshape2)
library(ggplot2)
#install.packages("tm")
#library(tm)
library(genefilter)
#install.packages("pheatmap")
library(pheatmap)
#install.packages("RColorBrewer")
library(RColorBrewer)
library(limma)
library(spdep)
library(adegenet)
biocLite("GSEABase")
#library(GSEABase)
biocLite("pathview")
#library("pathview")
biocLite("goseq")
#library("goseq")
library("GO.db")
#devtools::install_github("hms-dbmi/UpSetR")
library("UpSetR")
library("reshape2")
library(lattice)
library(latticeExtra)
```

#### Reading in files

```
#Read in stringtie merged file
Pdam_stringtie <- read.csv(file= "../P_dam_stringtie_merged.gtf", sep="\t", header = FALSE)

#set colnames for the attributes
colnames(Pdam_stringtie) <- c('seqname', 'source', 'feature','start','end','score','strand','frame', 'attribute')

#subset for just transcript lines
Pdam_stringtie_transcripts <- Pdam_stringtie %>% filter(feature =="transcript")
```

#### DEG Analysis with TRANSCRIPT Count Matrix
* Pdam_2011_sample_info.csv file contains metadata on the count table's samples  
* Make sure excel sample info is in the same order or these commands will change data to be wrong

```
#Extract correct rows and columns from the PHENO DATA and transcript data
Pdam_TranscriptCountData <- as.data.frame(read.csv("../transcript_count_matrix.csv", row.names="transcript_id"))
head(Pdam_TranscriptCountData)

###filtering values for PoverA
#set filter values for PoverA, P percent of the samples have counts over A
filt <- filterfun(pOverA(0.25,5))

#create filter for the counts data
tfil <- genefilter(Pdam_TranscriptCountData, filt)

#identify transcripts to keep by count filter
keep <- Pdam_TranscriptCountData[tfil,]

#identify transcript list
gn.keep <- rownames(keep)

#data filtered in PoverA, P percent of the samples have counts over A
counts.5x <- as.matrix(Pdam_TranscriptCountData[which(rownames(Pdam_TranscriptCountData) %in% gn.keep),])
write.csv(counts.5x, file="filtered_counts.csv")

Pdam_sample_ColData <- read.csv("Pdam_2011_sample_info.csv", header=TRUE, sep=",")
print(Pdam_sample_ColData)

#change rownames to match
rownames(Pdam_sample_ColData) <- Pdam_sample_ColData$Sample.ID
colnames(counts.5x) <- Pdam_sample_ColData$Sample.ID
head(Pdam_sample_ColData)
head(counts.5x)

# Check all sample IDs in Pdam_sample_ColData are also in Pdam_TranscriptCountData and match their orders
all(rownames(Pdam_sample_ColData) %in% colnames(counts.5x))  #Should return TRUE
# returns TRUE
all(rownames(Pdam_sample_ColData) == colnames(counts.5x))    # should return TRUE
#returns TRUE

#give the treatment column levels
Pdam_sample_ColData$Treatment <- factor(Pdam_sample_ColData$Treatment)
levels(Pdam_sample_ColData$Treatment)
```

#### Construct DESeq dataset from matrix
* DESeqDataSet from count matrix and labels, separate into resistant and susceptible
* add an interaction term to compare treatment between two conditions
* layout used for interactions: https://support.bioconductor.org/p/58162/

```
#apply a regularized log transformation to minimize effects of small counts and normalize wrt library size
rld <- rlog(ddsS4, blind=FALSE)
head(assay(rld), 3) #view data

#calculate distance matix
sampleDists <- dist(t(assay(rld)))

#distance matrix
sampleDistMatrix <- as.matrix(sampleDists)

#assign row names
rownames(sampleDistMatrix) <- colnames(rld)

#assign col names
colnames(sampleDistMatrix) <- NULL

#assign colors
colors <- colorRampPalette( rev(brewer.pal(9, "Blues")) )(255)

```

#### Plotting heatmap for Expression Visualization
```
pdf(file="heatmapEV.pdf")
pheatmap(sampleDistMatrix, #plot matrix of expression similarity
         clustering_distance_rows=sampleDists, #cluster rows
         clustering_distance_cols=sampleDists, #cluster columns
         col=colors) #set colors
dev.off()
```
![EVHeatmap](https://github.com/kevinhwong1/P.damicornis_Transcriptome_Analysis/blob/master/Output/heatmapEV.jpg)

#### Plotting PCA from Expression visualization
```
pdf(file="PCAEV.pdf")
plotPCA(rld, intgroup = c("Treatment")) #plot PCA of samples with all data
dev.off()
```
![EVPCA](https://github.com/kevinhwong1/P.damicornis_Transcriptome_Analysis/blob/master/Output/PCAEV.jpg)

#### Differential Gene Expression Analysis
* Interaction Test: test of the factor of "group" with all combinations of the original factors as groups

```
#run differential expression test by group using the wald test
DEG.int <- DESeq(ddsS4)

#save DE results
DEG.int.res <- results(DEG.int)

#view DE results
resultsNames(DEG.int)

#identify the number of significant p values with 5%FDR (padj<0.05)
sig.num <- sum(DEG.int.res$padj <0.05, na.rm=T)

#identify signficant pvalues with 5%FDR
sig <- subset(DEG.int.res, padj<0.05,)

#subset list of sig transcripts from original count data
sig.list <- ddsS4[which(rownames(ddsS4) %in% rownames(sig)),]

#apply a regularized log transformation to minimize effects of small counts and normalize wrt library size
rsig <- rlog(sig.list, blind=FALSE)
write.csv(counts(sig.list), file="DEG_5FDR.all.csv")
```

#### Plotting DEG PCA
```
PCA.plot <- plotPCA(rsig, intgroup = c("Treatment")) #Plot PCA of all samples for DEG only
PCA.plot #view plot
PC.info <-PCA.plot$data #extract plotting data
pdf(file="PCA.DEG.pdf")
plot(PC.info$PC1, PC.info$PC2, xlim=c(-30,30), ylim=c(-16, 10), xlab="PC1 86%", ylab="PC2 5%", col = c("lightpink2", "steelblue1")[as.numeric(PC.info$Treatment)],)
legend(x="top",
       bty="n",
       legend = c("Ambient", "High"),
       text.col = c("lightpink2","steelblue1"),
       pch = c(15, 15),
       col = c("white","white", "black", "black"),
       cex=1)
dev.off()
```
![DEGPCA](https://github.com/kevinhwong1/P.damicornis_Transcriptome_Analysis/blob/master/Output/PCA.DEG.jpg)

#### Plotting DEG heatmap
```
#sort by decreasing sig
topVarGenes <- head(order(rowVars(assay(rsig)),decreasing=TRUE),sig.num)

#make an expression object
mat <- assay(rsig)[ topVarGenes, ]

#difference in expression compared to average across all samples
mat <- mat - rowMeans(mat)

#ordering columns by treatment
col.order <- c("1028","1034", "1038", "1040", "H11", "H12", "H2", "H4", "H5", "H6", "H7", "1026", "1030", "1032", "1036", "1042", "1044", "H1", "H10", "H3", "H8", "H9")
mat <- mat[,col.order]

#make dataframe
df <- data.frame(colData(rsig)[c("Treatment")])

pdf(file="DEG_Heatmap.pdf")
PMAT<- pheatmap(mat, annotation_col = df, clustering_method = "average",
         clustering_distance_rows="euclidean", show_rownames =FALSE, cluster_cols=FALSE,
         show_colnames =FALSE) #plot heatmap of all DEG by group
dev.off()
```
![DEGHeatmap](https://github.com/kevinhwong1/P.damicornis_Transcriptome_Analysis/blob/master/Output/DEG_Heatmap.jpg)
