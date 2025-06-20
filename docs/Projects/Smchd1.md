# 🧬 Structural Maintenance Of Chromosomes Flexible Hinge Domain Containing 1 (Smchd1) Project

This section covers all smchd1-related computational work on scRNAseq dataset of mouse testes with Dr. Shifeng Xue's lab.

---
## 🔍 Key Datasets

- **scRNA-seq**:
    - pooled scRNAseq dataset at P4 of Smchd1 heterozygous and Smchd1 homozygous. Cell Ranger aligned, and cell types labeled by: Matas Vitkauskas.
    - Final peprocessed object: `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_scRNAseq_Smchd1_project\scRNAseq_analysis/final_smchd1_combined_prepped`

---

## 🧠 Analysis Highlights

1. Too few germ cells to find resilience markers at P4.
2. Sertoli and Myoid cells show a resilience pattern, although not sure if this is useful for collaborator project.
3. We recapitulate known cell-cell signaling patterns: a) ACTIVIN + KIT signaling between Sertoli and germ cells (stem cell self-renewal/differentiation balance), b) BMP signaling - leydig cells and germ cells (testosterone production).
4. TE analysis where transposable elements are quantified from .bam files does not yield interesting insights.

---

## 📁 Data Storage

- **Raw data** (only aligned CellRanger data was provided by colllaborators): `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_scRNAseq_Smchd1_project\scRNAseq_analysis\CellRanger_data`
- **Processed data**: `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_MLO_scRNAseq_MERFISH_analysis`
- **Slides**: `S:\GIS-Liujy\Vitkauskas_Matas\Smchd1_slides_MV_25_05_05`

---
## 📦 Smchd1 analysis master script

- **A single R file** 
    - scRNA-seq (Seurat) and CellChat analysis of smchd1 mutation efects in mouse testes: `S:\GIS-Liujy\Vitkauskas_Matas\script_Smchd1_analysis_MV.R`

---

## 🧑‍🔬 Collaborators

- **Dr. Jinyue Liu** – Principal Investigator.
- **Angie Chong En Qi** – Created scRNAseq dataset and assisted with cell typing.