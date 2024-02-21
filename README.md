# Xenium-Data-analysis

This repo consists of data-analysis conducted by Xenium 10x Genomics in correspondance with Bioturing Inc. and Cleveland Lab at UC San Diego. The data analyzes 2 different types of mouse, control mouse and mouses that exhibit Huntington's disease.

#### The following are the sample ids of the mouses analyzed (3 - 3 month old control mouse) (3 - 24 month old control mouse) (3 - 24 month old huntington mouse) (1 - severe huntington mouse):
- C3m1
- C3m2
- C3m3
- C24m1
- C24m2
- C24m3
- HD24m1
- HD24m2
- HD24m3
- R61

#### This repo consists of the following notebooks:
- Xenium UMAP - all mouse
    - a compilement of data analysis of all Xenium mouses. It includes a generation of UMAP for all samples together as well as all samples individually. It also includes a cell type heatmap that is used to label cell types of the umap. It also includes bar charts that indicate the gene expression of teh top 20 genes in each cluster
        
- Xenium - Generate umaps and cell type labeling
    - Generate the umap of all mouses together, generate the cell type bubble heatmap based off the Allen Brain Atlas cell type database. Generate the cell type umap of the mouses toghether. Generate umap for each invididual mouse
    
- Xenium - Generate gene expression bar graphs
    - This notebook looks that the top 20 expressed genes in each cluster of the umap. It looks at the number of transcripts per cell, and incluses 2 types of graphs, top 20 expressed genes based on raw counts and top 20 expressed genes based on raw counts normalized. It is normalized by the number of transcripts in each cluster.
    
- Xenium Subclustering and PCA analysis
    - This notebook looks at select clusters of the umap and increases resolution to generate more clusters within that particular cluster. A cell type heatmap is also generated to confirm cell type. A PCA analysis was then conducted based on condition (i.e. Control, Huntington, Severe Huntingon)
    
- Xenium - Find mean cell size, sensitivity chart, specificity chart
    - This notebook pulls from the raw Xenium data to find the mean cell size in microns of all cells in the Xenium dataset. A sensitivity chart was then generated to show the number  of cells that consists of how many particular transcripts.