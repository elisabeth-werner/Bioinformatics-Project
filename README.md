# Comparative Pan-Cancer Analysis Reveals Pathway Signatures Distinguishing Lung Adenocarcinoma from Squamous Cell Carcinoma


## Analysis of Pan-Cancer expression with focus on LUAD

The project aimed to compare gene expression and pathway regulation in different types of cancer. First, gene expression data and pathway regulation for 33 different tumor types were compared using the "tcga_exp" data set (pan-cancer analysis). Subsequently, the data were specifically analyzed for lung adenocarcinoma (LUAD) using the "LUAD" data set. Both data sets underwent preprocessing and descriptive analysis.

To identify further interesting gene sets, a gene set enrichment analysis (GSEA) was performed on oncogenic signature gene sets from Molecular Signatures Database (MSigDB). The gene sets that were most variant in the average LUAD patient (23 new gene sets) were added to the data set of the hallmark gene sets. A gene set variation analysis (GSVA) was performed on all of these gene sets to identify differences and similarities between the tumor types. Additionally, hierarchical clustering and Uniform Manifold Approximation and Projection (UMAP) analysis were used to identify different groupings within the data.

Similar analysis methods were applied to LUAD-specific data, including gene set enrichment analysis (GSEA) and UMAP. Based on these studies, the tumor types LUAD and lung squamous cell carcinoma (LUSC) were specifically compared. This comparison formed the basis for logistic regression, allowing non-small cell lung tumor tissue to be assigned to either LUAD or LUSC.

### cloning of repository and data preparation

First, clone the repository using the following link:

<https://github.com/datascience-mobi-2024/topic02_03>

Download the data files and safe them in the “data” folder:

hallmark gene sets: <https://figshare.com/s/4f917a4f41e90027dd6f>

tcga_exp: <https://figshare.com/s/3c2bf4d766181a17a2e0>

tcga annotations: <https://figshare.com/s/eed44ff6fdcf451cebd9>

luad: <https://figshare.com/s/3b9aa021a5cebc249ffa>

You need to make sure that you can easily access the data after that. Therefore, you will create a new project in the repository. Accessing all data and files by relative paths is possible.

### Repository organization

**1. Preprocessing:** The pan-cancer (tcga_exp) and luad-specific data sets were used for data cleaning, dimension reduction using PCA & UMAP.

**2. Gene sets:** The Genesets were compared using the Jaccard index.

**3. PanCancer:** GSVA and visualization of pathway activities were performed.

**4. LUAD:** A Volcano plot was computed as a descriptive analysis. GSEA and visualization of pathway activities were performed.

**5. Regression:** GSVA on only LUAD and LUSC was calculated. Based on this a logistic regression model was implemented, which can distinguish these non-small cell lung carcinoma.

**6. Protocol:** Within the protocol there are the figures used in the report and the sources.
