# Visualizing high-dimensional biological data with Clustergrammer-Widget in the Jupyter Notebook

Nicolas Fernandez: Icahn School of Medicine at Mount Sinai

github: cornhundred

### Presenter went wayyyyy too fast to write effective notes, managed to steal the slides though:
[Presentation Slides](http://bit.ly/clustergrammer-jupytercon)

[Clustergrammer Github](https://github.com/MaayanLab/clustergrammer)

[Clustergrammer Demonstration](https://github.com/MaayanLab/clustergrammer-widget/blob/master/README.md)

[Presentation Notebook](http://nbviewer.jupyter.org/github/MaayanLab/CCLE_Clustergrammer/blob/master/notebooks/Tissue_Specific_Viz.ipynb)

>Biological data and other data collected from complex systems can have tens of thousands of variables that interact nonlinearly. Interactive visualizations enable users to develop an intuition about the global structure of their data and immediately identify patterns. While dimensionality reduction techniques are useful for obtaining a bird’s eye view of data, these techniques often obscure important information. Heatmaps, or clustergrams, are powerful alternative but complementary visualization techniques for directly visualizing all variables from high-dimensional data. While there are many software tools that can generate clustergrams, few are web based, fully interactive, or seamlessly integrated into Jupyter notebooks.

>Nicolas Fernandez offers an overview of Clustergrammer-Widget, which enables users to easily visualize high-dimensional data (e.g., a pandas DataFrame) within a Jupyter notebook as an interactive hierarchically clustered heatmap. Clustergrammer-Widget generates highly interactive visualizations (e.g., reorderable and zoomable) that can be embedded within notebooks and shared using nbviewer. Clustergrammer-Widget was developed to analyze high-dimensional biological data but can be applied to any high-dimensional data from other fields. Nicolas explains how to use Jupyter notebooks and Clustergrammer-Widget to produce transparent and reproducible analyses for a wide variety of biological datasets and demonstrates how to share your results with collaborators.

Previous examples are with interactive D3.js plots

## Biological data can be difficult to visualize

Can be very high-dim
* RNA-seq proteomics

## Dimensionality Reduction two techniques are useful
* t-SNE


## Heatmaps and clusterframs enable direct visualization of high dim data

* Clustergrams expand on heat maps 
* built with D3.js front
* python back end


Clustergrammer-widget can be thought as a pandas dataframe visualizaer

[REGL - GPU Accelerated WebGL](http://regl.party/)
