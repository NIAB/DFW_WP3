---
layout: post
title:  "NIAB_WW_SHW_NAM data repository"
date:   2023-07-17 10:43:05 +0000
categories: jekyll update
---

# Summary 

This page hosts the genetic marker and phenotypic data from Wright, Horsnell et al. (*underprep*). This version of the data has been through a quality control pipeline outlined in the paper.

# Data Download

The QC'd genotype data can be downloaded [here](https://github.com/NIAB/niab-dfw-wp3/raw/main/data/NIAB_WW_SHW_NAM_clean_geno.zip). The zip folder includes the following files:

The repository contains the following files:
- `dataset.map.csv` the physical positions for 11,051 SNP markers
- `dataset.1.NAM.mapped.csv` the genotypes across 11,051 markers for 2637 SHW NAM individuals  
- `dataset.1.NAM.mapped.with.parents.csv`the genotypes across 11,051 markers for 2637 SHW NAM individuals + 54 primary SHW parents and Robigus
- `dataset.2.NAM.mapped.skim100` is `dataset.1.NAM.mapped.csv` skimmed to remove markers with an absolute Pearson correlation (r) of 1
- `dataset.3.NAM.mapped.skim80` is `dataset.1.NAM.mapped.csv` skimmed to remove markers with an absolute Pearson correlation (r) above 0.80
- `NIAB.WW.SHW.NAM.pedigree.info.csv` contains the pedigree information for the population

The data is in numeric format and was converted from the original axiom call codes format (AA, AB, BB and NoCall) using the following conversion:

`"NoCall" = NA`
`"AA" = 0`
`"AB" = 1`
`"BB" = 2`

The phenotypic data from the six trials used in the paper can be downloaded [here.](https://github.com/NIAB/niab-dfw-wp3/raw/main/data/NIAB_WW_SHW_NAM_combined_pheno.zip)

The raw and unedited version of the genotype data can be downloaded from [here](https://github.com/NIAB/niab-dfw-wp3/raw/main/data/NIAB_WW_SHW_NAM_raw_geno.zip). This zip folder includes the following files:

- `full.markers.winter.shw.nam.v1.csv` the dataset with NIAB codes.
- `GRUvs.NIAB.code.conversion.csv` a conversion file to link up the Academic and Breeders' toolkit lines with the NIAB codes. See [here](https://designingfuturewheat.org.uk/work-package-3/) for more info on these toolkits. 


# Contact 

For queries on the data and usage please contact:

- tally.wright@niab.com and richard.horsnell@niab.com


![](/niab-dfw-wp3/image/shw-nam.png)