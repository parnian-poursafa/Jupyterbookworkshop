#1. INSTRUCTIONS FOR SUBJECT INCLUSION, PHENOTYPES & COVARIATES

###Inclusion
We propose to perform analyses on homogeneous groups of subjects with the same ancestry  (based on genetic principal components). If you have multiple ancestries within your dataset, please separate them and run separate GWASs for each ancestral group. Only include subjects who have used cannabis at least once during their lifetime in the analyses. Subjects who have never used cannabis should be excluded from the analyses. 

###Phenotypes
Please refer to the instructions sent to your group (see Instructions on how to analyse the phenotype.docx)

###Covariates
Please use these variables as a covariate in your GWAS analysis:

-	Age at the time of the phenotypic assessment (in years since birth).

-	Sex coded as 1=male, 2=female (to be used in the analysis including both males and females).

-	Birth cohort To correct for cohort effects please recode year of birth to groups spanning 20 year-periods. Make a dummy variable for each of 20-year cohort except for the reference group. The lowest birth cohort is the reference group. For example, if the birth range in your cohort is 1940 to 1992, please make 3 birth cohorts: 1940-1959, 1960-1979 and 1980-2000. The lowest birth cohort (1940-1959) is the reference group. Two dummy variables are required: 
-	BirthCohortDummyA is ‘1’ if the subject is born in 1960-1979 and ‘0’ otherwise.
-	BirthCohortDummyB is ‘1’ if the subject is born in 1980-2000 and ‘0’ otherwise.
Include the dummy variables as covariates in the GWAS analyses.

-	Micro-array chips: if your genotyping includes multiple micro-array platforms, include the micro-array as a covariate using dummy variables. For example, if your samples have been genotyped on two platforms, include one dummy variable (platform 1=0; platform 2=1) as a covariate. If your samples have been genotyped on three platforms, please include two dummy variables (platform 1 = 0/0; platform 2=0/1; platform 3=1/1).  

-	Population structure: please correct for population structure by including genetic PCs as covariates (include 20 PCs or the number of PCs that is suitable for your sample). 

-	If necessary, add study-specific covariates, e.g., site or batch effects.
