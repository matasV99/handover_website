Project folder ? [author]_[technique]_[subject]
+-- Vitkauskas_Matas_CosMx_GBM_project
    +-- Raw_CosMx
    ¦   +-- Slide1  (samples: GLIO-0209 CORE, GLIO-0209 edge,
    ¦   ¦              GLIO-0141 core, GLIO-0141 IM)
    ¦   ¦   +-- SpotFiles                 # raw CosMx spot-call outputs
    ¦   ¦   ¦   +-- *.fth  (62 FOVs)
    ¦   ¦   +-- RunSummary
    ¦   ¦   ¦   +-- FovTracking           # stitching info
    ¦   ¦   +-- CellStatsDir
    ¦   ¦       +-- Morphology2D          # nuclei & membrane TIFFs
    ¦   ¦       ¦   +-- *.tif  (62 FOVs)
    ¦   ¦       +-- AnalysisResults       # CosMx segmentation results
    ¦   ¦           +-- (62 FOVs)
    ¦   +-- Slide2  (samples: GLIO-0133 core, GLIO-0133 margin 1,
    ¦   ¦              GLIO-0133 margin 2, GLIO-0180 CORE,
    ¦   ¦              GLIO-0180 MARGIN)
    ¦   ¦   +-- (65 FOVs structured like Slide1)
    ¦   +-- a174a2f9-936d-4801-aba9-d21a984207ed_TileDB
    ¦       +-- (CosMx run parameters)
    +-- Matching_stains
    ¦   +-- High_res_H&E
    ¦   +-- 40x_stain_CEP7                # .czi whole-section stains + alignments
    +-- CosMx_analysis
        +-- Raw_to_gcm_files
        +-- Clustering_and_other_stuff   # [TODO] move Extended_GBM_analysis here
        ¦   +-- Extended_GBM_analysis_labeled_object
        +-- QC_plots                     # nuclei & cell-area cutoffs
        +-- averaged_immunostaining_metadata
        ¦   +-- (CD68, CD45, PanCK per mask)
        +-- individual_samples           # per-FOV outputs
        +-- sample_metadata.csv          # collaborator metadata
        +-- unnormalized_full_CosMx.rds  # combined CosMx object, no preprocessing