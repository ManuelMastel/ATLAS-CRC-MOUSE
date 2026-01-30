# Mouse Colorectal Cancer Atlas

This repository contains the complete R code and analysis notebooks required to reproduce **Figures** of the manuscript:

**“Genotype-phenotype mapping identifies fetal-like CD55+ immunoregulatory cancer cells as mediators of immune escape in colorectal cancer”**  
Mastel et al., *Biorxiv* (in preparation / in press)

The code covers all atlas-level visualizations, single-cell analyses, pathology annotations, trajectory inference, immune-tumor interaction analyses and cross-species comparisons presented in the text.

## Overview

We constructed a comprehensive mouse colorectal cancer (CRC) atlas spanning:

- Classical and serrated tumorigenesis routes  
- GEMM and multiplex CRISPR-GEMM models  
- Wild-type colon tissue, adenomas and carcinomas from different mouse models  
- Epithelial plasticity, immune evasion, and microenvironmental remodeling  
- Cross-species integration with human CRC (TCGA, scRNA-seq)

Figures 1–7 integrate:

- Cohort and genotype overview (Fig. 1)
- Histopathological stratification (Fig. 1e)
- Single-cell ecosystem composition (Fig. 2–4)
- Tumor cell state plasticity and immune-regulatory programs (Fig. 5–6)
- Cross-species and translational analyses (Fig. 7)

All panels are generated from the same processed objects used for the manuscript, ensuring full computational reproducibility.

## Goals

The goal of this repository is to provide a fully transparent and executable reference for:

- Reproducing every figure
- Linking genotype, pathology, and single-cell states
- Enabling reviewers and readers to regenerate all plots directly from source data
- Facilitating reuse of the atlas framework for comparative and translational studies

If the notebooks for the figures execute successfully and regenerate the published panels, this repository has achieved its goal.

## Figure–code mapping

| Figure | Notebook | Description | 
|--------|----------|-------------|
| Fig. 1b | `Code_Figure_1.Rmd` | Atlas genotype & cohort overview |
| Fig. 1e | `Code_Figure_1.Rmd` | Histopathology grid by genotype |
| Fig. 2  | `Code_Figure_2.Rmd` | Single-cell ecosystem composition |
| Fig. 3  | `Code_Figure_3.Rmd` | Tumor cell states and microenvironment |
| Fig. 4  | `Code_Figure_4.Rmd` | Lineage trajectories and fate branching |
| Fig. 5  | `Code_Figure_5.Rmd` | Immune evasion and regulatory programs |
| Fig. 6  | `Code_Figure_6.Rmd` | Plasticity, fetal-like and squamous programs |
| Fig. 7a–i | `Code_Figure_7_a_i.Rmd` | Cross-species state alignment |
| Fig. 7j–l | `Code_Figure_7_j_l.Rmd` | TCGA survival and CMS/IRC analyses |

## Usage

All analyses were performed in **R ≥ 4.3**.

Core packages include:
Seurat v5, ComplexHeatmap, ggplot2, patchwork, circlize, slingshot, GSVA, fgsea, survival, survminer.

## Environment

The analyses were developed and tested on macOS and Linux using:

- R 4.3+
- Seurat 5.0+
- ComplexHeatmap 2.18+
- ggplot2 3.5+
- slingshot 2.8+
- GSVA 1.50+

## Data Availability

Processed single-cell objects are available via **Figshare** (DOI to be added).  
Raw sequencing data are deposited at **ArrayExpress** (accession to be added).
Integrative single-cell analysis of human colorectal cancer can be downloaded via **Figshare** (https://doi.org/10.6084/m9.figshare.25323397)
TCGA data were accessed through **TCGAbiolinks**.

## Citation

If you use this code or data, please cite:

Mastel M. et al.  
*Genotype-phenotype mapping identifies fetal-like CD55+ immunoregulatory cancer cells as mediators of immune escape in colorectal cancer.*  
Bioarxive.

## History

All figures in the manuscript were generated directly from the scripts contained in this repository to ensure complete computational provenance and long-term reproducibility.


