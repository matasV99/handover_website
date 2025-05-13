# 🧬 Glioblastoma (GBM) Projects

This section outlines analysis pipelines, image processing workflows, and data integration for spatial transcriptomics of GBM tissue.

---

## 🧪 Key Datasets

- **CosMx spatial profiling**:
    - dataset of 4 patients (core vs edge) (FAILED NOT Edgy enough).
    - 940 genes x ~250k cells.
    - 3 protein stains: CD68, PanCK, CD45.
    - Final peprocessed object: [INSERT PATH TO FINAL OBJECT IN S3 BUCKET]
- **Matched H&E-stained slides**:
    - For homeodomain analysis (???).
- **Matched CEP7-stained slides**:
    - Matched CEP7-stained slides for neoplastic status determination (FAILED too far away).

---

## 🧠 Analysis Pipeline

- **Cell segmentation**:
    - Nuclei-based segmentation using Cellpose. Cell membrane stain used to optimize how much to dilate nuclei for cytoplasmic signal (13 px).
- **Cell typing**:
    - Graph-based clustering and subclustering of mixed clusters. Main datasets used: Neftel et al 2019, Ruiz-Moreno et al 2022, and Harwood et al 2024. Majority label picked from 3 annotators: Matas & Quyen, Yuk Kien, Wisna.
    - FAILED: neoplastic vs non-neoplastic label transfer using GBMap.
- **Downstream**:
    - Differential gene expression between core and edge samples.
    - Cell-cell signaling and ligand-receptor analysis using CellChat weighted based on distance between cells.
    - Spatial co-localization analysis per slide.
    - H&E annotations manually transferred after a manual affine transformation.
    - popV consensus based label transfer failed due to low number of genes not being able to label transcriptionally homogeneous GBM cells.


---

## 📁 Data Storage

- **S3 Bucket** for data (Need private keys to access): `s3://gbm.store.genome.sg`
- **GIS R Drive** for slides (Need GIS VPN to access): `S:\GIS-Liujy\Vitkauskas_Matas`

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