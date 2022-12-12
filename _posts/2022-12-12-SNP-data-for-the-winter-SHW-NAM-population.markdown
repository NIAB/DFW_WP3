---
layout: post
title:  "SNP data for the winter SHW NAM population"
date:   2022-12-12 10:43:05 +0000
categories: jekyll update
---

# Summary 

This page contains links to the full 35k breeders' array genotype data for the NIAB winter Synthetic Hexaploid Wheat (SHW) Nested Association Mapping (NAM) population. The data consists of 35,143 markers and 3,295 genotypes (including individuals and parents). There are 55 nested populations, each formed through backcrossing a different primary SHW with the recurrent parent Robigus. The genotyping array was the Breeders' 35K Axiom® array (Affymetrix product ID 550524) and the genotyping was carried out at the [University of Bristol](https://www.bristol.ac.uk/), the DNA extraction and SNP calling was completed at NIAB. All work was funded by the Biotechnology and Biological Sciences Research Council (BBSRC) Cross-Institute Strategic Programme ‘Designing Future Wheat’ BB/P016855/1.

# Data Download

The data can be downloaded [here](/_data/niab.winter.shw.nam.zip). The zip folder includeds the following files:

- `full.markers.winter.shw.nam.v1.csv` the dataset with NIAB codes.
- `GRUvs.NIAB.code.conversion.csv` a conversion file to link up the Achedmic and Breeders' toolkit lines with the NIAB codes. See [here](https://designingfuturewheat.org.uk/work-package-3/) for more info on these toolkits. 
- `pedigree.for.winter.shw.nam.csv` a file with information on the pedigree of the 55 nested populations.

 # Information on data
 
 The genotype QC in the axiom software was completed with QC thresholds of DQC = 0.8 and a QC call rate = 90%. An inbred penalty of 4 and a cr-cut off of 96 were used in the SNP calling. The data is in numeric format and was converted from the original axiom call codes format (AA, AB, BB and NoCall) using the following conversion:

`"NoCall" = NA`
`"AA" = 0`
`"AB" = 1`
`"BB" = 2`

The marker calls for all 35,143 SNPs are included. The last 25 columns of the data contain SNP metrics outputted from the axiom software. 

The data includes NAM individuals, SHW parents and a number of Robigus replicates in the following number:

 | Line Type  | Count |
| ------------- | ------------- |
| NAM individuals  | 3137  |
| SHW parents  | 126  |
| Robigus replicates  | 32  |


The NAM population contains 55 nested populations, backcrossed into Robigus and each with a different primary SHW donor. Each NAM individual's name starts with a population code (e.g. `NIAB.SHW.BC.489.x.x.x.x`). The below table shows the pedigree and information of genotypes in the data: 

| **Population Code** | **No. of Genotypes** | **Founder of Population** | **Recurrent Parent** |
|---------------------|----------------------|---------------------------|----------------------|
| 38/39               | 86                   | NIAB.SHW.008              | Robigus              |
| 42/45               | 61                   | NIAB.SHW.012              | Robigus              |
| 50                  | 42                   | NIAB.SHW.018              | Robigus              |
| 141                 | 41                   | NIAB.SHW.027              | Robigus              |
| 144                 | 68                   | NIAB.SHW.035              | Robigus              |
| 209/211             | 64                   | NIAB.SHW.041              | Robigus              |
| 212                 | 59                   | NIAB.SHW.054              | Robigus              |
| 213                 | 52                   | NIAB.SHW.055              | Robigus              |
| 219                 | 61                   | NIAB.SHW.069              | Robigus              |
| 222                 | 83                   | NIAB.SHW.071              | Robigus              |
| 226                 | 52                   | NIAB.SHW.073              | Robigus              |
| 233                 | 65                   | NIAB.SHW.075              | Robigus              |
| 237                 | 64                   | NIAB.SHW.076              | Robigus              |
| 244                 | 60                   | NIAB.SHW.077              | Robigus              |
| 348                 | 59                   | NIAB.SHW.082              | Robigus              |
| 350/351             | 63                   | NIAB.SHW.083              | Robigus              |
| 353/354             | 60                   | NIAB.SHW.084              | Robigus              |
| 356/358             | 40                   | NIAB.SHW.085              | Robigus              |
| 359/361             | 56                   | NIAB.SHW.086              | Robigus              |
| 363/365             | 21                   | NIAB.SHW.087              | Robigus              |
| 368/369             | 36                   | NIAB.SHW.078              | Robigus              |
| 398                 | 59                   | NIAB.SHW.089              | Robigus              |
| 401                 | 69                   | NIAB.SHW.090              | Robigus              |
| 403                 | 37                   | NIAB.SHW.091              | Robigus              |
| 405                 | 69                   | NIAB.SHW.092              | Robigus              |
| 465                 | 64                   | NIAB.SHW.099              | Robigus              |
| 467                 | 37                   | NIAB.SHW.100              | Robigus              |
| 470                 | 54                   | NIAB.SHW.088              | Robigus              |
| 472                 | 51                   | NIAB.SHW.093              | Robigus              |
| 473                 | 76                   | NIAB.SHW.094              | Robigus              |
| 476                 | 52                   | NIAB.SHW.095              | Robigus              |
| 478                 | 58                   | NIAB.SHW.101              | Robigus              |
| 480                 | 64                   | NIAB.SHW.104              | Robigus              |
| 484                 | 78                   | NIAB.SHW.106              | Robigus              |
| 487                 | 72                   | NIAB.SHW.113              | Robigus              |
| 489                 | 57                   | NIAB.SHW.116              | Robigus              |
| 492                 | 33                   | NIAB.SHW.125              | Robigus              |
| 589                 | 67                   | NIAB.SHW.029              | Robigus              |
| 590                 | 54                   | NIAB.SHW.031              | Robigus              |
| 592                 | 55                   | NIAB.SHW.080              | Robigus              |
| 622                 | 74                   | NIAB.SHW.097              | Robigus              |
| 624                 | 59                   | NIAB.SHW.102              | Robigus              |
| 626                 | 53                   | NIAB.SHW.111              | Robigus              |
| 627                 | 63                   | NIAB.SHW.112              | Robigus              |
| 628                 | 61                   | NIAB.SHW.117              | Robigus              |
| 631                 | 51                   | NIAB.SHW.118              | Robigus              |
| 633                 | 30                   | NIAB.SHW.126              | Robigus              |
| 634                 | 73                   | NIAB.SHW.127              | Robigus              |
| 639                 | 57                   | NIAB.SHW.131              | Robigus              |
| 640                 | 68                   | NIAB.SHW.132              | Robigus              |
| 641                 | 54                   | NIAB.SHW.134              | Robigus              |
| 642                 | 52                   | NIAB.SHW.136              | Robigus              |
| 644                 | 39                   | NIAB.SHW.137              | Robigus              |
| 645                 | 54                   | NIAB.SHW.138              | Robigus              |
| 647                 | 50                   | NIAB.SHW.143              | Robigus              |


# Contact 

For queries on the data and usage please contact:

- richard.horsnell@NIAB.com and tally.wright@NIAB.com 

![](/image/shw-nam.png)

