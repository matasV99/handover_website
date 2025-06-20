# 🧬 Glioblastoma (GBM) Project

This section outlines analysis pipelines, image processing workflows, and data integration for spatial transcriptomics of GBM tissue.

---

## 🧪 Key Datasets

- **CosMx spatial profiling**:
    - dataset of 4 patients (core vs edge). 1 patient contains putatively "healthy infiltrated cortex" totaling 6 FOVs, but these are not enriched in NPC-like cells or neurons.
    - 940 genes x ~250k cells.
    - 3 protein stains: CD68, PanCK, CD45.
    - Final peprocessed object: `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_CosMx_GBM_project\CosMx_analysis\GBMap_clustering\labeled_object`
- **Matched H&E-stained slides**:
    - Slides annotated by a trained pathologist can be found here: `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_CosMx_GBM_project\Matching_stains\H&E stains (high res + annotation)`
- **Matched CEP7-stained slides**:
    - Matched CEP7-stained slides for neoplastic status determination. Slices are too far away from CosMx.

---

## 🧠 Analysis Pipeline

- **Cell segmentation**:
    - Nuclei-based segmentation using Cellpose. Cell membrane stain used to optimize how much to dilate nuclei for cytoplasmic signal (13 px).
- **Cell typing**:
    - Graph-based clustering and subclustering of mixed clusters. Main datasets used: Neftel et al 2019, Ruiz-Moreno et al 2022, and Harwood et al 2024. Majority label picked from 3 annotators: Matas & Quyen, Yuk Kien, Wisna.
    - FAILED (too few genes in CosMx panel): neoplastic vs non-neoplastic label transfer using GBMap.
- **Downstream**:
    - Differential gene expression between core and edge samples. No enrichment in NPC-like cells found in edge samples, possibly due to bulk nature of labeling samples.
    - Cell-cell signaling and ligand-receptor analysis using CellChat weighted based on distance between cells. Find strong SPP1 and VEGFA signaling between MES-like cells and TAM-BDM, and endothelial cells respectively.
    - Spatial co-localization analysis per slide.
    - H&E annotations manually transferred after a manual affine transformation. No new insights based on H&E annotations.
    - popV consensus based label transfer failed due to low number of genes not being able to label transcriptionally homogeneous GBM cells.


---

## 📁 Data Storage

- **Raw data**: `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_CosMx_GBM_project\Raw_CosMx`
- **Processed data**: `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_CosMx_GBM_project\CosMx_analysis`
- **Slides**: `S:\GIS-Liujy\Vitkauskas_Matas\GBM_slides_MV_25_05_05`

---

## 🤖 Ronin AWS virtual machine packages

The Ronin AWS virtual machine project packages can be found at Neuromics-PD > New Machine > Project Packages:
- PopV - for consensus cell label transfer (CUDA set-up).
- Matas - to replicate PD and GBM project environments.

---

## 📦 GitHub Repositories

- **[GBM](https://github.com/matasV99/GBM)**  
  Image processing, segmentation, spot calling, and graph-based clustering pipelines for glioblastoma spatial transcriptomics.
- Backup of the main GBM analysis script can be found on the GIS R Drive: `S:\GIS-Liujy\Vitkauskas_Matas\script_GBM_analysis_MV`

---

## 🧑‍🔬 Collaborators

- **Dr. Jinyue Liu** – Principal Investigator.
- **Dr. Quyen Do** – Helped with CosMx annotation.
- **Dr. Yuk Kien Chong** – Helped with CosMx annotation.
- **Wisna Novera** – Helped with CosMx annotation.