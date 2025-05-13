Smchd1_project/
+-- Intermediate_files
¦   # Intermediate files for transposable element analysis. I had to get BAM files in a certain format for package scTE.
¦   +-- cleanup_script.sh
¦   ¦   # reformats the header of raw .bam files.
¦   +-- run_scTE.sh
¦   ¦   # runs scTE transposon quantification on the cleaned files andoutputs .excel files.
¦   +-- out_Het.xlsx, out_Hom.xlsx
¦       # The output from this out_Het.xlsx and out_Hom.xlsx can be found in Smchd1_project/TE_analysis/TE_files.
¦
+-- scRNAseq_analysis
¦   +-- CellRanger_data
¦   ¦   # output files from CellRanger genome alignment pipeline.
¦   +-- update_23_09_11
¦   ¦   # first result that we shared with Xue lab - DEG per cell type, GO enrichment).
¦   +-- updates_25_03_26
¦   ¦   # DEG of different cell types that are merged (not split up by high resolution) + CellChat analysis
¦   +-- final_smcdh1_combined_prepped
¦       # Final preprocessed object for this analysis.
¦
+-- TE_analysis
    +-- scTE
    ¦   # installed package
    +-- 7_9_23_TE_analysis
    ¦   # Preliminary analysis of an object containing transposable elements. For final plots, see the folders below.
    ¦
    +-- DE_TEs_celltype_comparison
    ¦   +-- within Homozygous or Heterozygous cell-types, what are the differentially expressed TEs between cell-types?
    ¦   +-- 0.25 log-2-fold-change cutoff; 0.25 proportion of cells have to express this gene within cluster
    ¦   +-- This comparison will tell you which TEs are present in each celltype in each genotype.
    ¦
    +-- combined_DE_TEs_celltype_comparison
    ¦   +-- Within both Homozygous and Heterozygous cells, what are the differentially expressed TEs between cell-types?
    ¦   +-- 0.25 log-2-fold-change cutoff; 0.25 proportion of cells have to express this gene within cluster
    ¦
    +-- DE_TEs_genotype_comparison
        +-- Within a cell-type, what are the differentially expressed TEs between genotypes?
        +-- 0.1 log-2-fold-change cutoff; 0.1 proportion of cells have to express this gene within cluster
        +-- This comparison will tell you which TEs are present/absent in homo compared to het. it won't tell you which TEs are present in both.