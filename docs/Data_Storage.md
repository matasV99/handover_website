# 🗂️ Data Storage

## 1. 💻 AWS S3 Buckets

PD-related datasets are stored in the **test S3 bucket**. GBM-related datasets are stored in the **GBM S3 bucket**. Naming conventions are outlined in the `.README` file (see below).

### 🧾 Bucket README Summary
- [author]_[technique]_[subject]
- E.g., `Xie_Jessica_scRNAseq_merFISH_WT_DJ1KO`
- Contains raw fastq, aligned Cell Ranger outputs, raw TIFs, and segmentation masks.

📄 Full README from the S3 bucket [TBD]:

- [See `test_s3_README.txt`](test_s3_README.txt)
- [See `GBM_s3_README.txt`](gbm_s3_README.txt)

### 🔑 Bucket Access Keys
> (Omitted here — should be found within a .txt file in R drive here: S:\GIS-Liujy\Vitkauskas_Matas\s3_keys.txt)

## 2. 🤖 Ronin AWS virtual machine packages

Virtual machines that can be found on lab's Ronin AWS website: RNASEQ > New_Machine > Search_Packages:
- PopV - for consensus cell label transfer (CUDA set-up).
- Kallisto-scVelo - for rapid transcript pseudo-quantifiation using kallisto and all the necessary packages to run scVelo for RNA velocity analysis.
- Cellpose - for cell segmentation using Cellpose.
- Matas - to replicate PD and GBM project environments.

## 3. 💿 GIS R-Drive
Path: `R:/Projects/Neurogenomics/Matas/`
- Archived Smchd1 data.
- Archived Slides for PD, GBM, Smchd1 and Miscellaneous on day 2025_05_05.