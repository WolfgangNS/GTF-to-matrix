# GTF-to-matrix
Downloads gtf files from NCBI, uses mappings to convert Entrez to Ensembl, and and returns matrix of TPM counts.

This project was heavily inspired by my undergraduate research capstone, assigned to me by my PI. In that project, we used RNA-Seq data to find gene expression differences between dominant and subordinate males in a highly competitive social fish tank, with a highly competitive species, Astatotilapia Burtoni. In this Github repository, I am seeking to parallel that project to showcase my abilities while foregoing data leaks before the lab publishes their findings.  

<div align="center"><img src="Colab notebook screenshot.PNG" style="width:50%;height:50%"></div>

<div align="center"><img src="Full WGCNA workup of mouthbrooding females.png" style="width:50%;height:50%"></div>


# Features
## Python notebook
* Download annotations from BioMart
* Download NCBI data
* Generate gene expression matrix from GTF files using HTSeq
* Download and parse MINiML file into TSV format

## R Notebook
* Generate DESeq pathway enrichment diagram via KEGG
* Download annotations via Bioconductor's AnnotationHub
* Construct WGCNA network
* Analyze correlations between WGCNA modules and traits
* Enrich module genes via ClusterProfiler
* Visualize membership of module eigengenes for each sample using a heatmap and bar chart
* Plot network graphs via ggraph to visualize coexpression patterns
