# Import of Datasets

**1.** **Export data from PhenoMaster software**

TSE Analytics only supports TSE Dataset files (\*.tse), which are experimental date files exported from PhenoMaster Software Version **_(????? -> insert latest version number)_** or higher using the dedicated data export function for TSE Analytics.

**_(to be added: explanation and screenshots on how to export datafiles from phenomaster -> ask anton or knut)_**


**2.** **Import Datasets into TSE Analytics**

Datasets exported from PhenoMaster Software as described above (file ending **\*.tse**)can be imported into TSE Analytics via **File** – **Import Dataset** in the header or via the **Import Dataset** button. The \***.tse** dataset exported from the PhenoMaster software can then be selected in the _File Explorer_ and is loaded into TSE Analytics upon clicking **Open**.

If binary files containing Drink/Feed data (DrinkFeed bin data) or calorimetry data (Calo bin data) or ActiMot raw data should be imported into TSE Analytics together with the main table, the respective file types can be selected from the _Data Import_ popup window which appears after opening a \*.tse file and needs to be confirmed by clicking **OK.**

After successful import, the dataset will appear in the _Dataset_ widget. The dataset will only be displayed if the _Dataset_ widget is activated (indicated by checked tick box) under **View**.

Multiple datasets can be imported into TSE Analytics one after the other, but not simultaneously. Each dataset which has been loaded into TSE Analytics becomes part of the current _Workspace_ and contains a set of individual settings. All relevant metadata, such as sampling intervals, animal information and variables list are extracted automatically during import individually for each dataset. There is no limit to the number of datasets that can be loaded into a workspace.

A dataset can be selected for data processing and analysis by clicking on the respective dataset in the _Dataset_ widget. The active dataset is then highlighted in blue, and all other widgets will be updated accordingly.

**Note:**

- Only one dataset can be active (highlighted in blue) at one time in the workspace.
- Selecting a dataset and working with the respective data is only possible if the _Dataset_ widget is visible. Therefore, please ensure to tick **Datasets** in the _View_ settings located in the header when importing new datasets or switching between datasets.



