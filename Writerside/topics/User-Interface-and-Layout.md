# User Interface and Layout

This chapter provides a comprehensive overview of the TSE Analytics software user interface and layout and its possibilities for customization. The software interface includes the header and toolbar together with the main window, which is comprised of several movable widgets. For detailed instructions on the functionality of specific widgets, please refer to the subsequent chapters of this manual.

![Overview of the software interface (default layout) and available widgets.png](Overview of the software interface (default layout) and available widgets.png)

*Figure : Overview of the software interface (default layout) and available widgets*

**1.** **Header and Toolbar**

The _header_, located at the top of the TSE Analytics interface, comprises file import and export functions under **File** (see also 4. Import and Export of Data), view settings under **View** and access to additional information and support under **Help**

![Header.png](Header.png)


**File**
- Open Workspace/ Open Recent: Open an existing (recently used) workspace.
- Save Workspace: Save the current workspace.
- Import Dataset: Import an individual dataset.
- Export to CSV/ Excel: Export data as .csv/ .xlsx file.
- Exit: Close the application.

>**Warning**: “Exit” will save any changes regarding the software layout but will not automatically save the workspace or any other changes.{style='warning'}



**View**

- Show/Hide Tool Panels: Customize the interface by de-/activating individual widgets.
- Reset layout: Restores initial layout with all widgets activated.

**Help**

- Help: Access support resources.
- About: View information about the software version, access to open-source code, license agreement and third-party libraries.

The _toolbar_ contains three shortcut buttons:

- **Open Workspace**: Open a previously saved workspace to continue your analysis.
- **Save Workspace**: Save your current workspace, including all datasets, respective settings and reports.
- **Import Dataset**: Import individual datasets into the current workspace for analysis.
- 
![Toolbar.png](Toolbar.png)

In the initial layout, the toolbar is located underneath the header. It can be detached from the main window or moved to the bottom, left- or right-hand side of the main window via drag and drop by clicking and holding the **dotted area** of the toolbar.

![Detaching and moving the toolbar.png](Detaching and moving the toolbar.png)

The toolbar can be activated or deactivated by selecting or deselecting the _ToolBar_ **check box** which appears when **right-clicking on the header/ toolbar area**.

**2.** **Main Window Interface**

The main window of TSE Analytics is a host of multiple dockable _widgets_. The widgets and their functionality are:

- **Datasets**: Provides an overview of all imported, cloned and merged datasets and options for data preprocessing (Adjust, Remove, Clone, Merge).
- **Info**: Displays general information about the selected dataset including animal information, variables, file name and data path, sampling interval and PhenoMaster version.
- **Help**: Upon clicking the ‘Help’ icon **‘(?)’**, further information, explanations and instruction for the respective software function are displayed here.
- **Log**: Error messages and warnings regarding the software code executed are displayed here. In case of any malfunction of the software, please inform TSE Systems about error messages shown here.
- [//]: # (TODO: Contact Information Link)
- **Variables**: This widget shows a list of all variables extracted from the selected data file. Time binning operations (Aggregation) per variable and outlier settings (outlier detection mode, sensitivity and variable selection) can be defined here.
- **Factors**: Animals can be grouped according to factors determined by the user. Factors can be created and edited in this widget and are listed together with their associated groups.
- **Binning**: Data can be binned over customizable time intervals. (De-)Activation of time binning and binning mode settings can be controlled in this widget.
- **Table**: “Table” provides a tabular representation of the selected dataset according to selected settings.
- **Plot**: “Plot” provides a graphical representation of the selected variable as a line plot or scatter plot over time or as bar plots if binning by light/ dark phases or custom time phases is applied
- **Exploration**: The “Exploration” tab contains several tools for exploratory data analysis including histograms, violin plots, box plots and QQ plots for normality testing.
- **Bivariate**: Using this widget, correlation and regression analysis can be performed.
- **AN(C)OVA**: The “AN(C)OVA” tab offers various options for ANOVA, including One-Way ANOVA, N-way ANOVA, repeated measures and mixed ANOVA as well as ANCOVA.
- **Dimensionality**: Tools for multidimensional analysis including matrix plots, principal component analysis (PCA) and t-distributed stochastic neighbor embedding (t-SNE) are provided here.
- **Timeseries**: PhenoMaster data collected over time can be analyzed for trends and patterns using time series analysis in this widget.
- **Report**: Analysis results and custom text can be added to the report. The “Report” tab shows the current report together with export options and editing tools.

Widgets can be detached (moved to a new application window), rearranged or grouped (combining multiple widgets in one window). Widgets can be reorganized by moving the widget via drag and drop (i.e. clicking on a widget header and holding while moving the widget until it has been moved to the desired location).

Each widget can also be detached or closed (deactivated) individually by **right-clicking** on the respective widget header and selecting **Detach** or **Close**.

![etaching and closing a widget via right-click.png](etaching and closing a widget via right-click.png)

*Figure: Detaching and closing a widget via right-click*

Similarly, groups can be detached or closed by **right-clicking** on the header of a group of widgets on the right side of the widget names (not on the widget name itself) and selecting **Detach Group** or **Close Group**. All widgets except for the selected group will be closed when selecting **Close Other Groups**.

![Deaching or closing a group via right-click.png](Deaching or closing a group via right-click.png)

*Figure: Detaching or closing group via right-click*

All widgets of a group except for the selected widget will be closed when **right-clicking** on the widget name within a group and selecting **Close Others**.

![Detaching or closing widgets in a group via right-click.png](Detaching or closing widgets in a group via right-click.png)

*Figure: Detaching or closing widgets in a group via right-click*

An overview of all widgets together with the possibility to de-/activate single widgets and to reset the layout to its initial state can be found under **View**.

- Widgets can be activated and deactivated (closed) using the checkboxes in the widget list. The widget list can be found under **View** in the software header.
- The default layout including the original arrangement of widgets may be restored by clicking **View - Reset Layout**.

![De-/Action of widgets.png](image_2.png)

*Figure: De-/Activation of widgets in the widget list (left) and reset of software layout (right) under "view"*

>**Note:** The layout is saved when quitting the application by closing the main window or via **File – Exit** and is independent of loaded workspaces or datasets.