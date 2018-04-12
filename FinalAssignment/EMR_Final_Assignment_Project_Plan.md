# Final Assigmment for BIO 594 April 2018

### Erin Roberts

## Project Plan

### Brief Summary
  The genome of the eastern oyster, *Crassostrea virginica* was sequenced in 2016 from a single inbred gynogenetic oyster^[1]^. This was chosen as a strategy to decrease the genetic polymorphism
  present in oysters. In order to survey the genetic variation across populations of the eastern oyster, a whole genome sequencing approach was used for 14 different populations, using 6 oysters from each population.
  I performed DNA extraction and sample preparation for this project as part of the Eastern Oyster Genome Consortium. WGS data is now currently available from these samples.
  Though many analyses are likely going to be performed on this large data set, I would like to start by estimating neutral population structure from this data.

### Data Description
Whole genome sequencing data is available for 90 oysters from each of 14 populations. 5 or 6 oysters were sequenced for each population (differences in number due to library prep errors). Reads were sequenced paired-end using an Illumina HiSeq X PE150. Libraries were created without PCR. Sequencing was performed at a sequencing depth of 20X. LuciGen adaptors were used. Read sets have been fully sequenced and are currently available for 90 samples and the data is located on the Genome Quebec online server. The average quality score of reads is 38. Read sets will be transferred to the URI bluewaves cluster for analyses.  

### Analysis Plan

1. Alignment of reads to the eastern oyster reference genome using BWA mem.
2. Sorting of BAM files using PICARD SortSam
3. Mark duplicates using PICARD MarkDuplicates
4. Perform variant calling with FreeBayes
5. Filter variant calls to remove low confidence calls using samtools
6. Characterize neutral genomic variations by calcalculating allele frequencies, percentage of exclusive variants, and the level of nucleotide diversity using VCFTools
7. Calculate pairwise linkage disequilibrium via the correlation coefficient in VCFTools
8. Assess genetic structure by using a PCA through the package adegenet 

### References
Benjelloun, Badr, et al. "Characterizing neutral genomic diversity and selection signatures in indigenous populations of Moroccan goats (Capra hircus) using WGS data." Frontiers in genetics 6 (2015): 107.

