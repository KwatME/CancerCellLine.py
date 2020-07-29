# Get Cancer Cell Line Data

Program for downloading cancer cell line data.

## Get

Download this.

## Use

Run [code/all.ipynb](code/all.ipynb). You specify a directory. And it will make a folder for each feature type. Inside each folder, it will download things, process them, and make useful feature_x_sample.tsv.

It should take less than 30 minutes to run.

It produces the file structure below. \* marks the useful .tsv files.

```
directory
├── feature
│   ├── sample_info.csv
│   ├── * cell_line_name_rename.tsv
│   ├── * feature_x_cell_line.tsv
│   ├── * feature_x_cell_line_x_01.tsv
│   └── * feature_x_cell_line_x_continuous.tsv
├── antibody
│   ├── CCLE_RPPA_20181003.csv
│   └── * antibody_x_cell.tsv
├── copy_number
│   ├── CCLE_gene_cn.csv
│   ├── * gene_x_cell_line.tsv
│   └── * gene_loss_gain_x_cell_line.tsv
├── crispr
│   ├── Achilles_gene_effect_unscaled.csv
│   └── * gene_x_cell_line.tsv
├── ctrp
│   ├── v20._COLUMNS.txt
│   ├── v20._README.txt
│   ├── v20.data.curves_post_qc.txt
│   ├── v20.data.per_cpd_avg.txt
│   ├── v20.data.per_cpd_post_qc.txt
│   ├── v20.data.per_cpd_pre_qc.txt
│   ├── v20.data.per_cpd_well.txt
│   ├── v20.meta.media_comp.txt
│   ├── v20.meta.per_assay_plate.txt
│   ├── v20.meta.per_cell_line.txt
│   ├── v20.meta.per_compound.txt
│   ├── v20.meta.per_experiment.txt
│   ├── new-abs-auc-with-qc.txt
│   ├── * gene_x_compound.tsv
│   ├── * activity_x_compound.tsv
│   └── * compound_x_cell_line.tsv
├── fusion
│   ├── CCLE_fusions_unfiltered.csv
│   └── * gene_x_cell_line.tsv
├── gdsc
│   ├── sanger-viability.csv
│   ├── sanger-dose-response.csv
│   ├── * compound_dose_x_cell_line.tsv
│   └── * compound_x_cell_line.tsv
├── methylation
│   ├── CCLE_RRBS_tss_CpG_clusters_20181022.txt.gz
│   └── * gene_x_cell_line.tsv
├── mutation
│   ├── CCLE_mutations.csv
│   ├── * gene_x_cell_line.tsv
│   ├── * gene_x_cell_line_x_01.tsv
│   ├── * gene_variant_classification_x_cell_line.tsv
│   └── * gene_protein_change_x_cell_line.tsv
├── np24
│   ├── CCLE_NP24.2009_Drug_data_2015.02.24.csv
│   └── * compound_x_cell_line.tsv
├── prism
│   ├── primary-screen-replicate-treatment-info.csv
│   ├── primary-screen-replicate-collapsed-logfold-change.csv
│   ├── secondary-screen-replicate-treatment-info.csv
│   ├── secondary-screen-replicate-collapsed-logfold-change.csv
│   ├── secondary-screen-dose-response-curve-parameters.csv
│   ├── * compound_dose_x_cell_line_x_primary.tsv
│   ├── * compound_dose_x_cell_line_x_primary.tsv
│   └── * compound_x_cell_line_x_secondary.tsv
├── protein
│   ├── protein_quant_current_normalized.csv.gz
│   └── * gene_x_cell_line.tsv
├── rna
│   ├── CCLE_expression_full.csv
│   └── * gene_x_cell_line.tsv
|── rnai
|   ├── shRNAmapping.csv
|   ├── achilles55kbatch1repcollapsedlfc.csv
|   ├── achilles55kbatch2repcollapsedlfc.csv
|   ├── achilles98krepcollapsedlfc.csv
|   ├── drivepoolalfcmat.csv
|   ├── drivepoolblfcmat.csv
|   ├── D2_combined_gene_dep_scores.csv
|   └── * gene_x_cell_line.tsv
└── gene_set
    └── * gene_set_x_sample.tsv
```
