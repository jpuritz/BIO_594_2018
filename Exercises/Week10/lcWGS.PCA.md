#  PCA and MDS for NGS

Exercise created by [Anders Albrechtsen](http://www.popgen.dk/groupWiki/index.php/Anders_Albrechtsen)

## Small intro with known genotypes

First lets input the genotype into R. First open R by typing 'R' in the command line:
 
```R
G <-matrix(c(1,0,2,0,2,0,2,1,1,1,0,1,0,2,1,2,1,1,1,1,1,0,1,0,2,0,1,1,0,2,1,2,0,1,0),5,by=T)
nInd <- nrow(G)

print(G)

## don't close R

```

 - Identify the rows and the columns. Does each row contain the genotypes of a site or an individual? And what about each column?

Let's try to do MDS. First let's calculate the distance. The simple distance measure as seen in the slides is called a Manhatten distance.
 
```R

## continue in R

D<-dist(G,upper=T,diag=T,method="manha")
D

## don't close R

```

-  How many dimensions are used to represent the distances?
 
Then reduce the dimension to 2 dimensions using MDS and plot the results:

```R
 ## continue in R	
 
 #perform MDS to 2 dimensions
 k2 <- cmdscale(D,k=2)
 print(k2)
 
 #plot the results
 
 plot(k2,pch=16,cex=3,col=1:5+1,ylab="distance 2th dimension",xlab="distance 1.  dimension",main="Multiple dimension scaling (MDS)")
 points(k2,pch=as.character(1:5))
 
 ## don't close R
```

If you cannot view the figure then you can find it [here](http://popgen.dk/albrecht/open/bgi/mds.pdf).


 - Can you find a example of where the 2 dimensional representation does not capture the true pairwise distances?


First lets try to perform PCA directy on the normalized genotypes without calculating the covariance matrix

 - Why do we normalize the genotypes?
 
```R
 ## continue in R

 #first normalize the data do that the mean and variance is the same for each SNP
  
 normalize <- function(x){
    nInd <- nrow(x)
    avg <- colMeans(x)
    M <- x - rep(colMeans(x),each=nInd)
    M <- M/sqrt(2*rep(avg/2*(1-avg/2),each=nInd))
    M
 }
 M <- normalize(G)

 svd <- svd(M)
 ## print the decomposition for M=SDV
 ## u is the eigenvectors
 ## d is eigen values  

 print(svd)

##make a diagonal matrix with the eigenvalues 
SIGMA <- matrix(0,nInd,nInd)
diag(SIGMA) <- svd$d 

## using the matrixes from the decomposition we can undo the transformation of our normalized genotypes
M2 <- svd$u%*%SIGMA%*%t(svd$v)
print(M)
print(M2)

## don't close R
```

 - Did the reconstruction of the normalized genotypes work?
 - Would you be able to reconstruct the unnormalized (raw) genotypes?

Now try performing PCA based on the covariance matrix instead:

```R
 ## continue in R



 ## calculate the covariance matrix
 C <- M %*% t(M)
 print(C)
 

 ## then perform the PCA by singular value decomposition
 e <- eigen(C)	 

 ## print first PC
 print(e$vectors[,1])
 
 ##plot 2 first PC. for the 5 indiviudals
  X11() #open new plot
 plot(e$vectors[,1:2],pch=16,cex=3,col=1:5+1,ylab="2. PC",xlab="1. PC",main="Principle component analysis (PCA)")
 points(e$vectors[,1:2],pch=as.character(1:5))
 ## don't close R
```

If you cannot view the figure then you can find it [here](http://popgen.dk/albrecht/open/bgi/pca.pdf).
 - Did you get the same results using the covariance matrix as using the normalized genotypes directly?
 - What does negative values in the covariance matrix mean?
 - Compare the two plots (MDS vs. PCA)? 

Bonus information:

Unlike MDS, PCA will not remove information so you are actually able to reconstruct your covariance matrix from the principal components

```R
##continue in R
##make a diagonal matrix with the eigenvalues 
SIGMA <- matrix(0,nInd,nInd)
diag(SIGMA) <- e$value

## transform the PC back to the original data
## using matrix multiplication V SIGMA Vt
out <- e$vectors %*% SIGMA %*% t(e$vectors)
print(out)
print(C)
#close R after you are done
```
 


## PCA/MDS for real data

### Setup data and environment

First, we need to create and load a ANGSD bioconda environment:
```
conda create -n ANGSD angsd
source activate ANGSD

mkdir Week10
cd Week10
ln -s /home/BIO594/Exercises/Week_10/data/* .

ls *.bam > all.files


Get the IBS and covariance matrix from the NGS data. 
```
angsd -bam all.files -minMapQ 30 -minQ 20 -GL 2 -out all -doMajorMinor 1 -doMaf 1 -SNP_pval 2e-6 -minInd 25  -doIBS 1 -doCounts 1 -doCov 1 -makeMatrix 1 -minMaf 0.05 -P 5
```


## Multidimensional scaling (MDS)

Lets try to look at our estimate IBS matrix that was created from the first angsd command.

#### Do in R

```R
#read in the names of each individual
s<-strsplit(basename(scan("all.files",what="theHeck")),"\\.")
pop<-as.factor(sapply(s,function(x)x[5]))

#name of the ibsMatrix file
name <- "all.ibsMat"
m <- as.matrix(read.table(name))

#do the MDS analysis on the IBS matrix
mds <- cmdscale(as.dist(m))

#plot the results colored by population
plot(mds,lwd=2,ylab="Dist",xlab="Dist",main="multidimensional scaling",col=pop)
legend("center",levels(pop),fill=1:3)
```

If you cannot view the figure then you can find it [here](http://popgen.dk/albrecht/open/bgi/all.mds.pdf).

 - Based on the plot which two populations are closest and this population is most distant?
 - Does it make sense that the YRI population form the most distant cluster?


## Principal component analysis (PCA)

Similarly to the MDS analysis above, now try to do a PCA analysis based on the covarience matrix:

```
#in R
s<-strsplit(basename(scan("all.files",what="theHeck")),"\\.")
pop<-sapply(s,function(x)x[5])

name <- "all.covMat"
m <- as.matrix(read.table(name))

#get the eigen vectors
e <- eigen(m)

#plot the two first eigen vectors
plot(e$vectors[,1:2],lwd=2,ylab="PC 2",xlab="PC 2",main="Principal components",col=as.factor(pop),pch=16);legend("top",fill=1:3,levels(as.factor(pop)))
```

If you cannot view the figure then you can find it [here](http://popgen.dk/albrecht/open/bgi/all.pca.pdf).


The plots are some what noisy. If you had used the whole genome it would have looked like this [plot](http://popgen.dk/angsd/images/thumb/0/06/PCA_MDS.png/800px-PCA_MDS.png).

# fastNGSadmix for PCA

We will try to use an genotype likelihood appoach with admixture aware priors using fastNGSadmix

```
# Set path for the fastNGSadmixPCA program.  fastNGSadmix is already installed on KITT

fastNGSadmixPCA=/home/BIO594/Exercises/Week_10/fastNGSadmixPCA.R

# Set path for all input files you will use in this exercise
inputpath=/home/BIO594/Exercises/Week_10/admix_data/

## genotypes of reference panel
refGeno=/home/BIO594/Exercises/Week_10/admix_data/ref_panel/humanOrigins_7worldPops



```

We will use this  reference panel:

|Code| Population of Origin|
|---|-----|
|French     | French individuals |
|Han        | Chinese individuals |
|Chukchi    | Siberian individuals |
|Karitiana  | Native American individuals |
|Papuan     | individuals from Papua New Guinea, Melanesia |
|Sindhi     | individuals from India |
|YRI        | Yoruba individuals from Nigeria |


And we will also use the same individual as last time namely the two karitiana individuals sample2 and sample3.

First rerun fastNGSadmix to get the admixture proportions, which we will use as admixture aware priors in the PCA analysis

```
# Analyse sample2
$fastNGSadmix -likes ${inputpath}/sample2.beagle.gz -fname ${inputpath}/refPanel.txt -Nname ${inputpath}/nInd.txt -outfiles sample2 -whichPops all

# Analyse sample3
$fastNGSadmix -likes ${inputpath}/sample3.beagle.gz -fname ${inputpath}/refPanel.txt -Nname ${inputpath}/nInd.txt -outfiles sample3 -whichPops all
```

Both qopt files should indicate that the sample is 100% Karitiana. We will add our sample to the  genotypes of our reference panel can perform PCA using the genotype likelihoods and admixture aware priors for the NGS sample


First lets look a sample 2.
 - How many sites did that sample have?
```
Rscript $fastNGSadmixPCA -likes ${inputpath}/sample2.beagle.gz -qopt sample2.qopt -ref $refGeno -out sample2
## -likes: is the genotype likelihoods of the NGS sample
## -qopt: the estimate admixture proportions we will use as prior
## -geno: genotypes of the reference panel
## -out: output name (prefix)
```


 - what information does the program spit out?

View the PCA plot by typing:
```
 evince sample2_PCAplot.pdf

```

Your sample is shown as the X

 - Does the sample fall where you would expect?

Let's try to see what the prior looks like.

I told you that you could use the results of admixture analysis to generate a PCA plot. This be done by removing all information from the NGS data. Let's try to set all genotype likelihoods to 0.33: 

```
zcat ${inputpath}/sample2.beagle.gz | sed 's/\(^.*\t.*\t.*\)\t.*\t.*\t.*$/\1\t0.33\t0.33\t0.33/g' | gzip -c > noInfo.beagle.gz
```

Try to view the new beagle file using for example less:
```
less noInfo.beagle.gz
```


Now let's estimate the PCA based on the uninformative beagle file. This will show you where the prior will be placed in the PCA.

```
Rscript $fastNGSadmixPCA -likes noInfo.beagle.gz -qopt sample2.qopt  -ref $refGeno -out noInfo
```

view the output plot called noInfo_PCAplot.pdf

```
 evince noInfo_PCAplot.pdf
```

The non-informative prior was set to 0.33 for each genotype. Try to modify the above script and change the value 0.33 to something else. Then perform the PCA one more time

 - Does the PCA change?
 - Why is the value not important?


When we use a prior we want to make sure that it does not dominate the results. We want our NGS data to add information. Lets look at the sample with ultra low depth called sample3.
- How many informative site with reads did this sample have?

The sample only has a single read at each informative sites out of a posible 442769 sites in the reference panel.

 - What is the average depth of the sample?


Run the PCA for the low depth sample:

```
Rscript $fastNGSadmixPCA -likes ${inputpath}/sample3.beagle.gz -qopt sample3.qopt  -ref $refGeno -out sample3

## view the results
evince sample3_PCAplot.pdf
```

 - Does this sample fall just as nicely as the other Karitiana sample?
 - Does is fall in the same place as the prior?


# admixture aware priors without estimated admixture proportions

Let's try to perform PCA analysis on the large 1000 genotype genotype likelihoods that you performed admixture analysis on yesterday.
First let set the path to program and the input file
```
# NB this must be done every time you open a new terminal
AA=/home/albrecht/PhDCourse

## PCAngsd
PCAngsd=$AA/prog/pcangsd/pcangsd.py

## beagle genotype likelihood file
GL1000Genomes=$AA/admixture/data/input.gz

## copy population information file to current folder
cp $AA/admixture/data/pop.info .

```


 - What were the populations included? And how many sites?

```
python $PCAngsd -beagle $GL1000Genomes -o input -n 100
```

The program estimates the covariance matrix that can then be used for PCA. look at the output from the program

 - How many significant PCA (see MAP test in output)?

Plot the results in R 

```
#open R
pop<-read.table("pop.info")

C <- as.matrix(read.table("input.cov"))
 e <- eigen(C)
pdf("PCAngsd.pdf")
plot(e$vectors[,1:2],col=pop[,1],xlab="PC1",ylab="PC2")
legend("top",fill=1:5,levels(pop[,1]))
dev.off()
## close R
```

view the results with

```

evince PCAngsd.pdf
```




Compare with the estimate admixture proportions
 http://randy.popgen.dk/popgen17/pass/exercises/admixexercisefiles/plots/BestK3.png

 - In the PCA plot can you identify the Mexicans with only European ancestry?
 - What about the African American with East Asian ancestry?
 - Based on the PCA would you have the same conclusion as the admixture proportions?

Try the same analysis but without estimating individual allele frequencies. This is the same as using the first iteration of the algorithm

```
python $PCAngsd -beagle $GL1000Genomes -o input2 -iter 0 -n 100
```

Plot the results in R
```
#open R
pop<-read.table("pop.info")

C <- as.matrix(read.table("input2.cov"))
 e <- eigen(C)
pdf("PCAngsd2.pdf")
plot(e$vectors[,1:2],col=pop[,1],xlab="PC1",ylab="PC2",main="joint allele frequency")
legend("top",fill=1:5,levels(pop[,1]))
dev.off()
## close R
```

View plot:

```
evince PCAngsd2.pdf
```


 - Do you see any difference?
 - Would any of your conclusions change? (compared to the previous PCA plot)




Let try to use the PCA to infer admixture proportions based on the first 2 principal components. For the optimization we will use a small penalty on the admixture proportions (alpha).
```
 python $PCAngsd -beagle $GL1000Genomes -o input -n 100 -admix -admix_alpha 50
```

Plot the results in R
```
#open R
pop<-read.table("pop.info",as.is=T)
q<-read.table("input.K3.a50.0.qopt")

## order according to population
ord<-order(pop[,1])
barplot(t(q)[,ord],col=2:10,space=0,border=NA,xlab="Individuals",ylab="Admixture proportions")
text(tapply(1:nrow(pop),pop[ord,1],mean),-0.05,unique(pop[ord,1]),xpd=T)
abline(v=cumsum(sapply(unique(pop[ord,1]),function(x){sum(pop[ord,1]==x)})),col=1,lwd=1.2)
    
## close R
```
 - how does this compare to the NGSadmix analysis?




## Inbreeding in the admixed individuals

Inbreeding in admixed samples is usually not possible to estimate using standard approaches. 
Let's try to estimate the inbreeding coefficient of the samples using the average allele frequency

```
python $PCAngsd -beagle $GL1000Genomes -o IB0 -inbreed 2 -n 100 -iter 0
```


join names and results, sort the values and look at the results
```
paste pop.info IB0.inbreed | LC_ALL=C sort -k3g
``` 
The third column is an estimate of the inbreeding coefficient (allowing for negative)

 - Does any of the individuals look more inbreed than an offspring of a pair of first cousins  ?
 - how do you interpret negative values?
 - The results will be affected by population structure - Why?
 - see any pattern of which individuals have low (negative) and high inbreeding coefficients? - can you explain the pattern?

Now let's try to estimate the inbreeding coefficient of the samples by using the individual allele frequencies predicted by the PCA

```
python $PCAngsd -beagle $GL1000Genomes -o IB -inbreed 2 -n 100 
```


join names and results, sort the values and look at the results
```
paste pop.info IB.inbreed | LC_ALL=C sort -k3g
``` 

 - Does any of the individual look inbreed?

# PCangsd and selection

For very resent selection we can look within closely related individuals for example with in Europeans

```

## copy positions and sample information 
cp $AA/PCangsd/data/eu1000g.sample.Info .

#set pa
EU1000=$AA/PCangsd/data/eu1000g.small.beagle.gz
wc eu1000g.sample.Info
N=424 #one line for header
```


Run PCangsd with to estimate the covariance matrix while jointly estimating the individuals allele frequencies


```
python $PCAngsd -beagle $EU1000 -o EUsmall -n $N -threads 20
```

Plot the results in R

```
## R
 cov <- as.matrix(read.table("EUsmall.cov"))

 e<-eigen(cov)
 ID<-read.table("eu1000g.sample.Info",head=T)
 plot(e$vectors[,1:2],col=ID$POP)
 
 legend("topleft",fill=1:4,levels(ID$POP))
```


- Does the plot look like you expected?


Since the European individuals in 1000G are not simple homogeneous disjoint populations it is hard to use PBS/FST or similar statistics to infer selection based on populating differences. However, PCA offers a good description of the differences between individuals which out having the define disjoint groups.

Now let try to use the PC to infer selection along the genome based on the PCA

```
python $PCAngsd -beagle $EU1000 -o EUsmall -n $N -selection 1 -sites_save
```

plot the results

```
## function for QQplot
qqchi<-function(x,...){
lambda<-round(median(x)/qchisq(0.5,1),2)
  qqplot(qchisq((1:length(x)-0.5)/(length(x)),1),x,ylab="Observed",xlab="Expected",...);abline(0,1,col=2,lwd=2)
legend("topleft",paste("lambda=",lambda))
}

### read in seleciton statistics (chi2 distributed)
s<-scan("EUsmall.selection.gz")
## make QQ plot to QC the test statistics
qqchi(s)

# convert test statistic to p-value
pval<-1-pchisq(s,1)

## read positions (hg38)
p<-read.table("EUsmall.sites",colC=c("factor","integer"),sep="_")

names(p)<-c("chr","pos")

## make manhatten plot
plot(-log10(pval),col=p$chr,xlab="Chromosomes",main="Manhatten plot")

## zoom into region 
 w<-range(which(pval<1e-7)) + c(-100,100)
 keep<-w[1]:w[2]
 plot(p$pos[keep],-log10(pval[keep]),col=p$chr[keep],xlab="HG38 Position chr2")

## see the position of the most significant SNP 
 p$pos[which.max(s)]
```

see if you can make sense of the top hit based on the genome.
- Look in [[http://genome.ucsc.edu/cgi-bin/hgGateway][UCSC browser]]
- Choose human GRCh38/hg38
- search for the position of the top hit and identify the genes at that loci



