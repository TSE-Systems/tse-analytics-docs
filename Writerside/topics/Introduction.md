# Introduction
## Overview of TSE Analytics

TSE Analytics is a data analysis application designed specifically to work with the data output produced by
[TSE PhenoMaster](https://www.tse-systems.com/service/phenotype/) software. It allows a simplified management of
multiple datasets, data sharing and reproducibility of experimental results in a flexible and user-friendly way.

TSE Analytics offers a wide range of tools for easy and convenient processing of large datasets. These include:

- **Integrated Data Handling**: TSE Analytics is designed to manage complex datasets like PhenoMaster data and integrates data processing, visualization, and statistical analysis.
- **Flexible Data Customization**: The software allows users to tailor data structures to their specific needs by, for example, excluding outliers, defining time frames, merging multiple datasets, and creating new grouping factors.
- **Automated Data Management**:TSE Analytics facilitates multi-dataset management with automatic metadata extraction and dataset processing options.
- **Dynamic Visualization**: TSE Analytics allows to quickly visualize data over time using the plot function and quickly screen and compare data across different groups, individual animals, or specific time periods.
- **Comprehensive Statistical Analysis**: The software includes a broad range of statistical tools, from data exploration to advanced analyses.
- **User-Friendly, Flexible and Efficient**: TSE Analytics stands out for its ease of use and extensive analytical capabilities combined with various export functions.
- **Reproducibility and Collaboration:** By using TSE Analytics, researchers can generate standardized output reports to ensure the reproducibility and comparability of research findings.

## Data Visualization and Statistical Analysis

TSE Analytics hosts various options for data analysis and visualization:

- **Timeline Visualization**: Visualize raw data on a timeline or in time bins with the possibility to easily switch between individual animals or apply grouping by factors or runs.
- **Explorative Analysis**: Assess and visualize data distribution of selected variables using histograms, violin or box plots, and normality analysis with the possibility to apply grouping by animal, factor or run.
- **Bivariate Analysis:** Calculate correlations between two variables using correlation or linear regression analysis.
- **AN(C)OVA**: Perform several types of ANOVA (N-way, repeated measures, mixed design) or ANCOVA under consideration of factors and time bins.
- **Multivariate and High-Dimensional Analysis**: Visualize and analyze correlations between multiple variables using matrix plots and dimensionality reduction techniques such as PCA and t-SNE.
- **Time Series Analysis:** Perform time series analysis to detect patterns or trends in PhenoMaster data collected at regular time intervals.
## Main Window

Main window of TSE Analytics is a host of multiple dockable widgets. Users may resize, move and organize the layout
of the main application window up to their liking. Users can hide/show some widgets by using **View** section
in the main menu.

The layout is saved when you quit application.

> Default layout may be restored by clicking **View - Reset Layout** menu item.

![main.png](main.png)


## Data structure organization in TSE Analytics

All data in the application are organized in the following manner:

```
├── Workspace
│   ├── Dataset 1
│   │   ├── Metadata 1
│   │   ├── Animals set 1
│   │   ├── Variables set 1
│   │   ├── Factors set 1
│   │   ├── Settings 1
│   ├── Dataset 2
│   │   ├── Metadata 2
│   │   ├── Animals set 2
│   │   ├── Variables set 2
│   │   ├── Factors set 2
│   │   ├── Settings 2
│   ├── Dataset ...
│   │   ├── Metadata ...
│   │   ├── Animals set ...
│   │   ├── Variables set ...
│   │   ├── Factors set ...
│   │   ├── Settings ...
```

Top level data structure is a *Workspace*. It can contain one or many datasets.

Each *dataset* represents a single imported CSV data file from TSE PhenoMaster software. All relevant metadata
extracted during import procedure (e.g. sampling time, animals and variables lists, etc.) Each dataset contains a set of
its own settings. After initial import, dataset is assigned an experiment *Run* number **1** by default.

In order to import dataset, please click **File - Import Dataset** command. As soon as data from CSV file are imported,
you will see a new entry in the *Datasets* widget. By selecting specific entry in this widget, one can switch freely
between different datasets:

![datasets.png](datasets.png)

> **Note:** Only one dataset can be active at the time in the workspace!

When dataset is selected, all other widgets will be updated accordingly: for example, **Info**, **Animals**,
**Variables** and **Factors** widgets will show information relevant to the active (currently selected) dataset.

Let's have a look at the selection widgets.

### Animals

Here users can select one or many animals from the list of all animals that were registered in the experiment. This
allows to filter (exclude) some of them from further analysis and visualisation.

![animals.png](animals.png)

In order to select all animals at once, please press **CTRL-A** or drag mouse over entries you want to choose.
To select/deselect individual entries, click on the entry holding **CTRL** key.

> **Note**: When there is no selection in the animals list, it is considered as if all animals are selected!

### Variables

This widget is used to choose of one or many variables that you want to display in the **Data** widget table or
include in the downstream analysis in components that support multiple variables selection, like **Matrix** or **PCA**
widgets.

![variables.png](variables.png)

Similarly to **Animals** widget, in order to select all variables at once, please press **CTRL-A** or drag mouse over
entries you want to choose. To select/deselect individual entries, click on the entry holding **CTRL** key.

### Factors

![factors.png](factors.png)

## Data analysis pipeline

Almost all widgets (with some exceptions mentioned later) work with the preprocessed data that passed through the
internal data analysis pipeline.

1. Raw data first goes into *Animal Filter* pipe operator. This unit obtains data only for the selected set
   of animals. Animals can be selected in **Animals** widget.
2. Second step is the outliers removal in the *Outliers* pipe operator. This unit can be activated/deactivated in the
   **Outliers** widget (see details below).
3. Last step in the preprocessing data pipeline is *time binning* operation.

> **Note**: If you observe some strange results during your analysis, please check that proper animals are selected in
> **Animals** widget!
