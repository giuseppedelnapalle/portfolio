# Portfolio

## [Project 1: Single-cell mean rank gene set scoring method for comparing gene set activity](https://github.com/giuseppedelnapalle/scmrgss)
* Created a straightforward yet informative method called single-cell mean rank gene set scoring (scMRGSS) to compare gene set activity between cell types from either identical or distinct sources using single-cell RNA-seq (scRNA-seq) data.
* Average rank of gene expression is calculated for each gene set (pathway) of interest, followed by normalisation based on the number of expressed genes. 
* Robust to common gene expression normalisation and transformation methods, such as counts per million (CPM), log-transformed CPM, so long as the rank data is preserved.
* Demonstrated its efficacy through both simulated and real-world datasets.
* Applied scMRGSS to glioblastoma data to prove its utility and found cellular heterogeneity in NF-κB pathway activity in glioblastoma.
* Developed utility tools to import and process H5AD, H5, and Loom files to facilitate building analysis workflow as well.
* The program is implemented in Julia.
* [Preprint available](https://doi.org/10.51094/jxiv.580).

<img src="img/scmrgss/heatmap_prop_diff_scores_jk_293t_kegg_jurkat-293t_jurkat-293t-jurkat_293t_50_50-jurkat_293t_99_1_0.6_1.15_2000_2_upd_v1.6.5.jpg" alt="heatmap_prop_diff_jk_293t" width="700"/>

**Figure 1**. Propotions of differential KEGG gene sets between cell lines from four separate datasets.

![violin_box_bt346_trg_nfkb](img/scmrgss/violin_box_plot_BT346.filtered_Mesenchymal_fetal_brain_tRG_ctx_dev_tRG_BIOCARTA_NFKB_PATHWAY_mdf.jpg)

**Figure 2**. NF-κB pathway activity of mesenchymal glioblastoma cancer cells in sample BT346 and truncated radial glia (tRG) from two fetal brain development datasets estimated by scMRGSS.
