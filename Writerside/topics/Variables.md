# Variables

The **Variables** Widgets in TSE Analytics allows users to select and manage experimental variables. Users can configure aggregation methods for each variable, such as mean, sum, or other statistics. Selected variables are automatically applied to downstream components, including **Matrix** and **PCA** statistical tools, ensuring analyses use a consistent and properly processed dataset.

The Variables interface also allows users to **delete a selected variables** by clicking the delete button or **add custom variables** by clicking the *Add* button.

![Variables Widgets.png](Variables Widgets.png)

Similarly to **Animals** widget, in order to select all variables at once, please press <shortcut>Ctrl+A</shortcut> or drag mouse over
entries you want to choose. To select/deselect individual entries, click on the entry holding <shortcut>Ctrl</shortcut> key.


## Aggregation

Different methods of calculation (**Aggregation** modes) can be used for the calculation of data values for individual time bins during binning(i.e., when raw data are grouped into defined time intervals): mean, median, sum, minimum and maximum.

The *Binning* widget and its settings will be described in detail in the following section.

![Figure: Aggregation mode](aggregation-mode.png)

> **Note**:For cumulative variables, such as DistK,the default aggregation mode is max. Within each time bin, this mode reports the maximum cumulative value, corresponding to the total distance reached by the end of that interval. 
> 
> If you are interested in the distance covered within each interval (i.e., interval-based activity), you can use the differential variable DistD and apply aggregation modes such as sum or mean.
> 
> The default aggregation mode is only a suggestion; users can adjust it according to specific analysis needs.
{style='note'}

These modes can be specified individually for each variable via the dropdown menu in the **Aggregation** column of the _Variables_ widget.
The most suitable aggregation mode differs between variables depending on the way data is collected and displayed during a PhenoMaster experiment.

![Figure: Resetting variables](resetting-variables.png)

The default aggregation mode is the recommended method of calculation. Aggregation modes for all variables can be reset to the default state by clicking **Reset** in the header of the _Variables_ widget.


## Outlier Detection

Outlier detection settings can be adjusted in the _Variables_ widget.
Here, one can choose between different modes via the dropdown menu: no outlier detection (**Outliers detection off**), highlighting outliers in the data table (**Highlight outliers**), and removing outliers from the dataset (**Remove outliers**).

![Figure: Outlier detection mode](outlier-detection-mode.png)

The sensitivity of outlier detection can be adjusted via the coefficient (for further information about the outlier detection method used (please see below: IQR method for outlier detection).
Decreasing the coefficient will result in more values being identified as outliers, while increasing the coefficient will result in less outliers.

![Figure: Outlier detection coefficient](outlier-detection-coefficient.png)

The variables to which outlier detection should be applied, need to be selected using the tick boxes in the ‘**Outliers**’ column in the _Variables_ widget.
Only variables selected here will be considered for the identification of outliers.
The variable selection for outlier detection can be reset to the default (no variables selected) together with the aggregation mode selector by clicking **Reset** in the Variables widget.

> **Important**: Selecting **Remove outliers** will not only delete outlier values but the whole row (i.e. time bin) in the data set which contains one or more values detected as outliers.
> This means that values of all variables recorded at the same time point as the outlier are removed from the dataset as well. 
>
> Therefore, it is recommended to only select the variable(s) for outlier detection which are used for subsequent analysis.
{style='warning'}

![Figure: Selecting outliers variables](selecting-outliers-variables.png)


> **IQR method for outlier detection**
> - **The IQR (Interquartile Range) method** detects outliers by analyzing the middle 50% of the data.
> First, the 1st quartile (Q1) and 3rd quartile (Q3) are calculated, giving IQR = Q3 – Q1. A coefficient k (default is 1.5 in TSE Analytics) is then applied to define the bounds: Lower Bound = Q1 – k × IQR, Upper Bound = Q3 + k × IQR.
> - All data points outside of the range [Q1 – IQR * coefficient; Q3 + IQR * coefficient] are considered **outliers**.
{style='note'}
