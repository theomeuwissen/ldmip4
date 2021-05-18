# _ldmip4_ 
ldmip4 performes multilocus iterative peeling of SNP  marker data. 
SNPs can be treated independently or linked.
In case of linked paternal/maternal segregation probabilities are calculated.
in case of unlinked SNPs the peeling can be performed in parallel by several threads.
A linkage analysis based G matrix (GLA) can be calculated following Fernando & Grossman 1989 (only when assuming the SNPs linked).
Computational costs for GLA are high, but can be reduced by parallel computation 
This may substantially increase memory requirements as several GLA matrices are calculated simultaneously.

Input files:
ldmip4.inp (see this file for more details on usage)

ldmip4.ped (pedigree file with 4 columns: IDindiv IDsire IDdam; IDs are sorted from old to young and (re)numbered: 1,2,3,4...)
(negative IDsire or IDdam denotes genetic groups, whose SNP allele-frequencies are seperately estimated)

ldmip4.mrk  (marker genotype file. 2 lines per genotyped individual: IDindiv allele SNP1 alleleSNP2; nextline: IDindiv 2ndallele SNP1 2ndalleleSNP2...


Usage: ./ldmip4


# _Report problems to theo.meuwissen@nmbu.no. Do not distribute ldmip4 without written consent of the author._ 

