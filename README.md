# miR203_developmental_timing

## Description

This github repository contains the analysis code used in "miR-203 controls developmental timing and early fate restriction during preimplantation embryogenesis" published in bioRxiv:

Link: [https://www.biorxiv.org/content/10.1101/2024.02.06.579214v1](https://www.biorxiv.org/content/10.1101/2024.02.06.579214v1)

## Table of contents

- [Data](#Data)
- [Scripts](#Scripts)


## Data

All data of the project are available at the GEO repository under the accession code: GSE259428. This SuperSeries record provides access to all project data including SubSeries of Cut&Run data (GSE259425), Ultra-low input bulk RNA-seq (GSE259426) and single-cell RNA sequencing data (GSE259427). All data needed to evaluate the conclusions in the paper are present in the paper and/or the Supplementary Materials.

## Scripts

1. RNAseq

- [Ultra_low_input_RNAseq_analysis.ipynb](/scripts/RNAseq/Ultra_low_input_RNAseq_analysis.ipynb): Using as input files counts.txt file and metadata, it is done a preprocessing, exploratory analysis, dimensional reduction, score calculations of signatures and differential expression.

2. single-cell RNAseq
   
- [A.Create_object_and_initial_analysis.ipynb](/scripts/scRNAseq/A.Create_object_and_initial_analysis.ipynb): Using as input files STARsolo output files (gene and velocito) in this notebook is created an Anndata object, initial visualization, filtering, normalization and dimensional reduction.
- [B1.Downstream_analysis.ipynb](/scripts/scRNAseq/B1.Downstream_analysis.ipynb): Using as input file Part A output file, in this notebook is done clustering, scoring of signatures, cell classification, MERVL analysis and velocity.
- [B2.Downstream_analysis_paper_figures.ipynb](/scripts/scRNAseq/B2.Downstream_analysis_paper_figures.ipynb): Use Part B1 outfile and only visualization tasks are done, paper figures were created in that notebook.
- [C.Differential_expression_and_functional_analysis.ipynb](/scripts/scRNAseq/C.Differential_expression_and_functional_analysis.ipynb): In this notebooks has been done differential expresion and functional analysis doing comparisons of subpopulations, treatments, conditions and others. The h5ad file output of B1 part has been use in this notebook.

## Authors

All uploaded scripts have been done by:

- Marcos Malumbres
- Agustín Sánchez-Belmonte
