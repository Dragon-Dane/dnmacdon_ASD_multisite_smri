# Brainhack School 2020
## Week 3 Interactive Visualization Assignment
David MacDonald

## Background
This project uses a version of [ComBat](https://github.com/jfortin1/ComBatHarmonization) to harmonize site differences in multi-site structural MRI data, in this case from a subset of the [ABIDE](http://fcon_1000.projects.nitrc.org/indi/abide/) autism dataset. The scans were preprocessed and segmented using [MAGeT Brain](https://github.com/CobraLab/MAGeTbrain). The volumes of the thalamus, globus pallidus, and striatum, as computed by MAGeT Brain, are the input data here.

The interactive visualizations produced here would be used to verify and explore the data. You can explore scatter plots of subcortical volumes against age and total brain volume, you can see the distributions of these volumes both before and after harmonization, and you can examine the fitted-values vs. residual plots of the site-harmonized volumes regressed on age and diagnosis.

## Instructions
Run the notebook Week3-InteractiveVisualization.ipynb:
 1. Clone this repository or download the contents of this directory. It includes the data (data_trimmed.csv), and a conda environment file (harmonization.yml) with the required dependencies, and the Jupyter Notebook (Week3-InteractiveVisualization.ipynb).
 2. Create and activate a conda environment using harmonization.yml

```
conda env create -f harmonization.yml
conda activate harmonization
```

 3. Open the jupyter notebook

```
jupyter notebook Week3-InteractiveVisualization.ipynb
```

 4. Run all cells (Cell menu -> Run All)

The interactive visualizations are in the bottom cells. They present seaborn-based graphs. You can select the specific structure you wish to view, and, on one visualization, choose what data is used to colour the points (diagnosis or site).

