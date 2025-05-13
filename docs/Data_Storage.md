# 🗂️ Data Storage

## 1. 💻 AWS S3 Buckets

PD-related datasets are stored in the **test S3 bucket**. GBM-related datasets are stored in the **GBM S3 bucket**. Smchd1-related datasets are stored in the **GBM S3 bucket** as it was too big to be placed in GIS R Drive (~140 Gb). Naming conventions are outlined in `.README` file (see below).

### 🧾 Bucket README Summary
- [author]_[technique]_[subject]
- E.g., `Xie_Jessica_scRNAseq_merFISH_WT_DJ1KO`
- Contains raw fastq, aligned Cell Ranger outputs, raw TIFs, and segmentation masks.

📄 Full README from the S3 bucket [TBD: Still working on reordering s3 buckets]:

- [See `PD_s3_README`](test_s3_README.txt)
- [See `GBM_s3_README`](gbm_s3_README.txt)
- [See `Smchd1_README`](smchd1_RDrive_README.txt)

### 🔑 Bucket Access Keys
> (Omitted here — should be found within a .txt file in R drive here: S:\GIS-Liujy\Vitkauskas_Matas\s3_keys.txt)

## 2. 🤖 Ronin AWS virtual machine packages

Virtual machines that can be found on lab's Ronin AWS website: RNASEQ > New_Machine > Search_Packages:

- PopV - for consensus cell label transfer (CUDA set-up).
- Kallisto-scVelo - for rapid transcript pseudo-quantifiation using kallisto and all the necessary packages to run scVelo for RNA velocity analysis.
- Cellpose - for cell segmentation using Cellpose.
- Matas - to replicate PD and GBM project environments.

## 3. 🎰 NCBI GEO accession
Multi-modal data from PD project is currently private (scheduled to be publicly available on Jun 25, 2028 or following publication of the PD manuscript):

- GSE271115 [RNAseq]: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE271115
- GSE271116 [scRNAseq]: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE271116
- GSE271118 [MERFISH]: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE271118

## 4. 💿 GIS R-Drive
Path: `S:\GIS-Liujy\Vitkauskas_Matas`

- Archived Slides for PD, GBM, Smchd1 and Miscellaneous on day 2025_05_05.
- Archived s3 bucket keys, NCBI GEO reviewer keys.
- PD Manuscript code backup, GBM, and Smchd1 main script backup (25_05_13 upload).