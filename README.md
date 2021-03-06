# Bioinformatics tutorial
## Introduction
This tutorial introduces you to the world of single cell RNA-seq (scRNA-seq) data analysis.   

### Contents
This tutorial includes how to:
1. manipulate scRNA-seq data with Python
2. pre-process the data
3. reduce the dimension of and cluster the data
4. find marker genes of cell types and annotate clusters

### Goals  
Through this tutorial, you can learn:  
1. how to process and analyze scRNA-seq data with Python   
2. to what extent your choice of methods for pre-process and analyses affects outcomes
3. how algorithms behind tools work  
4. how easily artifacts arise  

### Requirements  
Before beginning the tutorial, please set up your envirionment.  
1. Install Python (>= ver. 3.6)
2. Install the following libraries:  
` numpy pandas matplotlib scanpy seaborn louvain leidenalg`    
If you manage your environment with conda, I'd recommend you to add these channels before installation:  
` conda config --add conda-forge`  
` conda config --add bioconda` 
3. Make sure you can use jupyter notebook. 

If you have any trouble setting up your environment, feel free to ask me!

### Data
**I processed and uploaded the data we use [here](https://drive.google.com/drive/u/1/folders/17x4THurk7woJsXdYMadzTPBHBCaYzQ7w).**  
**Please download and decompress the data in advance.**  
If you are interested in the original, raw data, please go [here](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE117498).  
This website is called Gene Expression Omnibus (GEO), which is one of the most popular database for gene expression data.  
For now, I processed the original, raw data to save time, but when you want to use any data uploaded on a database, you need to download and process it yourself somehow.  
That is often VERY time-consuming and not cool (but the real bioinformatics).  


---  

## Key papers
### Data

* [A comprehensive single cell transcriptional landscape of human hematopoietic progenitors](https://www.nature.com/articles/s41467-019-10291-0)  
Pellin, D. et al., 2019, Nature Communications  

### Tool

* [SCANPY: large-scale single-cell gene expression data analysis](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-017-1382-0)  
Wolf, F. A. et al., 2018, Genome Biology

* [PAGA: graph abstraction reconciles clustering with trajectory inference through a topology preserving map of single cells](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1663-x)  
Wolf, F. A. et al., 2019, Genome Biology  

* [Comparative single-cell trajectory network enrichment identifies pseudo-temporal systems biology patterns in hematopoiesis and CD8 T-cell development](https://www.biorxiv.org/content/10.1101/2020.04.02.021295v3)  
Grønning, A. G. B., et al., 2020, bioRxiv  

### Algorithm  

* [From Louvain to Leiden: guaranteeing well-connected communities](https://www.nature.com/articles/s41598-019-41695-z)  
Traag, V. A. et al., 2019, Scientific Reports  
I'd recommend you to read the introduction of this paper, which is well-written and very cool!  
* [UMAP does not preserve global structure any better than t-SNE when using the same initialization](https://www.biorxiv.org/content/10.1101/2019.12.19.877522v1)  
Kobak, D & Linderman, G. C., 2019, bioRxiv 

## Key websites

* [Scanpy tutorials](https://scanpy-tutorials.readthedocs.io/en/latest/index.html)

* [Ensembl](https://asia.ensembl.org/)  
* [Scellnetor](https://exbio.wzw.tum.de/scellnetor//)

## Further reading
* [SPRING: a kinetic interface for visualizing high dimensional single-cell expression data](https://academic.oup.com/bioinformatics/article/34/7/1246/4708233)  
Weinreb, C. et al., 2018, Bioinformatics  
* [Fundamental limits on dynamic inference from single-cell snapshots](https://www.pnas.org/content/115/10/E2467)  
Weinreb, C. et al., 2018, PNAS  
* [Population snapshots predict early haematopoietic and erythroid hierarchies](https://www.nature.com/articles/nature25741)  
Tusi, B. K. et al., 2018, Nature  
* [Structure-Aware Data Consolidation](https://ieeexplore.ieee.org/document/8046026)  
Wu, S. et al., 2018, IEEE Transactions on Pattern Analysis and Machine Intelligence
