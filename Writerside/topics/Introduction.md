# Software overview
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




