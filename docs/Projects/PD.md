# 🧬 Parkinson’s Disease (PD) Project

This section covers all PD-related computational work, including MERFISH, scRNA-seq, bulk RNA-seq, and multi-modal analyses on hMLOs and DJ-1 KO human midbrain-like organoids (hMLOs).

---

## 🔍 Key Datasets

- **MERFISH**:
    - WT and DJ-1 KO midbrain-like organoids (Generated by: Jessica Xie, Spots assigned + analyzed by: Matas Vitkauskas).
    - Final preprocessed object: `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_MLO_scRNAseq_MERFISH_analysis\MERFISH_files\analysis\40_genes_object`
- **scRNA-seq**:
    - Two sequencing batches of 8 hMLO WT datasets (day 60-156) and 4 x 4 WT and paired DJ-1 KO datasets (day 60-150). Aligned using Cell Ranger and analyzed using Seurat and other third-party R packages by: Matas Vitkauskas.
    - Final preprocessed object of all cells object (both genotypes): `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_MLO_scRNAseq_MERFISH_analysis\figure_folders\Figure_1\final_object`
    - Final preprocessed object of DaN cells (both genotypes): `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_MLO_scRNAseq_MERFISH_analysis\figure_folders\Figure_3\MLO_DA`
- **Bulk RNA-seq**: 
    - SNCA-A30P, PARK2 KO, PINK1 KO, GBA KO, GBA (Junghyun Jo, Yang Lin).
    - LBLI D60/D90 samples from Annals of Neurology 2021 paper.
    - day 60 WT vs DJ-1 KO (Jessica Xie).

---

## 🧠 Analysis Highlights

1. Both scRNAseq and MERFISH are used on hMLOs.
2. hMLOs have topographical segmentation that mimic in-vivo-like patterns (areas representing dopaminergic and GABAergic regions).
3. Four DaN Subtypes across the vulnerabilty-resilience transcriptomic axis in PD.
4. DJ-1 perturbation reveal broad mitochondrial dysregulation across all cell types and synapatic dysfunction specific to dopaminergic neurons.

---

## 📁 Data Storage

- **Raw data**: `S:\GIS-Liujy\PD_data`
- **Processed data**: `S:\GIS-Liujy\Vitkauskas_Matas\Vitkauskas_Matas_MLO_scRNAseq_MERFISH_analysis`
- **Slides**: `S:\GIS-Liujy\Vitkauskas_Matas\PD_slides_MV_25_05_05`

Each folder contains a .readME file that explains the overarching structure of the data.

---

## 🎰 NCBI GEO accession
Multi-modal data from PD project is currently private (scheduled to be publicly available on Jun 25, 2028 or following publication of the PD manuscript):

- GSE271115 [RNAseq]: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE271115
- GSE271116 [scRNAseq]: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE271116
- GSE271118 [MERFISH]: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE271118
- NCBI GEO reviewer keys: `S:\GIS-Liujy\Vitkauskas_Matas\reviewer_tokens`

---

## 🤖 Ronin AWS virtual machine packages

The Ronin AWS virtual machine project packages can be found at Neuromics-PD > New Machine > Project Packages:

- Kallisto-scVelo - for rapid transcript pseudo-quantifiation using kallisto and all the necessary packages to run scVelo for RNA velocity analysis.
- Cellpose - for cell segmentation using Cellpose.
- Matas - to replicate PD and GBM project environments.

---

## 📦 GitHub Repositories

- **[PD_project_analysis](https://github.com/matasV99/PD_project_analysis)**  
scRNA-seq and MERFISH analysis pipelines for PD midbrain organoids and KO models.
- Backup of the publication scripts can be found on the GIS R drive: `S:\GIS-Liujy\Vitkauskas_Matas\PD_manuscript_scripts\`

---

## 🧑‍🔬 Collaborators

- **Dr. Jinyue Liu** – Principal Investigator
- **Dr. Jessica Xie** – Created scRNAseq and MERFISH datasets (+ CRISPR-cas9 DJ-1 lines)
- **Dr. Quyen Do** - Helped with analysis of scRNAseq and MERFISH datasets