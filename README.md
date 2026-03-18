# Single-cell RNA-seq Analysis of AML vs Healthy Pediatric Bone Marrow

## Overview

This project performs a comprehensive single-cell RNA sequencing (scRNA-seq) analysis to compare Acute Myelomonocytic Leukemia (AML) samples with healthy pediatric bone marrow controls. The analysis includes quality control, data integration, clustering, cell type annotation, differential expression, and functional enrichment.

## Workflow

### 1. Quality Control

* Assessed cell quality using gene counts, UMI counts, and mitochondrial gene expression
* Filtered out low-quality cells and technical artifacts
* Improved dataset consistency and removed potentially dying cells

### 2. Dimensionality Reduction and Clustering

* Performed PCA, UMAP/t-SNE, and graph-based clustering
* Observed batch effects before integration
* Applied data integration to correct batch effects
* Post-integration clustering reflects biological similarity rather than sample origin

### 3. Cell Type Annotation

* Identified clusters using canonical marker genes
* Annotated major hematopoietic cell types
* Generated annotation plots to visualize cellular composition

### 4. Differential Expression Analysis

* Used pseudobulk strategy per cell type
* Applied DESeq2 for AML vs control comparison
* Identified significant genes (adjusted p-value < 0.01, |log2FC| ≥ 1)
* Visualized results using volcano plots

### 5. Functional Enrichment Analysis

* Performed GO and KEGG enrichment analysis
* Analyzed T cells and GMP populations

Key findings:

* T cells: enrichment in mitochondrial activity, oxidative phosphorylation, and immune signaling
* GMP cells: enrichment in cell cycle, DNA replication, and proliferation pathways

## Key Insights

* AML samples show altered immune cell function and metabolic reprogramming
* Myeloid progenitor cells exhibit increased proliferation activity
* Distinct biological programs differentiate AML from healthy bone marrow

## Tools and Technologies

* R
* Seurat
* DESeq2
* GO / KEGG enrichment

## Results

* UMAP clustering (before and after integration)
* Cell type annotation plots
* Volcano plots
* Enrichment analysis visualizations

## Conclusion

This analysis highlights major transcriptional and functional differences between AML and healthy bone marrow at the single-cell level, providing insights into disease biology and cellular heterogeneity.
