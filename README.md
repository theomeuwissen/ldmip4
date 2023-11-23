# _lamip_ 
lamip performes multilocus iterative peeling of SNP  marker data (previously ldmip4). 
SNPs can be treated independently or linked.
In case of linked paternal/maternal segregation probabilities are calculated.
the peeling can be performed in parallel by several threads.
A linkage analysis based G matrix (GLA) can be calculated following Fernando & Grossman 1989 based on the resulting lamip.s file.
Computational costs for GLA are high, but can be reduced by parallel computation 

Input files:
lamip.inp (see this file for more details on usage)

lamip.ped (pedigree file with 4 columns: IDindiv IDsire IDdam; IDs are sorted from old to young and (re)numbered: 1,2,3,4...)
(negative IDsire or IDdam denotes genetic groups, whose SNP allele-frequencies are seperately estimated)

ldmip4.mrk  (marker genotype file. 2 lines per genotyped individual: IDindiv allele SNP1 alleleSNP2; nextline: IDindiv 2ndallele SNP1 2ndalleleSNP2...
(note lamip.mrk may be replaced by plink.ped (using 12-coding in PLINK)


Usage: ./lamip




