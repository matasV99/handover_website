The following is an overarching structure of S3 test (Parkinson's disease) bucket for Jinyue Liu's single-cell spatial neuromics lab:

Project folder --> [author]_[technique]_[subject]


1. Yang_Lin_scATACseq_scRNAseq_CDA_project
-scRNA
--CDA # contains 17S and 18S iPSC lines from NYSCF from Woodard 2014, MTA docs are with Judy 
-scATAC
--18S
--17S  

2. Jo_Junghyun_bulkRNAseq
# human midbrain-like organoid sample
LRRK2 - H9 isogenic LRRK2-G2019S point mutation
PINK1, PARK2, GBA - H9 isogenic KO for respective gene
SNCA - overexpression of HA-tagged SNCA-A30P 
- RHE1174	LRRK2-1 D90
- RHE1175	LRRK2-2 D90
- RHE1176	LRRK2-3 D90
- RHE1177	PINK1-1 D90
- RHE1178	PINK1-2 D90
- RHE1179	PINK1-3 D90
- RHE1180	PARK2-1 D90
- RHE1181	PARK2-2 D90
- RHE1182	PARK2-3 D90
- RHE1183	H9 WT1 D90
- RHE1184	H9 WT2 D90
- RHE1185	H9 WT3 D90
- RHE1186	GBA1 D90
- RHE1187	GBA2 D90
- RHE1188	GBA3 D90
- RHE1189	SNCA1 D90
 RHE1190	SNCA2 D90
- RHE1191	SNCA3 D90
- RHE1192	GBA-SNCA 1 D90
- RHE1193	GBA-SNCA 2 D90
- RHE1194	GBA-SNCA 3 D90
- RHN834	H9-wildtype-day60-1
- RHN835	H9-wildtype-day60-2
- RHN836	H9-wildtype-day60-3
- RHN837	H9-PARK2 KO-day60-1
- RHN838	H9-PARK2 KO-day60-2
- RHN839	H9-PARK2 KO-day60-3
- RHN840	H9-PINK1 KO-day60-1
- RHN841	H9-PINK1 KO-day60-3
- RHN842	H9-PINK1 KO-day60-4
- RHN843	H9-GBA KO-day60-2
- RHN844	H9-GBA KO-day60-3
- RHN845	H9-GBA KO-day60-4
- RHN846	H9-SNCA Dox-)-day60-1
- RHN847	H9-SNCA Dox-)-day60-2
- RHN848	H9-SNCA Dox-)-day60-3
- RHN849	H9-SNCA Dox+)-day60-1
- RHN850	H9-SNCA Dox(+)-day60-2
- RHN851	H9-SNCA Dox(+)-day60-3
- RHN852	GM23338-day60-1
- RHN853	GM23338-day60-3
- RHN854	GM23338-day60-4
- RHN855	ND34391-day60-1
- RHN856	ND34391-day60-3
- RHN857	ND34391-day60-4


3. Jo_Junghyun_bulkRNAseq_LBLI # Published in a 2021 paper in annals of neurology # lbli = lewy body like inclusions
- LBLI_D60 # (WT-H9, GBAko, SNCA-WT o/e samples)
- LBLI_D90 #LBLI_D90 (published in Annals of Neurology, WT-H9 and SNCA-WT o/e samples)


4. Yang_Lin_bulkRNAseq_MSD
- MSD_D60 # MSD is merck/ Merck Sharp & Dohm, a company that funded this collaboration
- D60_G - LRRK2 G2019S isogenic knock-in, batch 1 and batch 2
- D60_S - SNCA-A30P overexpression, batch 1 and batch 2
- D60_WT - H9 WT, batch 1 and batch 2
- D90L - LRRK2 G2019S isogenic knock-in, batch 1, batch 3 and batch 4
- D90S - SNCA-A30P overexpression, batch 1, batch 3 and batch 4
- D90WT - H9 WT, batch 1, batch 3 and batch 4


5. Xie_Jessica_bulkRNAseq_WT_DJ1KO
- novogene_nov2020_bulk
-----D60_G - LRRK2 G2019S isogenic knock-in, batch 1 and batch 2
-----D60_S - SNCA-A30P overexpression, batch 1 and batch 2
-----D60_WT - H9 WT, batch 1 and batch 2
-----D60_DJ1 - DJ1 KO, batch 1 and batch 2

- Xie_Jessica_bulk_alignment_and_analysis
- TH_DJ1_bulk
- WT_DJ1_bulk
----- these 3 folders are analysis files not raw files

6. Xie_Jessica_scRNAseq_merFISH_WT_DJ1KO
-scRNA
-------WT
--------------fastq_files
-------------------MLO1-6 # scRNAseq of midbrain-like organoids
-------------------XHO006 # Supposedly MLO0 sample with library code MUX 11099, downloaded from SRA by Jessica
--------------after_hg38_alignment_no_introns # MLO scRNAseq hg38 genome alignment results performed by ??? in ???
-----------------------MLO0-6 
-----------------------Matas_MLO_3_2_23 # folder containing the finalized scRNAseq object at 3_2_23 by Matas Vitkauskas; used the aligned genomes in this folder
--------------after_hg38_alignment_with_introns # MLO scRNAseq hg38 genome alignment results performed by Matas Vitkauskas in 2023 March. Used Cell Ranger v7.0+
-----------------------XHO006_MLO0 # XHO006_HS007 and XHO006_HS006 (both MLO0) aligned to hg38 genome with cellranger count
-----------------------MLO1-6 #scRNAseq samples from scRNA folder aligned to hg38 genome with cellranger count
-----------------------HS006-XHO006_MLO0 #XHO006_HS006 (MLO0) without GFP knocked into its reference genome - after cellranger count
-----------------------GFP_HS006_XHO006_MLO0 #XHO006_HS006 (MLO0) sample with GFP knocked into its reference genome - after cellranger co
-------WT_DJ1KO
--------------fastq_files
-------------------XHI023-30 # WT and DJ1KO aligned to hg38 genome
--------------after_hg38_alignment_with_introns # Used Cell Ranger v7.0+
----------------------XHI023-30 # WT and DJ1KO aligned to hg38 genome
-merFISH
---------raw_TIF_files # raw merFISH TIF files taken by Jessica Xie
----------------------each file contains 'DAPI' and 'S10' hyb images, raw imaging data.
---------JX_spot_assignment
----------------------01-22 # folders containing individual samples with .dapi image, cell segmentation mask, and unassigned spots (coors_combined_merged.hdf5). Other files come from linli's cell segmentation script titled "spot_assignment_linli_221101"
---------spot_assignment_linli_221101

7. Sun_Alfred_scRNAseq_MS
---MS3 # Alfred Sun's midbrain spheroid samples

8. Author_X_fastq_files_TH_EGFP 
--- HO001-06 # The origin of these samples is not clear, XHO006 seems to be MLO0 sample

