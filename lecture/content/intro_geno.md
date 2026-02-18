## 2. INSTRUCTIONS FOR GENOTYPES & IMPUTATION

###General genotype properties
Genotypes must be obtained from micro-array chips that ensure genome-wide coverage (i.e., > ~200,000 genome-wide SNPs). The genotypes must be in build 37/hg19 and on the forward strand. If you are unsure which strand your genotypes are on this website can help you: https://www.well.ox.ac.uk/%7Ewrayner/strand/. If you have multiple arrays in the same study, make sure you merge the datasets prior to imputation and make sure that you include the different arrays as covariates in the GWAS analysis as dummy variables. 

### Pre-imputation Quality Control (QC) 
We assume that your genotypes have been extensively QCed. Typically, GWAS studies exclude SNPs from further analysis (or imputation) with:
•	Minor allele frequency <1% 
•	Call rate <95% or <99%
•	HWE p < 1e-6
•	Known to have evidence of poor clustering on visual inspection of intensity plots

### GWAS studies also remove subjects with:
•	Low overall call rates (< 95%)
•	Excess autosomal heterozygosity or homozygosity (indicating genotyping errors or excessive inbreeding), usually with F < -.1 or F > .1 (see http://zzz.bwh.harvard.edu/plink/ibdibs.shtml#inbreeding for more info on the inbreeding coefficient F)
•	Duplicate samples
•	Unintended 1st or 2nd degree relatives in case of a sample of unrelated individuals
•	Wrong gender (excessive X-chromosome homozygosity in males)
•	Chromosome abnormalities, such as XXY’s, etc.
