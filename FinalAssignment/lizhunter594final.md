# **Summary**
Apicomplexa is a phylum synonymous with obligate parasitism, containing several species of significance for human health, including Plasmodium, Toxoplasma, and Cryptosporidium. Though this phylum was previously known to be universally parasitic, genus Nephromyces reportedly engages in a mutualistic relationship with its host ascidians in the Mogula family, as evidenced by its virtual 100% infection rate. Sister taxa Cardiosporidium also hosts in ascidians, but is still considered by the current literature to be parasitic. Nephromyces only occurs in multispecies infections with up to 26 species per host, whereas genus Cardiosporidium contains only a single species. Both these taxa are also known to host bacterial endosymbionts. The phylogeny suggests Nephromyces did not simply retain the genes required to maintain the status of a mutualist, but in fact regained them. The reversal of parasitism is extremely uncommon, and the focus of our research into gaining insight into how such a lifestyle transition occurred. These unique genuses are close enough to provide a strong basis for comparison to highlight the genomic differences that have led to the reversal of parasitism in genus Nephromyces.

## Goals include:
1. To assemble high likelihood transcriptomes from each genus and differentiate both host and bacterial sequences from the final assembly

2. To compare the transcriptomes of Nephromyces and Cardiosporidium to the published annotated genomes of other Apicomplexans and determine loci under selective pressure
3. To sort loci under selection from the final dataset by those associated with virulence and host immune evasion, and examine the molecular and functional pathway differences therein, in particular comparing parasitic Cardiosporidium to mutualistic Nephromyces

# **Data Description**
#### Nephromyces
		Lab grown 4 species “isolate” sample - single individual
		Illumina HiSeq paired end RNA
		1 lane, split 7 libraries

#### Cardiosporidium: 25% sucrose gradient sample
		Locally collected individuals - multiple individuals
		Illumina HiSeq paired end RNA
		1 lane, split 3 libraries
		230,155,470 raw sequences

# **Analysis**
## Assembly:
1. Quality check - Fastq
2. Trimming - Trimmomatic
3. Assembly - Trinity
4. Binning
  * Sort by taxonomy (blast to refseq)
  * Re-map reads to sorted assemblies

## Comparison:
1. Compilation of Apicomplexan published genomes
  * Potentially sorted for factors associated with virulence and host immune evasion at this stage? Or maybe it would be smarter to compare across the board and then examine processes of interest
2. Comparison of loci under selection with pamL
3. Analysis of functional pathway differences
  * Kegg/Interpro
4. Visualization of molecular/functional pathway variances
  * GOslim 
