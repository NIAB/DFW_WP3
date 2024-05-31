---
layout: post
title:  "Sequence variants for key tetraploid wheat components within NIAB DFW germplasm"
date:   2024-05-31 11:11:05 +0000
categories: jekyll update
---

# Summary

*John Connell, Lawrence Percival-Alwyn, Tally I. C. Wright, Philip Howell*.

Sequence variants for wild emmer accession ‘TTD-140’ (donor for NIAB_AB_CSSL lines) and durum wheat ‘Hoh-501’ (most commonly used tetraploid component of NIAB Synthetic Hexaploid Wheat lines).  

# Method

<p align="justify"> Paired-end reads were trimmed using trim-galore (Krueger. 2019) to remove adapter sequences and quality filter (-q 25), retaining only reads with a length greater or equal to 75 bp (-l 75) before aligning with BWA mem version 0.7.17-r1188 (Li. 2013) against their respective reference assemblies (HOH501 to <i>Triticum turgidum</i> [ensemblegenomes release-55] and TTD140 to <i>Triticum dicoccoides</i> [ensemblegenomes release-55]), in addition to both samples being mapped to Chinese Spring  (RefSeq v1.0, IWGSC 2018). Following BWA alignment, SAMtools (Li et al., 2009) was used to retain proper read pairs with a mapping quality of 20 and above and to remove non-primary alignments (-q 20 -f3 and -F256). Duplicates were removed using Picard tools version 3.1.1 (www.github.com/broadinstitute/picard) before and after merging BAMs of the same sample. Variant calling was performed using BCFtools (version 1.9) (Li, 2011) mpileup, where allelic and total depth information were computed (-a AD,DP) before calling using BCFtools call in consensus-caller mode (-c) to identify variants (-v) and it output a file in vcf format (-Ov). </p>

# Link

The VCF data is hosted on the Grassroots Data Repository, a link to the page can be found [here.](https://opendata.earlham.ac.uk/wheat/under_license/toronto/Howell_2024_05_17_Tetraploid_sequencing/)

# Funding

This work was supported by the BBSRC through the Cross-Institute Strategic Program ‘Designing Future Wheat’ (BB/P016855/1) and the Bioinformatics and Biological Resources Fund research grant ‘Ensembl Plant Populations’ (BB/X018725/1). 

# References

The International Wheat Genome Sequencing Consortium (IWGSC), Appels R, Eversole K, Feuillet C, Keller B, Rogers J, Stein N, Pozniak CJ, Stein N, Choulet F, Distelfeld A, Eversole K, Poland J, Rogers J, Ronen G, Sharpe AG, Pozniak C, Ronen G, Stein N, Barad O, Baruch K, et al. (2018) Shifting the limits in wheat research and breeding using a fully annotated reference genome. Science 361: eaar7191

Krueger, F. (2019). Trim Galore! Available online at: http://www.bioinformatics.babraham.ac.uk/projects/trim_galore/

Li H, Handsaker B, Wysoker A, Fennell T, Ruan J, Homer N, Marth G, Abecasis G, Durbin R; 1000 Genome Project Data Processing Subgroup. 2009. The Sequence Alignment/Map format and SAMtools. Bioinformatics. DOI: 10.1093/bioinformatics/btp352.

Li H. (2011). A statistical framework for SNP calling, mutation discovery, association mapping and population genetical parameter estimation from sequencing data. Bioinformatics, 27(21), 2987–2993. DOI:10.1093/bioinformatics/btr509

Li, H. (2013). Aligning sequence reads, clone sequences and assembly contigs with BWA-MEM. arXiv:1303.3997v2.11 pt

*Triticum dicoccoides*: https://ftp.ensemblgenomes.ebi.ac.uk/pub/plants/release-55/fasta/triticum_dicoccoides/dna/Triticum_dicoccoides.WEWSeq_v.1.0.dna.toplevel.fa.gz

*Triticum turgidum*: https://ftp.ensemblgenomes.ebi.ac.uk/pub/plants/release-55/fasta/triticum_turgidum/dna/Triticum_turgidum.Svevo.v1.dna.toplevel.fa.gz
