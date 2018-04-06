# Final Project Plan
#### Ian Bishop - BIO-594

## Brief Summary
<i>Describe the project/system, and highlight the basic goals of the
analysis.</i>

The species I propose to anayze for our final project is <i>Thalassiosira rotula</i>, a marine phytoplanktonic diatom with a global/cosmopolitan distribution. This species is closely related <i>Thalassiosira pseudonana</i>, which is one of a prized few fully sequenced and heavily annotated diatom genomes<sup>1</sup>. Although the two species are congeneric, <i>T. rotula</i> would definitely be considered a non-model organism and in assembling sequencing data I propose adopting a de novo approach.

Last year, a post-doc in our lab sequenced 40 diatoms genomes (WGS), 20 each from populations in Narragansett Bay and Durban, South Africa. The dataset has been previously analyzed, but there were concerns about its de novo assembly quality. It has not yet been published.

The basic goals of the proposed project are as follows:
1. Develop a personal pipeline for analyzing neutral population structure in marine diatoms. My PhD work will be focusing on populations of cultured diatoms recently collected from 6 different regions of the Southern Ocean. I will be using microsatellites to characterize this structure (see goal #2), but I also want to use SNPs. This dataset will help me prep for my own analyses.
2. Test my ability to discover candidate microsatellite markers using the same shotgun sequencing dataset as is used to analyze SNPs. As a library of microsatellite markers have recently been developed in our lab for <i>T. rotula</i>, I would like to compare what I might find bioinformatically (with bioconda tools like pal_finder) with markers found by other means.

## Data description
<i>Summarize the type of data, the location, and the size of the data set</i>

These data are from a multiplexed whole genome shotgun sequencing effort. The closely related <i>T. pseudonana</i> has a an estimated ~35mb genome size.

<i>Populations</i>: 2 (eastern North America - Atlantic Ocean; southern Africa - Indian Ocean)
<br>
<i>Invididuals per Population</i>: 20
<br>
<i>Raw WGS dataset size</i>: 465 million reads
<br>
<i>Library Prep Kit</i>: Illumina Nextera XT library kit
<br>
<i>Sequencing Platform</i>: HiSeq 2500 (125bp PE, 1 lane)

## Analysis Plan
<i>Briefly outline your analysis plan with a one-line justification for each
step.</i>

##### Initial Raw Data Assessment and Characterization
* Assess incoming dataset size and general read quality

##### Bioinformatic Processing
* Read Trimming and Adapter Removal
* De Novo Reference Assembly
  * congeneric model reference genome available, likely too genetically distant. Also practice with de novo assembly will help with future work, as I will definitely not be using a model organism
* Contig binning.
  * DNA extractions derive from cultures and while <i>T. rotula</i> should be only eukaryote present, lots of assembled contigs will be bacterial and viral in origin
* Filtering of non-eukaryote contigs from de novo reference
* Read Mapping
* SNP Variant Calling
  * Filter out putatively selected SNP loci using BayeScan
* Microsatellite Calling
  * Filter for stable flanking region, variability of repeat motif, using [pal_finder](https://sourceforge.net/projects/palfinder/)

##### Population-level
* Neutral Population Structure
  * DAPC using SNPs
  * DAPC using microsatellites
* Recovery of previously developed <i>T. rotula</i> microsatellite location
  * Extent of overlap between project-generated microsatellite loci and already developed and [utilized set](http://www.pnas.org/content/pnas/suppl/2017/02/15/1612346114.DCSupplemental/pnas.1612346114.sapp.pdf) (Whittaker & Rynearson 2017)<sup>2</sup>


##### References
  <sup>1</sup>
  Armbrust, E. V., Berges, J. A., Bowler, C., Green, B. R., Martinez, D., Putnam, N. H., ... & Brzezinski, M. A. (2004). The genome of the diatom <i>Thalassiosira pseudonana</i>: ecology, evolution, and metabolism. <i>Science</i> 306(5693): 79-86.
  <br><sup>2</sup>
  Whittaker, K. A., & Rynearson, T. A. (2017). Evidence for environmental and ecological selection in a microbe with no geographic limits to gene flow. <i>Proceedings of the National Academy of Sciences</i> 114(10): 2651-2656.
