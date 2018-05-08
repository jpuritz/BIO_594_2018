# A transcriptomic analysis of pre-conditioned reef-building corals to elevated temperature and PCO2 conditions during reproduction.

## Background

In 2015, Dr. Hollie Putnam published a peer-reviewed journal article describing the potential for trans-generational acclimatization in the reef-building coral, *Pocillopora damicorns* (Putnam and Gates, 2015). 22 adult *P. damicornis* colonies were collected from the fringing reefs of Kaneohe Bay, Hawaii, and were subjected to either ambient (26.5°C and 417 atm PCO2) or high (28.9°C and 805 atm PCO2) treatment conditions for 1.5 months prior to the anticipated peak larval release in September 2011. After the peak larval release, the larvae experienced a reciprocal exposure to the ambient and high experimental treatments for 5 days. Following the exposure, larval size and dark respiration was measured for the larvae. Additionally, the photophysiology of the *Symbiodinium*, photosynthetic and dark respiration rates, and calcification rates were measured for the adult corals post larval release.

Of the 12 colonies in this experiment released larvae (~55%), seven colonies released larvae in the ambient treatment and five colonies released larvae in the high treatment. The *P. damicornis* colonies in the high treatment had reduced photochemical efficiency, photosynthetic rates, and photosynthesis to respiration rate ratios than the colonies in the ambient treatment. However, there was a significant interaction between parental exposure and larval exposure for the size-normalized dark respiration rates of the larvae. The larvae that were brooded in the high parental treatments had higher respiration rates in the high larval treatment than the larvae that were brooded in the ambient treatments. This indicates the potential for trans-generational acclimatization of *P. damicornis* to elevated temperature and PCO2 conditions.

## Objectives

The objective of this study is to analyze the sampled transcriptomes of the 22 colonies in this experiment to determine if there is differential gene expression between the ambient and high treatment groups. Additionally, the genes will be fully annotated to give insight on the possible mechanisms behind trans-generational acclimatization.

## Data
- Population: One population under two different Treatment conditions.
- Location: The data location and analyses will be performed on KITT.
- Size: 22 100bp PE transcriptomes. Sequenced with  Illumina Genome Analyzer IIx housed at the Hawaii Institute of Marine Biology.


## Methods

-	Check for upload completion (checksum)
-	Count the RAW reads
-	Examine quality of data (FASTQC)
-	Trimming adapters and low quality reads (BBTools)
-	Statistics and file conversion (HISAT2)
-	Read alignment to reference transcriptome (SAM Tools)
-	Assembly to reference transcriptome (String Tie)
-	Differential expression analysis (DESeq2)
-	Gene annotation (Trinotate)

