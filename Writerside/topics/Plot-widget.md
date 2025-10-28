# Plot

Line and scatter plots or bar plots can be generated using the **Plot** widget. 

![Plot widget.png](Plot widget.png)

Using the control panel, researchers can choose the animals, experimental groups, variables, and time phases for plotting and analysis.

> **Important**: Only animals selected in the Animal list are considered for the calculation of plots in the Plot widget
{style = 'warning'}
> 
![Figure: Selecting widgets.png](Selecting widgets.png)

Various selections for plotting can be made using the control panel located above the plot.

- **Variable Selection**: Users can select the variables of interest directly from the variables list. By default, descriptive statistics (aggregation) for the selected variables are calculated automatically. To view or modify these settings, use the **Variables → Aggregation** panel at the bottom-right of the interface.

- **Group Selection**: By default, data are grouped by individual animals or totals. If factor groups have been defined in the Factors panel, the group list will also display any additional groups created. To add or remove groups, use the **Factors → Edit Factors** panel at the bottom-right of the interface.

- **Binning Mode**: The binning mode for plot display can be further adjusted using the **Binning → Apply Binning** panel at the bottom-right of the interface.

>**Note**: All changes made through the control panel are reflected automatically in the plot. For large datasets, there may be a short delay of a few seconds.
{style = 'note'}



Errors for each mean value plotted are shown, if the **Display Errors** checkbox is ticked. Errors can be displayed as “Standard deviation” or “Standard error” (see selection underneath “Display Error”). No errors are displayed, if split mode ‘By animal’ is selected, if a factor group only contains one animal (for split mode ‘By factor’) or if only one animal is selected from the animal list independent of split mode.

For **line and scatter plots** (only if no time binning is applied or time binning using time intervals is applied):
- To change the plot style from line to scatter plot, the **Scatter plot** tick box must be checked.
- For line and scatter plots, two data plots are displayed. The large upper window is the main plot window and all settings specified in the control panel will be applied to this plot. The smaller plot at the bottom is always displayed as a line plot without error bars and serves as an overview over the whole plot. When the upper plot is used for zooming or enlarging an area of interest, a blue rectangle in the smaller plot at the bottom indicates the sector of the whole plot that is currently displayed in the upper window.
- The layout of both plots can be reset to their initial state by clicking **“A”** in the bottom left corner of each plot. The reset button (**“A”**) is only visible when hovering over the respective plot with the mouse cursor. 

![Figure: Line and scatter plots](line-scatter-plots.png)

Right-clicking on the plot opens a submenu for plot modifications.
Here, further adjustments regarding the plot appearance (e.g. axis, grid, transparency, etc.) can be made.****

![Figure: Plot options](plot-data-view-options.png)

The plot displayed can be exported by selecting **Export** and adjusting export options in the Export window.
Alternatively, the current plot can be added to the report by clicking **Add to Report** in the control panel and will be saved together with the currently active workspace.
