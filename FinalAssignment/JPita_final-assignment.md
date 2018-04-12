# BIO 594: Final Assignment Plan
Jessica N. Pita Aquino

## Brief Summary
For this study I will analyze the native range population genetic structure of the Cuban Brown Anole (<i>Anolis sagrei</i>). Kolbe and collaborators (2004) collected samples from 71 native populations to assay levels of genetic variation and conducted population-genetic analyses of mitochondrial DNA (mtDNA) sequences. Results showed that native range populations are highly genetically structured; notable patterns include substantial divergence among East Cuba and West Cuba populations, due to geographical distance. Moreover, most genetic variation was partitioned among, rather than within, populations. 
In 2008 native populations were resampled and nuclear DNA was obtained. With double-digest restriction site-associated DNA sequencing (ddRADseq) data we can have a more comprehensive view of these patterns. Genome-wide SNPs markers will provide a substantially more precise estimate of population geographic structure. This new approach provides both a valuable tool to determine population structure and will allow us to determine if this structural pattern persists. 

## Objectives 
For this study I will analyze ddRAD-seq data for native populations of the Cuban Brown Anole (<i>A. sagrei</i>) to:
(1)	Identify genome-wide SNP markers that are segregating among native <i>A. sagrei</i> samples
(2)	Characterize population structure

## Data Description
- Type: ddRAD-seq (sequenced on Illumina HiSeq 4000, with 150 bp paired end)
- Location: Data will be located and analyzed in KITT
- Size: 
- Populations (N=4): Esmerelda (ESM; Eastern Cuba), Caibarien (CAB; Central Cuba), Mariel (MAR; Western Cuba), Soroa (SOR; Western Cuba)

## Analysis Plan
-	FASTQC: Examine data quality
-	Trimmomatic: Trim adapters and low quality reads
-	dDocent: Make a de novo assembly, SNP calling and filtering 
-	VCFtools: Calculate pairwise Fst among all populations
-	R packages (pcadapt, adegenet) and STRUCTURE: Generate PCA, DAPC and STRUCTURE plots
  - PCA: individual variation
  - DAPC: individual variation and possible number of clusters
  - STRUCTURE: allele frequencies to generate clusters

## References
Kolbe, J., Glor, R., Rodríguez Schettino, L., Chamizo Lara, A., Larson, A., Losos, J. (2004). Genetic variation increases during biological invasion by a Cuban lizard. Nature. 431. 177-81. 10.1038/nature02807.
<br>
<br>
Puritz, J. B., Hollenbeck, C. M. & Gold, J. R. (2014). dDocent: a RADseq, variant-calling pipeline designed for population genomics of non-model organisms. PeerJ 2, e431. doi:10.7717/peerj.431.
