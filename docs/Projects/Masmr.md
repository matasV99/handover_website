# 🧬 Modular Algorithms for Spotcalling in MERFISH in R (masmr) Project

This section covers all masmr-related computational work on R-native MERFISH custom image processing pipeline.

---

## 🔍 Key Datasets

- **MLO MERFISH**:
    - 1 MERFISH run, 3 organoid samples, ~100 FOVs, 8 hybridization rounds x 2 channels. Everything has 5 z-stacks.
    - Raw data can be found here: `S:\GIS-Liujy\PD_data\Xie_Jessica_scRNAseq_merFISH_WT_DJ1KO\merFISH\raw_image_file\20220624_jx_A034_T2_block2_good`
    - Cookbook can be found here: `TBD after clear the masmr vm`
- **Mouse Brain MERFISH**:
    - Zhoang et al 2023. 2 Coronal sections. .dax format.
    - Raw data: `S:\GIS-Liujy\Vitkauskas_Matas\Zhuang_MERFISH_mouse_brain\coronal_1`
    - Cookbook and microscope information can be found here: `S:\GIS-Liujy\Vitkauskas_Matas\Zhuang_MERFISH_mouse_brain\additional_files`

---

## 🧠 My contribution to the project

1. Co-implementation for user-friendly quality control during the choice-making building the custom image processing pipeline.
2. Co-implementation of Maximum intensity projection support for multi-depth images.
3. Bug fixes related to image processing, stitching and overlap estimation during synthesis of multiple FOVs.
4. Ran Masmr on the MLO dataset.

---

## 📁 Data Storage

- **Processed data**: `TBD Matas' R drive`
- **Slides**: `TBD once finalized`

---

## 📦 Masmr-related code

- **Vignettes for MLO** 
    - Data structure checking, Spot assignment, Cell Segmentation, Stitching, Synthesis scripts and Downstream benchmarking: `S:\GIS-Liujy\Vitkauskas_Matas\MASMR_FOLDER`

---

## 🧑‍🔬 Collaborators

- **Dr. Jinyue Liu** – Principal Investigator.
- **Dr. Eugene Kwa** – The author of masmr. Implemented features that I suggested as the first masmr user.