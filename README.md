# Mouse Colorectal Cancer Atlas – Figures 1–7 Reproducibility Package

This repository contains the complete R code and analysis notebooks required to reproduce **Figures 1–7** of the manuscript:

**“Genotype-phenotype mapping identifies fetal-like CD55+ immunoregulatory cancer cells as mediators of immune escape in colorectal cancer”**  
Mastel et al., *Bioarxiv* (in preparation / in press)

The code covers all atlas-level visualizations, single-cell analyses, pathology annotations, trajectory inference, immune–tumor interaction analyses, and cross-species comparisons presented in the text.

---

## Overview

We constructed a comprehensive mouse colorectal cancer (CRC) atlas spanning:

- Classical and serrated tumorigenesis routes  
- GEMM and multiplex CRISPR-GEMM models  
- Primary tumors and metastases  
- Epithelial plasticity, immune evasion, and microenvironmental remodeling  
- Cross-species integration with human CRC (TCGA, scRNA-seq)

Figures 1–7 integrate:

- Cohort and genotype overview (Fig. 1)
- Histopathological stratification (Fig. 1e)
- Single-cell ecosystem composition (Fig. 2–4)
- Tumor cell state plasticity and immune-regulatory programs (Fig. 5–6)
- Cross-species and translational analyses (Fig. 7)

All panels are generated from the same processed objects used for the manuscript, ensuring full computational reproducibility.

---

## Goals

The goal of this repository is to provide a fully transparent and executable reference for:

- Reproducing every main-text figure (Fig. 1–7)
- Linking genotype, pathology, and single-cell states
- Enabling reviewers and readers to regenerate all plots directly from source data
- Facilitating reuse of the atlas framework for comparative and translational studies

If the notebooks for all figures execute successfully and regenerate the published panels, this repository has achieved its goal.

---

## Repository structure

├── data/
│ ├── ATLAS_OVERVIEW.xlsx
│ ├── histo_mouse_atlas.xlsx
│ └── TCGA_CRC_metadata/
├── seurat_objects/
│ ├── SOC.rds
│ ├── cite.rds
│ ├── tumcells.rds
│ └── ...
├── notebooks/
│ ├── Code_Figure_1.Rmd
│ ├── Code_Figure_2.Rmd
│ ├── Code_Figure_3.Rmd
│ ├── Code_Figure_4.Rmd
│ ├── Code_Figure_5.Rmd
│ ├── Code_Figure_6.Rmd
│ ├── Code_Figure_7_a_i.Rmd
│ └── Code_Figure_7_j_l.Rmd
├── scripts/
│ ├── palettes.R
│ ├── helper_functions.R
│ └── trajectory_utils.R
└── figures/
├── Figure1.pdf
├── Figure2.pdf
└── ...

---

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

---

## Usage

All analyses were performed in **R ≥ 4.3**.

Core packages include:
Seurat v5, ComplexHeatmap, ggplot2, patchwork, circlize, slingshot, GSVA, fgsea, survival, survminer.

---

## Environment 


