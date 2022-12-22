---
layout: post
title:  "SNP data for the spring tetraploid x hexaploid NAM population"
date:   2022-12-21 16:59:00 +0000
categories: jekyll update
---

# Summary 

This page contains links to the full 35k breeders' array genotype data for the NIAB spring tetraploid x hexaploid wheat (tet hex) Nested Association Mapping (NAM) population. The data consists of 35,143 markers and 1,983 genotypes (including individuals and parents). There are 59 nested populations, each formed through backcrossing a different tetraploid donor with the recurrent parent Paragon. The genotyping array was the Breeders' 35K Axiom® array (Affymetrix product ID 550524) and the genotyping was carried out at the [University of Bristol](https://www.bristol.ac.uk/), the DNA extraction and SNP calling was completed at NIAB. All work was funded by the Biotechnology and Biological Sciences Research Council (BBSRC) Cross-Institute Strategic Programme ‘Designing Future Wheat’ BB/P016855/1.

# Data Download

The data can be downloaded [here](https://github.com/NIAB/niab-dfw-wp3/raw/main/data/niab.spring.thex.nam.zip). The zip folder includes the following files:

- `full.markers.spring.thex.nam.v1.csv` the dataset with NIAB codes.


- **WILL CONTAIN SOON** `GRUvs.NIAB.code.conversion.csv` a conversion file to link up the Academic and Breeders' toolkit lines with the NIAB codes. See [here](https://designingfuturewheat.org.uk/work-package-3/) for more info on these toolkits. 
- `pedigree.for.spring.thex.nam.csv` a file with information on the pedigree of the 59 nested populations.

# Information on data
 
 The genotype QC in the axiom software was completed with QC thresholds of DQC = 0.8 and a QC call rate = 90%. An inbred penalty of 4 and a cr-cut off of 96 were used in the SNP calling. The data is in numeric format and was converted from the original axiom call codes format (AA, AB, BB and NoCall) using the following conversion:

`"NoCall" = NA`
`"AA" = 0`
`"AB" = 1`
`"BB" = 2`

The marker calls for all 35,143 SNPs are included. The last 25 columns of the data contain SNP metrics outputted from the axiom software. 

The data includes NAM individuals, tetraploid parents and a number of Paragon replicates in the following number:

| Line Type          | Count |
|--------------------|-------|
| NAM individuals    | 1784  |
| SHW parents        | 186   |
| Paragon replicates | 11    |
| Robigus replicates | 2     |


The NAM population contains 59 nested populations, backcrossed into Paragon and each with a different tetraploid donor. Each NAM individual's name starts with a population code (e.g. `THEX002_x_x_x`). The below table shows the pedigree and information of genotypes in the data: 

| **Population Code** | **No. of Genotypes** | **Founder of Population** | **Recurrent Parent** |
|---------------------|----------------------|---------------------------|----------------------|
| THEX002             | 4                    | tios                      | Paragon              |
| THEX003             | 34                   | em27996                   | Paragon              |
| THEX010             | 46                   | em14078                   | Paragon              |
| THEX011             | 24                   | em14235                   | Paragon              |
| THEX012             | 24                   | em16608                   | Paragon              |
| THEX013             | 22                   | em17202                   | Paragon              |
| THEX014             | 12                   | em18083                   | Paragon              |
| THEX015             | 36                   | em18209                   | Paragon              |
| THEX016             | 22                   | em18210                   | Paragon              |
| THEX018             | 34                   | dic012a                   | Paragon              |
| THEX019             | 14                   | dic012b                   | Paragon              |
| THEX020             | 122                  | dic016a                   | Paragon              |
| THEX021             | 36                   | dic016b                   | Paragon              |
| THEX022             | 5                    | dic034                    | Paragon              |
| THEX023             | 12                   | dic036                    | Paragon              |
| THEX024             | 37                   | dic045                    | Paragon              |
| THEX031             | 3                    | dic071                    | Paragon              |
| THEX032             | 16                   | dic072                    | Paragon              |
| THEX033             | 17                   | dic082                    | Paragon              |
| THEX035             | 14                   | dic094                    | Paragon              |
| THEX036             | 53                   | dic096                    | Paragon              |
| THEX038             | 13                   | dic107                    | Paragon              |
| THEX041             | 14                   | dic120                    | Paragon              |
| THEX043             | 9                    | dic130                    | Paragon              |
| THEX044             | 18                   | dic143                    | Paragon              |
| THEX046             | 19                   | dic147                    | Paragon              |
| THEX047             | 22                   | dic199                    | Paragon              |
| THEX090             | 36                   | du030_1                   | Paragon              |
| THEX092             | 57                   | du067_1                   | Paragon              |
| THEX094             | 50                   | du088_2                   | Paragon              |
| THEX096             | 74                   | ardente                   | Paragon              |
| THEX100             | 63                   | claudio                   | Paragon              |
| THEX101             | 44                   | croc1                     | Paragon              |
| THEX102             | 38                   | cultur                    | Paragon              |
| THEX104             | 44                   | exceldur                  | Paragon              |
| THEX105             | 13                   | hoh501                    | Paragon              |
| THEX106             | 47                   | hoh506                    | Paragon              |
| THEX108             | 55                   | karim                     | Paragon              |
| THEX109             | 57                   | lloyd                     | Paragon              |
| THEX110             | 21                   | miradoux                  | Paragon              |
| THEX113             | 70                   | pescodou                  | Paragon              |
| THEX114             | 14                   | sculptur                  | Paragon              |
| THEX117             | 37                   | cudic24                   | Paragon              |
| THEX145             | 27                   | acalou                    | Paragon              |
| THEX148             | 20                   | dic115                    | Paragon              |
| THEX149             | 52                   | dic145                    | Paragon              |
| THEX150             | 11                   | dic051                    | Paragon              |
| THEX190             | 10                   | dic056                    | Paragon              |
| THEX191             | 24                   | dic065                    | Paragon              |
| THEX193             | 1                    | dic087                    | Paragon              |
| THEX195             | 19                   | dic121                    | Paragon              |
| THEX196             | 37                   | du057_1                   | Paragon              |
| THEX197             | 18                   | dakter                    | Paragon              |
| THEX198             | 25                   | langdon                   | Paragon              |
| THEX212             | 63                   | cudic16                   | Paragon              |
| THEX213             | 26                   | capelli                   | Paragon              |
| THEX214             | 28                   | hoh-501                   | Paragon              |
| THEX224             | 21                   | biensur                   | Paragon              |

# Contact 

For queries on the data and usage please contact:

- fiona.leigh@NIAB.com bethany.love@NIAB.com and tally.wright@NIAB.com 

![](/niab-dfw-wp3/image/tet-parents.png)

