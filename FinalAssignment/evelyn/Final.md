## Final Project
### Brief Summary
The two species of interest to be analysed for population structure are Sardinella aurita and Sardinella maderensis. These are two separate species which  are among the most abundant small pelagic sardine fish species in the Gulf of Guinea region in West Africa however, currently, their abundance is known to fluctuate greatly and  declining in the region.
The population structure for each of these species among the countries in the Gulf of Guinea is currently absent . Therefore,there is limitation on the proper management and the sustainability of these fisheries within the region.
The basic goals of the analysis are as follows;
1. Perform a denovo assembly of raw reads, SNP calling and filtering using dDocent pipeline.
2. Perform a  population structure analysis on the two species separately using neutral SNP loci.
### Data description
These data is a demultiplexed ddRadseq PE sequencing on a illumina Hiseq for each separate species with a size of ~46G.
i. Populations:
a.sardinella aurita: five(5) populations(Ghana, Togo, Benin, Senegal, Mauritania)
b.sardinella maderensis: four(4) populations(Ghana, Benin, Senegal, Mauritania)
c.Individuals per Population for each species: 10 .
d.Number of reads:  96 million reads
e.sequencing Platform: HiSeq 2500 (150bp PE)

## Analysis Plan
### Initial Raw Data Assessment and Characterization
Assess the  general quality of the reads obtained using FastQC.

### Bioinformatic Processing
Denovo assembly, SNP calling and filtering using dDocent pipeline for analysis of Radseq data.
a.Read Trimming. This will remove reads of low quality and illumina adapters if detected.
b.De Novo Reference Assembly. The two species do not have a reference genome therefore a need to perform a denovo assembly of a reference genome for each species separately.
c.Read Mapping using BWA in the pipeline.
d.SNP calling using freebayes and SNP filtering using VCFtools in the pipeline.
e.Run Bayescan and pcadapt to filter out outliers and obtain neutral loci SNPs data for population structure analysis.

### population genetic statistics
Software for analysis:  R packages(Adegenet, Gstudio, Hierfstat etc), Stacks and Genodive.
i.Determine basic genetic statistics (Heterozygosity,FIS, allele frequency etc) to measure genetic diversity.
For population structure;
ii.Pairwise FST comparison
iii.PCA plot
iv.DAPC plot
v.Phylogenetic tree
vi.structure-like analysis using compoplot.

### References
Puritz, J. B., Hollenbeck, C. M. & Gold, J. R. 2014 dDocent: a RADseq, variant-calling pipeline
designed for population genomics of non-model organisms. PeerJ 2, e431. (doi:10.7717/peerj.431)

Sardinella, T. H. E., Off, F., Coast, T. H. E., West, O. F., Case, T. H. E., Common, O. F. A., & Resource, P. (1991). T. R. Brainerd 2.

Series, E. (2009). Cecaf/ecaf series 12/74 copace/pace séries 12/74, (October), 19–28.

