# Correlation

**Correlation analysis** is used to determine the strength and direction of the linear relationship between two variables, X and Y.
 
In TSE Analytics, the results are displayed as a scatter plot of all data pairs, along with individual density plots or histograms for each variable. Pearson's correlation coefficient is then calculated to quantify the strength and direction of this relationship. T-test statistics are used to assess the statistical significance of the correlation coefficient. Correlation analysis helps researchers identify significant associations between variables, guiding the further interpretation of experimental data.

![Figure: Correlation widget](Correlation widget.png)

## Correlation plots

Data pairs for each time bin are depicted as dots in the **scatter plot** and are dependent on the selected variables, groups and time binning settings.

![Figure: Correlation plot](Correlation plot.png)

**Histograms/ Density plots** represent how frequently different values occur for each variable. The plots are drawn along the axis corresponding to the variable, and the way the data is grouped and time-binned is taken into account.
> **Note**: Histograms are only shown when the data is grouped by “Total.” If the data is split into subsets (for example, by Animal or Factor), histograms are not used. Instead, a separate density curve is drawn for each subset.
{style = 'note'}

To adjust the appearance of a plot, use the **‘Customize’** tool (‘Graph’ symbol) in the plot menu and select the respective plot from the drop-down menu (**“[Variable X] – [Variable Y]”** for scatter plot and **“[Variable X] – Count/Density”** or **“Count/Density – [Variable Y]”** for density plots/ histograms).

- The title, as well as range, label and scale of axis and plot legend generation of individual plots can be defined in the **Axes tab** of the Customize tool.
- In the case of multiple animals, runs or groups (for split modes By Animal, By Run or By Factor, respectively), the appearance of each data subset can be adjusted individually in the **Curves tab** of the ‘Customize’ tool by selecting the respective subset form the upper
  dropdown menu.

![Figure: Axes tab of the customize tool](Customized the Histogram plots.png)

![Curve tab of the customized tool](image_2.png)


## Correlation results table

Correlation analysis results are calculated based on the (mean) data values per time bin depending on the respective split mode.

![Figure: Correlation analysis results table](correlation-analysis-results-table.png)

The **T-test statistics** comparing the X and Y variable include (from left to right):

- T: T-value
- dof: Degrees of freedom
- alternative: Tail of the test (two-sided)
- p-val: p-value
- CI95%: Confidence intervals of the difference in means
- cohen-d: Cohen d effect size
- BF10: Bayes factor of the alternative hypothesis
- power: Achieved power of the test (= 1 - type II error)


The **Pearson correlation** coefficient table indicates (from left to right):

-	X: Selected X variable
-	Y: Selected Y variable
-	method: Method of correlation analysis (pearson)
-	alternative: Tail of the test (two-sided)
-	n: Sample size (number of data pairs)
-	r: Correlation coefficient
-	CI95%: 95% parametric confidence intervals
-	p-unc: Uncorrected p-value
-	BF10: Bayes factor of the alternative hypothesis
-	power: Achieved power of the test (= 1 - type II error)

