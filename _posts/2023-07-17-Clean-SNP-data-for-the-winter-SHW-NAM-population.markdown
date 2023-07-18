---
layout: post
title:  "Clean SNP data for the winter SHW NAM population"
date:   2023-07-17 10:43:05 +0000
categories: jekyll update
---

# Summary 

This page hosts the genetic marker data used in Wright et al. (underprep). The data is the quality controlled version of the raw data available [here](https://niab.github.io/niab-dfw-wp3/jekyll/update/2022/12/12/SNP-data-for-the-winter-SHW-NAM-population.html).

# Data Download

The data can be downloaded [here](https://github.com/NIAB/niab-dfw-wp3/raw/main/data/clean.niab.winter.shw.nam.zip). The zip folder includes the following files:

The repository contains the following files:
- `dataset.map.csv` the physical positions for 11,051 SNP markers
- `dataset.1.NAM.mapped.csv` the genotypes across 11,051 markers for 2637 SHW NAM individuals  
- `dataset.1.NAM.mapped.with.parents.csv`the genotypes across 11,051 markers for 2637 SHW NAM individuals + 54 primary SHW parents and Robigus
- `dataset.2.NAM.mapped.skim100` is `dataset.1.NAM.mapped.csv` skimmed to remove markers with an absolute Pearson correlation (r) of 1
- `dataset.3.NAM.mapped.skim80` is `dataset.1.NAM.mapped.csv` skimmed to remove markers with an absolute Pearson correlation (r) above 0.80

The data is in numeric format and was converted from the original axiom call codes format (AA, AB, BB and NoCall) using the following conversion:

`"NoCall" = NA`
`"AA" = 0`
`"AB" = 1`
`"BB" = 2`

# Contact 

For queries on the data and usage please contact:

- richard.horsnell@niab.com and tally.wright@niab.com 


