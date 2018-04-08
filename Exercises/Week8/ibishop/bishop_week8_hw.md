

# FIRST, the simulated data

### CALLING SNPs

```
#create new environment for this hw
conda create -n week7_8 ddocent

#activate new environment week7_8
source activate week7_8

#move to simulated directory
cd simulated/
x`
#run dDocent
dDocent

# 80 threads used
# 0G specified (used all available?)
# reads were trimmed
# de novo assembly built using CD-HIT
# PE reads specified
# cluster similarity default value used (0.9)
# reads were mapped
# no new BWA paramters
# FreeBayes used to call SNPs
# minimum allele frequency (within individual) set to 5
# minimum number of individuals required to have allele set to 3

```


### FILTERING SNPs

```
#make new subdirectory for filtering
mkdir Filter

#move into new directory
cd Filter/

#make symbolic link to dDocent output in parent directory
ln -s ../TotalRawSNPs.vcf .

#filter out loci with missing data, alleles with low freq, and alleles with low quality scores
vcftools --vcf TotalRawSNPs.vcf --max-missing 0.5 --maf 0.001 --minQ 20 --recode --recode-INFO-all --out TRS

#filter out loci with low depth
vcftools --vcf TRS.recode.vcf --minDP 5 --recode --recode-INFO-all --out TRSdp5

pop_missing_filter.sh TRSdp5.recode.vcf ../popmap 0.05 1 TRSdp5p05

#filter out loci with poor allelic balance, off kilter mapping quality ratios among alleles, etc.
dDocent_filters TRSdp5p05.recode.vcf TRSdp5p05

vcfallelicprimitives -k -g TRSdp5p05.FIL.recode.vcf |sed 's:\.|\.:\.\/\.:g' > TRSdp5p05F.prim

#remove indels
vcftools --vcf TRSdp5p05F.prim --recode --recode-INFO-all --remove-indels --out SNP.TRSdp5p05F

#filter via HWE
filter_hwe_by_pop.pl -v SNP.TRSdp5p05F.recode.vcf -p ../popmap -c 0.5 -out SNP.TRSdp5p05FHWE

#filter out low maf loci
vcftools --vcf SNP.TRSdp5p05FHWE.recode.vcf --maf 0.05 --recode --recode-INFO-all --out SNP.TRSdp5p05FHWEmaf05

#vcopy/rename final SNP vcf file for ease of use
SNP.TRSdp5p05FHWE.recode.vcf final_SNPs.vcf

#copy final vcf file to simulated directory
cp final_SNPs.vcf ..
```



### DETECT OUTLIERS VIA BAYESCAN

```
cd ..

#run PGDSpider
java -jar /usr/local/bin/PGDSpider2-cli.jar -inputfile final_SNPs.vcf -outputfile final_SNPs_BS -spid BSsnp.spid

#run BayeScan
BayeScan2.1_linux64bits final_SNPs_BS -nbp 30 -thin 20

cp /home/BIO594/DATA/Week7/example/plot_R.r .

#start R
R

#import r plotting file
source("plot_R.r")

#plot BayeScan Fst output
plot_bayescan("final_SNPs_BS_fst.txt")

#quit r
quit()
```


### DETECT OUTLIERS VIA PCAdapt

```
#keep loci with max of two alleles
vcftools --vcf Final.recode.vcf --max-alleles 2 --recode --recode-INFO-all --out Final.recode2A.vcf

#start R
R

#Load PCAdapt library
library(pcadapt)

#load our VCF file into R
filename <- read.pcadapt("F2A.vcf.recode.vcf", type = "vcf" )

#Create first PCA
x <- pcadapt(input = filename, K = 20)

#Plot Plot the likelihoods for only first 10 K
plot(x, option = "screeplot", K = 10)

#Create population designations
poplist.names <- c(rep("POPA", 20),rep("POPB", 20),rep("POPC", 20), rep("POPD",20))

#Plot the actual PCA (first two PCAs)
plot(x, option = "scores", pop = poplist.names)
#Plot PCA with PCA 2 and PCA 3
plot(x, option = "scores", i = 2, j = 3, pop = poplist.names)
#Plot PCA with PCA 3 and PCA 4
plot(x, option = "scores", i = 3, j = 4, pop = poplist.names)

#Redo PCA with only 3 K
x <- pcadapt(filename, K = 3)

#Start looking for outliers
#Make Manhattan Plot
plot(x , option = "manhattan")
#Make qqplot
plot(x, option = "qqplot", threshold = 0.1)
# Look at P-value distribution
plot(x, option = "stat.distribution")

# Set FDR
library(qvalue)
qval <- qvalue(x$pvalues)$qvalues
alpha <- 0.1

# Save outliers
outliers <- which(qval < alpha)

outliers
 [1]  411  412  433  434  435  436  437  438  439  440  441  856 1033 1035 1245
[16] 2102
```

### GENERATE NEUTRAL SNP DATASET

```
#remove outliers from VCF file based on what BayeScan and PCAdapt found

#based on outliers found with BayesScan
#split vcf into header and loci
grep '#' Final.recode.vcf > header.temp.vcf

#remove rows identified with BayeScan using sed
grep -v '#' Final.recode.vcf | sed -e '648d;649d' > Final.recode.filtered.loci.vcf

#reattach header, save output as neutral only SNP vcf
cat header_temp.vcf Final.recode.filtered.loci.vcf > Final.recode.neutral.vcf
```

### RUN PCA ON NEUTRAL SNPs

```
#add headers to popmap, done in nano, assign output to "strata2"

R

library(adegenet)
library(vcfR)

my_vcf <- read.vcfR("final_SNPs_neutral.vcf")
my_genind <- vcfR2genind(my_vcf)

strata<- read.table("strata2", header=TRUE)
strata_df <- data.frame(strata)
strata(my_genind) <- strata_df

setPop(my_genind) <- ~Population

#Test Population Structure
library("hierfstat")
fstat(my_genind)

matFst <- pairwise.fst(my_genind)



#PCA

X <- tab(my_genind, freq = TRUE, NA.method = "mean")
pca1 <- dudi.pca(X, scale = FALSE, scannf = FALSE, nf = 3)
barplot(pca1$eig[1:50], main = "PCA eigenvalues", col = heat.colors(50))
s.class(pca1$li, pop(my_genind))
title("PCA of simulated dataset\naxes 1-2")
add.scatter.eig(pca1$eig[1:20], 3,1,2)

col <- funky(15)
s.class(pca1$li, pop(my_genind),xax=1,yax=2, col=col, axesell=FALSE, cstar=0, cpoint=3, grid=FALSE)
```


### RUN DAPC ON NEUTRAL SNPs

```
grp <- find.clusters(my_genind, max.n.clust=40)
table(pop(my_genind), grp$grp)

table.value(table(pop(my_genind), grp$grp), col.lab=paste("inf", 1:2), row.lab=paste("ori", 1:4))

dapc1 <- dapc(my_genind, grp$grp)
scatter(dapc1,col=col,bg="white", solid=1)

contrib <- loadingplot(dapc1$var.contr, axis=1, thres=.01, lab.jitter=1)
contrib
```



# REAL DATASET

### BAYESCAN

```
#convert vcf using pgdspider
java -jar /usr/local/bin/PGDSpider2-cli.jar -inputfile SNP.DP3g98maf01_85INDoutFIL.NO2a.HWE.FIL.recode.vcf -outputfile final_SNPs_BS -spid BSsnp.spid

#run BayeScan
BayeScan2.1_linux64bits final_SNPs_BS -nbp 30 -thin 20

R

source("plot_R.r")

plot_bayescan("final_SNPs_BS_fst.txt")

#no outliers found

```





### BayEnv2

```
java -jar /usr/local/bin/PGDSpider2-cli.jar -inputfile SNP.DP3g98maf01_85INDoutFIL.NO2a.HWE.FIL.recode.vcf -outputfile SNP.BayEnv.txt -spid SNPBayEnv.spid

bayenv2 -i SNP.BayEnv.txt -p 4 -k 100000 -r 63479 > matrix.out

tail -5 matrix.out | head -4 > matrix

#check structure of environ
cat environ
```
##### This step doesn't seem to work for me. Didn't get any BayEnv2 output
```
calc_bf.sh SNP.BayEnv.txt environ matrix 4 10000 2
```


### PCA

```
#no outliers found, so we didn't filter out any more loci

#add headers to popmap ---> strata

R

library(adegenet)
library(vcfR)

my_vcf <- read.vcfR("SNP.DP3g98maf01_85INDoutFIL.NO2a.HWE.FIL.recode2.vcf")
my_genind <- vcfR2genind(my_vcf)

strata<- read.table("strata2", header=TRUE)
strata_df <- data.frame(strata)
strata(my_genind) <- strata_df

setPop(my_genind) <- ~Population

#Test Population Structure
library("hierfstat")
fstat(my_genind)

matFst <- pairwise.fst(my_genind)


#PCA

X <- tab(my_genind, freq = TRUE, NA.method = "mean")
pca1 <- dudi.pca(X, scale = FALSE, scannf = FALSE, nf = 3)
barplot(pca1$eig[1:50], main = "PCA eigenvalues", col = heat.colors(50))
s.class(pca1$li, pop(my_genind))
title("PCA of simulated dataset\naxes 1-2")
add.scatter.eig(pca1$eig[1:20], 3,1,2)

col <- funky(15)

s.class(pca1$li, pop(my_genind),xax=1,yax=2, col=col, axesell=FALSE, cstar=0, cpoint=3, grid=FALSE)
```

### DAPC

```
grp <- find.clusters(my_genind, max.n.clust=40)
table(pop(my_genind), grp$grp)

table.value(table(pop(my_genind), grp$grp), col.lab=paste("inf", 1:2), row.lab=paste("ori", 1:16))

dapc1 <- dapc(my_genind, grp$grp)
scatter(dapc1,col=col,bg="white", solid=1)

contrib <- loadingplot(dapc1$var.contr, axis=1, thres=.01, lab.jitter=1)
contrib
```
