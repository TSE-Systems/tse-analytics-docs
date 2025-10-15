# Data Export

TSE Analytics offers multiple options for data export depending on the data format and the user’s preferences.

## Export of Data table

The data table of the active dataset including all variables can be exported using text (.csv) or Excel (.xlsx) format via **Export | Export to CSV** or **Export| Export to Excel** in the header.
After setting the file destination and file name in the File Explorer, the data table is stored at the selected destination by clicking **Save**. 

![Figure: Export of Data Table](Export of Data Table.png)

This data export option will save the current version of the active data table under consideration of changes that have been made using TSE Analytics. Changes considered for the exported data table include merging of datasets, exclusion of animals and animal selection in the animals list via checkboxes, exclusion of time phases and adjustment of time, editing of animal information or factors, time binning and removal of outliers.

> **Important**: Variable selection and Split Mode selection in the Table control panel do not affect the content of the exported data table, but only the way data is displayed in the Table widget.
> The exported data table always contains all variables extracted from the PhenoMaster file and data for individual animals (as for Split Mode “By Animal”).
>
> Similarly, sorting of data entries in the Table widget will change the order of data entries displayed under Table, but will not affect the exported data table.
{style='warning'}

##  Export of Raw Data Plots

First, ensure that your **main window** is displaying the plot you wish to export. For instructions on how to display data plots, refer to the chapter of this manual **Import|Data Overview and Visualization**

![Figure: Data Plot](Data Plot.png)

Once the plot is visible on your desktop, move the mouse cursor over the plot and **right-click**. This allows you to customize the display mode of the plot.

### Plot Export Options

![Figure: Raw data plot export](raw-data-plot-export.png)

In the **Plot Export** menu, you will find several options for exporting or customizing your plots:  

- **CSV of Original Plot Data** – Exports the raw data used to generate the plot in CSV format.  
- **Image File** – Exports the plot as an image file (e.g., PNG or JPEG).  
- **Matplotlib Window** – Opens the plot in a separate **Matplotlib** window, allowing further customization and editing.  
- **SVG** – Exports the plot as a scalable vector graphic file.  

#### Matplotlib Window

![Figure: Matplotlib Window](Matplotlib Window.png)

When selecting **Matplotlib**, the plot opens in a standalone Matplotlib interface where you can modify and refine its appearance in greater detail.  
The toolbar at the top of this window provides several useful tools, listed from left to right:  

![Figure: Matplotlib Toolbar](Matplotlib Toolbar.png)

- **Home (House icon)** – *Reset View.* Restores the plot to its original appearance after any modifications.  
- **Back/Forward (Arrow icons)** – Navigate backward or forward through previous plot views or edits.  
- **Pan (Crossed arrows icon)** – Enables panning and zooming of the entire plot. Click and drag to move the plot or adjust the zoom level.  
- **Zoom (Magnifying glass icon)** – Allows zooming into a specific area of the plot. After selecting this tool, the cursor changes shape; click and drag to define the region to magnify.  
- **Configure Subplots (Three horizontal bars icon)** – Opens the subplot configuration panel, allowing you to adjust the overall layout, including figure size, margins, and spacing.  

![Figure: Configure Subplots](Configure Subplots.png)

- **Edit Plot (Upward arrow icon)** – Opens the plot editor, where you can customize X- and Y-axis parameters such as range limits, scaling, and axis labels. 

![Figure: Edit Plot](Edit Figure.png)

- **Save (Floppy disk icon)** – Opens the save dialog, allowing you to select an output format (e.g., JPG, PNG, PDF) and specify the file version or name.  

![Save Dialog.png](Save Dialog.png)

This option is particularly useful when you need to refine or customize the visual presentation of your data plot before the final export.

## Export of Data from the Exploration, Bivariate, Dimensionality and Timeseries Widgets

Export of analysis results and graphs works in the same way for the _Exploration_ widget (histograms, violin plots, box plots and normal probability plots), _Bivariate_ widget (correlation and regression analysis) and the _Timeseries_ widget. 

Each widget contains a plot menu in the bottom right corner of the control panel including a **Save button** (‘Memory card’ symbol).
By clicking the **Save** **button**, a _File Explorer_ window opens, in which file destination, file name and format can be selected.
Clicking **Save** will store the graphic file at the selected location.

![Figure: Saving plots](saving-plots.png)

## Export of AN(C)OVA Results and Bivariate Analysis Tables

TSE Analytics does not offer a dedicated export function for AN(C)OVA or bivariate analysis (correlation and regression) result tables so far.
However, results can be saved outside TSE Analytics via copy and paste.
All analysis results can be selected by clicking on the data table and pressing <shortcut>Ctrl+A</shortcut> on the keyboard or by **right-clicking** on the analysis window and selecting **Select All**.
Selected content can then be copied to the clipboard using <shortcut>Ctrl+C</shortcut> or by right-clicking on the analysis window again and selecting **Copy**.
Content copied to the clipboard can then be pasted and saved outside TSE Analytics.

![Figure: Copy & Paste] (copy-paste.png)

## Export of Data via Report

In addition to specific export options which vary between different analysis and plots, all results can be saved within a workspace and outside of TSE Analytics using the **Add Widget | Utils | Report** widget. 

- Result tables and graphs can be added to the Report by clicking Add to Report at the bottom of the control panel of the respective widget. 

![Figure: Adding to report](add-to-report.png)

- In addition, the Report works as a text editor and allows adding customized text to analysis results. 

![Figure: Editing report](editing-report.png)

Each dataset has an individual report, and all reports are saved within a workspace in TSE Analytics when saving the workspace. 

The Report menu offers several tools for editing the report and text elements (from left to right):

- Undo/Redo
- Cut/ Copy/ Paste
- Selection of text font
- Selection of text size
- Text style: Bold/ Italic/ Underline
- Content alignment: Left/ Center/ Right/ Justify

![Figure: Report toolbar](report-toolbar.png)

Each dataset has an individual report and all reports are saved within a workspace in TSE Analytics when saving the workspace.

Reports can also be saved outside of TSE Analytics as an .html file by clicking on the **Save** button (‘Memory disk’ symbol) in the Report menu.

![Figure: Saving report](saving-report.png)

Reports can also be printed by clicking on the **Print** button (‘Printer’ symbol) in the Report menu.
If **Microsoft Print to PDF** is selected under **Printer** in the printing settings, reports can thereby also be saved as .pdf files.

![Figure: Printing report](printing-report.png)

All entries of an existing report are cleared by clicking the **New Report** button (‘Sheet’ symbol) on the left of the report menu.

![Figure: New report](new-report.png)

> **Warning**: This action cannot be undone! Clicking **New Report** will definitively delete all previous content from the report.
{style = 'warning'}
