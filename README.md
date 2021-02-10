# 2021Workshop-COVID19

## Single-cell COVID-19 data visualization

According to the United Nations, in the last years, the world has shown an increase in population aging and, as a consequence, chronic age-related diseases. From a national perspective, chronic diseases have severe implications in life expectancy and, as a result, generate economic and political pressures. This year with the COVID-19 pandemic, we have been trying to understand if survivors who have been seriously ill will have some sequelae such as pulmonary fibrosis, an irreversible chronic disease. High-throughput technologies have evolved too fast in the last years, and nowadays, single-cell RNA sequencing has become more popular because of the amount of information that we can obtain measuring thousands of single cells in one experiment. This project is focused on analyzing published single-cell data of COVID-19 and look if we can find some known biomarkers of pulmonary fibrosis. We will try classical visualization tools for single-cell data using R packages, but we will be creative and find new ways of visualizing data for finding patterns. Our main objective would be to guide hypothesis generation through the visualization of single-cell COVID data.

*Goal*: Visualization of single-cell COVID data for hypothesis generation.

  Some objectives are: 

    a) To manipulate single cell data formats and incorporate into R

    b) To learn different packages for analyzing single cell data

    c) To explore different types of visualization for single cell data

    d) To find cell type biomarkers

    e) To compare COVID biomarkers with those from pulmonary fibrosis

    f) To work as bioinformatic team 

    g) To incorporate and exchange information with other teams

    h) To present the results

-[Slides-Yalbi](https://www.canva.com/design/DAEVZWNn890/GIpO6ArnfLEjl0Vn2FlYBQ/view?utm_content=DAEVZWNn890&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton)

- [Slides](https://www.canva.com/design/DAEVYuo3T18/hsrXi3SWhVBEzciYZpk8ww/view?utm_content=DAEVYuo3T18&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton)


## Data 

- **Paper:**  [ Authors: Chua, R.L., Lukassen, S., Trump, S., Hennig, B.P., Wendisch, D., Pott, F., Debnath, O., Thürmann, L., Kurth, F., Völker, M.T. and Kazmierski, J., 2020. COVID-19 severity correlates with airway epithelium–immune cell interactions identified by single-cell analysis. Nature biotechnology, 38(8), pp.970-979.](https://www.nature.com/articles/s41587-020-0602-4)

- **Tissue:** BALF

- **Data type:** scRNA-seq 

- **Samples:** 5 Controls and 19 COVID19 patients

- **Download data:** [Data](https://figshare.com/articles/dataset/COVID-19_severity_correlates_with_airway_epithelium-immune_cell_interactions_identified_by_single-cell_analysis/12436517) has already been downloaded in the server (kneipe.lavis.unam.mx). You can find it in the directory:

      /home/bana/balf_human_Chua 

- **Raw sequencing:** https://ega-archive.org/datasets/EGAD00001006339/files

------

## Resources

Useful resources:

### singleCell RNA-seq

- [Seurat](https://satijalab.org/seurat/)

- [Seurat-Clustering_Tutorial]( https://satijalab.org/seurat/articles/pbmc3k_tutorial.html)

- [Seurat-Visualization_Tutorial](https://satijalab.org/seurat/articles/visualization_vignette.html)

- [Seurat Command list](https://satijalab.org/seurat/articles/essential_commands.html)


### Visualization

- [Data-to-viz](https://www.data-to-viz.com/): The most appropiated graph for your data

- [The R Graph Gallery](https://www.r-graph-gallery.com/)

- [R2D3](https://blog.rstudio.com/2018/10/05/r2d3-r-interface-to-d3-visualizations/): R interface to D3 visualizations

- [plotly](https://plotly.com/r/)

## Enrichment analysis 

- [hyperR](https://montilab.github.io/hypeR-workshop/articles/hyper_workshop.html)

- [TopGO](https://bioconductor.org/packages/release/bioc/html/topGO.html)

## Co-expression networks 

- [CoDiNA](https://deisygysi.github.io/rpackages/Pack-2)


## Others

- [Basic concepts](https://www.lecturio.com/)

## Pulmonary fibrosis 

- [Wijsenbeek, Marlies, and Vincent Cottin. "Spectrum of fibrotic lung diseases." New England Journal of Medicine 383.10 (2020): 958-968.](https://www.nejm.org/doi/full/10.1056/NEJMra2005230?casa_token=LUjzzYwonSUAAAAA:4P5vQva0tnVikeKH34AhyhzLzkgQ5oIKnGz2n2ko3JQWBZ1ys33e6oOMvNqR9tkxYvqkemGDPJWcTdRvqw)

- [Lopez-Leon, Sandra, et al. "More than 50 Long-term effects of COVID-19: a systematic review and meta-analysis." Available at SSRN 3769978 (2021).](https://www.medrxiv.org/content/10.1101/2021.01.27.21250617v2)


------

## Activities

### Day 2

- Import `.RDS` object into R

- Explore the `balf_human_Chua/covid_nbt_loc.rds` and `balf_human_Chua/covid_nbt_main.rds` objects and decide which one to use

- Plot a PCA, tSNE and UMAP. Discuss the results

- Is there any better visualization for the output of `VizDimLoadings(pbmc, dims = 1:2, reduction = "pca")`?

- Can you reproduce the UMAP [Fig 2](https://www.nature.com/articles/s41587-020-0602-4/figures/2) from the paper?

### Day3

1) Creativity to propose different visualization plots (Leo)

2) Pulmonary Fibrosis in COVID-19: Biomarkers of Pulmonary fibrosis (Saul)

3) Enrchiment analysis in scRNAseq data of COVID-19 (Basal, Ciliated, and Macrophages)  (Ana, Juwy)


------

## Additional data

- **Paper:**  [Wauters, E., Van Mol, P., Garg, A.D., Jansen, S., Van Herck, Y., Vanderbeke, L., Bassez, A., Boeckx, B., Malengier-Devlies, B., Timmerman, A. and Van Brussel, T., 2021. Discriminating mild from critical COVID-19 by innate and adaptive immune single-cell profiling of bronchoalveolar lavages. Cell research, pp.1-19.](https://www.nature.com/articles/s41422-020-00455-9)

- **Tissue:** BALF

- **Data type:** scRNA-seq and scTCR-seq

- **Samples:** 13 non-COVID19 (with pneumonia) and 22 COVID19 patients

- **Raw sequencing:** https://www.ebi.ac.uk/ega/studies/EGAS00001004717

- **Count matrix:** http://covid19.lambrechtslab.org/




