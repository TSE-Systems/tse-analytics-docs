# Binning widget


Time binning can be applied to a selected dataset by ticking the **Apply Binning** check box in the _Binning_ widget. For time binning, three different **Binning Modes** with customizable settings are available and can be selected from the dropdown menu: binning by repeating **Time Intervals**, binning according to **Light/Dark Cycles** and binning by custom **Time Phases**.

For binning by repeating **Time Intervals** of equal length, the duration of the time intervals can be set by choosing the respective unit (day, hour or minute) from the **Unit** drop-down menu and the number of days, hours or minutes, respectively, under **Delta**.

For binning by **Light/ Dark cycles**, the start of the light and dark cycle as the time of the day (24h format) can be customized under **Light cycle start** or **Dark cycle start**, respectively, after selecting the binning mode **Light/ Dark Cycles.**

When selecting binning by **Time Phases**, custom time phases can be added by clicking the ‘**+**’ (plus) symbol in the bottom left corner. A unique name for each time phase must be entered in the pop-up window and can be changed by double clicking on the phase name in the _Time Phases_ table. A time phase can be removed by selecting the respective row in the list (highlighted in blue) and clicking the ‘**\-**‘ (minus) symbol in the bottom left corner.

**Warning:**

- Changes in time binning settings (specification of time intervals, light/dark cycles or time phases) are not applied automatically to the data table in the _Table_ widget and plots in the _Plot_ widget. These widgets are only updated if previously deactivated time binning is activated again. It is recommended to change settings only while time binning is inactive (tick box not checked) and to apply changes by activating time binning again. Alternatively, time binning has to deactivated (uncheck tick box) and activated (check tick box) again to apply changes.
- For all other analysis widgets (Exploration, Bivariate, AN(C)OVA, Dimensionality and Timeseries), changes in time binning settings (applying of binning, binning mode and time binning settings) are only applied upon clinking **Update** in the control panel.

Different methods of calculation (**Aggregation** modes) can be used for the calculation of data values for individual time bins during binning: mean, median, sum, minimum and maximum. 

These modes can be specified individually for each variable via the dropdown menu in the **Aggregation** column of the _Variables_ widget. The most suitable aggregation mode differs between variables depending on the way data is collected and displayed during a PhenoMaster experiment. The default aggregation mode is the recommended method of calculation. Aggregation modes for all variables can be reset to the default state by clicking **Reset** in the header of the _Variables_ widget. Recommended (i.e. default) aggregation modes can also be found in the variables list in the appendix of this manual (INSERT LINK).
Start typing here...