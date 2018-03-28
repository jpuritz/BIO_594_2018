library(adegenet)
library(vcfR)


my_vcf <- read.vcfR("SNPs.vcf")


my_genind <- vcfR2genind(my_vcf)


strata<- read.table("strata", header=TRUE)
strata_df <- data.frame(strata)
strata(my_genind) <- strata_df

setPop(my_genind) <- ~Population


#PCA

X <- tab(my_genind, freq = TRUE, NA.method = "mean")
pca1 <- dudi.pca(X, scale = FALSE, scannf = FALSE, nf = 3)
col <- funky(15) 
s.class(pca1$li, pop(my_genind),xax=1,yax=2, col=col, axesell=FALSE, cstar=0, cpoint=3, grid=FALSE)
