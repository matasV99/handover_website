# 🧬 smchd1 mutation Projects

This section covers all smchd1-related computational work on scRNAseq dataset of mouse testes with Dr. Shifeng Xue's lab.

---
## 🔍 Key Datasets

- **scRNA-seq**:
    - pooled scRNAseq dataset at day X of Smchd1 heterozygous and Smchd1 homozygous. Cell Ranger aligned, and cell types labeled by: Matas Vitkauskas.
    - Final peprocessed object: `s3://gbm.store.genome.sg/Smchd1_project/scRNAseq_analysis/final_smchd1_combined_prepped`

---

## 🧠 Analysis Highlights

1. Too few germ cells to find resilience markers at day X.
2. Sertoli and Myoid cells show a resilience pattern, although not sure if this is useful for collaborator project.
3. We recapitulate known cell-cell signaling patterns: a) ACTIVIN + KIT signaling between Sertoli and germ cells (stem cell self-renewal/differentiation balance), b) BMP signaling - leydig cells and germ cells (testosterone production).
4. TE analysis where transposable elements are quantified from .bam files does not yield interesting insights.

---

## 📁 Data Storage

- **S3 Bucket** for data (Need private keys to access): `s3://gbm.store.genome.sg/Smchd1_project/`
- **GIS R Drive** for slides (Need GIS VPN to access): `S:\GIS-Liujy\Vitkauskas_Matas`

See `Data_Storage.md`  for detailed structure.

---
## 📦 Smchd1 analysis master script

- **A single R file** 
    - scRNA-seq (Seurat) and CellChat analysis of smchd1 mutation efects in mouse testes. Can be found in two locations:
        - `S:\GIS-Liujy\Vitkauskas_Matas\script_Smchd1_analysis_MV.R`
        - `s3://gbm.store.genome.sg/Smchd1_project/scRNAseq_analysis/script_Smchd1_analysis_MV.R`

---

## 🧑‍🔬 Collaborators

- **Dr. Jinyue Liu** – Principal Investigator.
- **Angie Chong En Qi** – Created scRNAseq dataset and assisted with cell typing.