# **Week 8** #

    mkdir week8
    ln -s /home/BIO594/Exercises/Week_7and8/simulated/*.fq.gz .

### Run dDocent ###
  * Data cutoff 8

### Filter output for SNPs ###

    mkdir Filter
    cd Filter/
    ln -s ../TotalRawSNPs.vcf .

    vcftools --vcf TotalRawSNPs.vcf --max-missing 0.5 --maf 0.001 --minQ 20 --recode --recode-INFO-all --out TRS

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
    --vcf TotalRawSNPs.vcf
    --recode-INFO-all
    --maf 0.001
    --minQ 20
    --max-missing 0.5
    --out TRS
    --recode

    After filtering, kept 80 out of 80 Individuals
    Outputting VCF file...
    After filtering, kept 2970 out of a possible 2990 Sites
    Run Time = 0.00 seconds

    vcftools --vcf TRS.recode.vcf --minDP 5 --recode --recode-INFO-all --out TRSdp5

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
    	--vcf TRS.recode.vcf
    	--recode-INFO-all
    	--minDP 5
    	--out TRSdp5
    	--recode

    After filtering, kept 80 out of 80 Individuals
    Outputting VCF file...
    After filtering, kept 2970 out of a possible 2970 Sites
    Run Time = 1.00 seconds

    pop_missing_filter.sh TRSdp5.recode.vcf ../popmap 0.05 1 TRSdp5p05
    rm: cannot remove ‘badloci’: No such file or directory

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
    	--vcf TRSdp5.recode.vcf
    	--keep keep.PopA
    	--out PopA
    	--missing-site

    Keeping individuals in 'keep' list
    After filtering, kept 20 out of 80 Individuals
    Outputting Site Missingness
    After filtering, kept 2970 out of a possible 2970 Sites
    Run Time = 0.00 seconds

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
    	--vcf TRSdp5.recode.vcf
    	--keep keep.PopB
    	--out PopB
    	--missing-site

    Keeping individuals in 'keep' list
    After filtering, kept 20 out of 80 Individuals
    Outputting Site Missingness
    After filtering, kept 2970 out of a possible 2970 Sites
    Run Time = 0.00 seconds

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
    	--vcf TRSdp5.recode.vcf
    	--keep keep.PopC
    	--out PopC
    	--missing-site

    Keeping individuals in 'keep' list
    After filtering, kept 20 out of 80 Individuals
    Outputting Site Missingness
    After filtering, kept 2970 out of a possible 2970 Sites
    Run Time = 0.00 seconds

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
    	--vcf TRSdp5.recode.vcf
    	--keep keep.PopD
    	--out PopD
    	--missing-site

    Keeping individuals in 'keep' list
    After filtering, kept 20 out of 80 Individuals
    Outputting Site Missingness
    After filtering, kept 2970 out of a possible 2970 Sites
    Run Time = 0.00 seconds

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
    	--vcf TRSdp5.recode.vcf
    	--exclude-positions loci.to.remove
    	--recode-INFO-all
    	--out TRSdp5p05
    	--recode

    After filtering, kept 80 out of 80 Individuals
    Outputting VCF file...
    After filtering, kept 2800 out of a possible 2970 Sites
    Run Time = 1.00 seconds

### Run dDocent Again ###
    dDocent_filters TRSdp5p05.recode.vcf TRSdp5p05
    Number of sites filtered based on allele balance at heterozygous loci, locus quality, and mapping quality / Depth
    691 of 2800

    Number of additional sites filtered based on overlapping forward and reverse reads
    0 of 2109

    Is this from a mixture of SE and PE libraries? Enter yes or no.
    yes
    Number of additional sites filtered based on properly paired status
    0 of 2109

    Number of sites filtered based on high depth and lower than 2*DEPTH quality score
    312 of 2109



                                             Histogram of mean depth per site


    250 +-+-+---+---+---+---+---+---+--+---+---+---+---+---+---+---+---+---+---+---+---+---+--+---+---+---+---+---+-+-+
        +   +   +   +   +   +   +   +  +   +   +   +   +   +   +   +   +   +   +   +   +   +  +   +   +   +   +   +   +
        |                                      *            'meandepthpersite' using (bin($1,binwidth)):(1.0) ******* |
        |                                     **                                                                      |
        |                                     **                                                                      |
    200 +-+                                  ****                                                                   +-+
        |                                    ****                                                                     |
        |                                    ****                                                                     |
        |                                  ******                                                                     |
    150 +-+                                *******                                                                  +-+
        |                                  *******                                                                    |
        |                                  *******                                                                    |
        |                                  *******                                                                    |
        |                                  ********                                                                   |
    100 +-+                                ********                                                                 +-+
        |                                  ********                                                                   |
        |                                  ********                                                                   |
        |                                **********                                                                   |
    50 +-+                              **********                                                                 +-+
        |                               ***********                                                                   |
        |                              *************                                                                  |
        |                              ***************                                                                |
      +   +   +   +   +   +   +   +  ****************+   +   +   +   +   +   +   +   +   +  +   +   +   +   +   +   +
    0 +-+-+---+---+---+---+---+---+********************--+---+---+---+---+---+---+---+---+--+---+---+---+---+---+-+-+
      10  15  20  25  30  35  40  45 50  55  60  65  70  75  80  85  90  95 100 105 110 11 120 125 130 135 140 145 150
                                                        Mean Depth

    If distrubtion looks normal, a 1.645 sigma cutoff (~90% of the data) would be 5152.27348
    The 95% cutoff would be 63

    Would you like to use a different maximum mean depth cutoff than 63, yes or no
    yes

    Please enter new cutoff
    75
    Number of sites filtered based on maximum mean depth
    0 of 2109

    Number of sites filtered based on within locus depth mismatch
    0 of 1917

    Total number of sites filtered
    883 of 2800

    Remaining sites
    1917

    Filtered VCF file is called Output_prefix.FIL.recode.vcf
    Filter stats stored in TRSdp5p05.filterstats

### More VCF Filtering ###

    vcfallelicprimitives -k -g TRSdp5p05.FIL.recode.vcf |sed 's:\.|\.:\.\/\.:g' > TRSdp5p05F.prim
    vcftools --vcf TRSdp5p05F.prim --recode --recode-INFO-all --remove-indels --out SNP.TRSdp5p05F

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
	  --vcf TRSdp5p05F.prim
	  --recode-INFO-all
      --out SNP.TRSdp5p05F
	  --recode
	  --remove-indels

    After filtering, kept 80 out of 80 Individuals
    Outputting VCF file...
    After filtering, kept 1654 out of a possible 2036 Sites
    Run Time = 1.00 seconds

    filter_hwe_by_pop.pl -v SNP.TRSdp5p05F.recode.vcf -p ../popmap -c 0.5 -out SNP.TRSdp5p05FHWE
    Processing population: PopA (20 inds)
    Processing population: PopB (20 inds)
    Processing population: PopC (20 inds)
    Processing population: PopD (20 inds)
    Outputting results of HWE test for filtered loci to 'filtered.hwe'
    Kept 1654 of a possible 1654 loci (filtered 0 loci)

    vcftools --vcf SNP.TRSdp5p05FHWE.recode.vcf --maf 0.05 --recode --recode-INFO-all --out SNP.TRSdp5p05FHWEmaf05

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
	--vcf SNP.TRSdp5p05FHWE.recode.vcf
	--recode-INFO-all
	--maf 0.05
	--out SNP.TRSdp5p05FHWEmaf05
	--recode

    After filtering, kept 80 out of 80 Individuals
    Outputting VCF file...
    After filtering, kept 927 out of a possible 1654 Sites
    Run Time = 0.00 seconds

    java -jar /usr/local/bin/PGDSpider2-cli.jar -inputfile SNP.TRSdp5p05FHWEmaf05.recode.vcf -outputfile SNP.TRSdp5p05FHWEBS -spid BSsnp.spid
    WARN  15:10:50 - PGDSpider configuration file not found! Loading default configuration.
    initialize convert process...
    read input file...
    read input file done.
    write output file...
    write output file done.

## Run Bayescan ##
    BayeScan2.1_linux64bits SNP.TRSdp5p05FHWEBS -nbp 30 -thin 20
    cp /home/BIO594/Exercises/Week_7and8/plot_R.r .

## Plot BayeScan ##
    source("plot_R.r")
    plot_bayescan("SNP.TRSdp5p05FH_fst.txt")

    $outliers
    [1]  39 220 221 473 474

    $nb_outliers
    [1] 5

    sed '40d;221d;222d;474d;475d' SNP.TRSdp5p05FH_fst.txt > neutral.txt


## VCF 2 Allele SNPs ##
    vcftools --vcf neutral.txt --max-alleles 2 --recode --recode-INFO-all --out neutralSNP.vcf
    VCFtools - 0.1.15

    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
	--vcf neutral.txt
	--recode-INFO-all
	--max-alleles 2
	--out SNP.neutral
	--recode

    After filtering, kept 0 out of 0 Individuals
    Outputting VCF file...
    After filtering, kept 922 out of a possible 922 Sites
    Run Time = 0.00 seconds

## PCA Adapt ##
    R
    > library(pcadapt)
    > filename <- read.pcadapt("SNP.neutral.recode.vcf", type = "vcf" )
    Error in vcfR::read.vcfR(input, verbose = FALSE) :
    File: SNP.neutral.recode.vcf does not appear to be a VCF file.
    First line of file:
    SNP.neutral.recode.vcf
    Should begin with:
    ##fileformat=VCFv

    (not sure why this is happening this is a definitely a vcf file)

## Neutral File ##
    /home/ehunter/week8/Filter/SNP.neutral.recode.vcf

# **Real Dataset** #

## Initial Filtering/dDocent ##
    ran dDocent
    ln -s ../TotalRawSNPs.vcf .

    vcftools --vcf TotalRawSNPs.vcf --max-missing 0.5 --maf 0.001 --minQ 20 --recode --recode-INFO-all --out TRS

    VCFtools - 0.1.14
    (C) Adam Auton and Anthony Marcketta 2009

    Parameters as interpreted:
	--vcf TotalRawSNPs.vcf
	--recode-INFO-all
	--maf 0.001
	--minQ 20
	--max-missing 0.5
	--out TRS
	--recode

    After filtering, kept 80 out of 80 Individuals
    Outputting VCF file...
    After filtering, kept 2973 out of a possible 2994 Sites
    Run Time = 1.00 seconds

## Bayescan ##
    java -jar /usr/local/bin/PGDSpider2-cli.jar -inputfile TotalRawSNPs.vcf -outputfile SNP.realdata -spid BSsnp.spid

    BayeScan2.1_linux64bits SNP.realdata -nbp 30 -thin 20
    R
    > source("plot_R.r")
    > plot_bayescan("SNP.real_fst.txt")
    $outliers
    [1] 1170 1172 1411

    $nb_outliers
    [1] 3

    java -jar /usr/local/bin/PGDSpider2-cli.jar -inputfile TotalRawSNPs.vcf -outputfile SNP.TRSdp5p05FHWEBayEnv.txt -spid SNPBayEnv.spid
    WARN  12:56:18 - PGDSpider configuration file not found! Loading default configuration.
    initialize convert process...
    read input file...
    read input file done.
    write output file...
    WARN  12:56:24 - Locus SNP_2114 was removed, as it is not polymorphic
    WARN  12:56:24 - Locus SNP_2258 was removed, as it is not polymorphic
    write output file done.

## BayEnv2 ##
    bayenv2 -i SNP.TRSdp5p05FHWEBayEnv.txt -p 4 -k 100000 -r 63479 > matrix.out
    tail -5 matrix.out | head -4 > matrix
    cp /home/BIO594/Exercises/Week_7and8/realdata/environ .
    cat environ

    calc_bf.sh SNP.TRSdp5p05FHWEBayEnv.txt environ matrix 4 10000 2

    ===== BAYENV2.0 =====

    input file is set
    environment file is set
    matrix is set
    number of iterations is set
    seed is set
    number of populations is set
    number of environmental variables is set
    TEST is set
    TEST = 1 . So running test at a SNP
    number of environmental variables 2

    MCMC VER 0.71 (THREADED)
    ITERATIONS = 10000
    INPUT FILE = snp_batchaaaaaaadno
    MATRIX FILE = matrix
    SEED = -29772

    ENVIRON FILE = environ
    reading environ
    num_alleles = 2.000000
    number of loci = 1
    (x 1000)

    paste <(seq 1 981) <(cut -f2,3 bf_environ.environ ) > bayenv.out
    cat <(echo -e "Locus\tBF1\tBF2") bayenv.out > bayenv.final

  ## R ##
    > table_bay <- read.table("bayenv.final",header=TRUE)
    Error in scan(file = file, what = what, sep = sep, quote = quote, dec = dec,  :
    line 982 did not have 3 elements
    > plot(table_bay$BF1)
    Error in plot(table_bay$BF1) : object 'table_bay' not found
    > table_bay[which(table_bay$BF1 > 100),]
    Error: object 'table_bay' not found

## Neutral File ##
    sed '1171d;1173d;1412d' SNP.real_fst.txt > neutral.txt
    /home/ehunter/week8/realdata/neutral.txt
