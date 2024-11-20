# Merge


Two or more datasets can be merged by selecting the respective datasets in the _Dataset_ widget using the **tick boxes** on the left-hand side of the dataset list. To open the _Merge_ _Datasets_ dialogue window, click **Merge** in the header of the _Dataset_ widget.

**Note**: The **Merge** button will only be active if two or more datasets are selected via tick boxes in the _Dataset_ widget.

_In this_ dialogue window, datasets can be adjusted individually via the **Adjust** button next to a dataset’s name to prepare and match all selected datasets for merging. Clicking **Adjust** opens the _Adjust Dataset_ window with the options to rename a dataset, apply resampling, apply time shift, trim time, exclude time and exclude animals (see INSTERT LINK) for each dataset individually. Tools to adjust a dataset can be activated by checking the respective tick box.

- **Apply resampling** allows to manually change (increase) the duration of sampling intervals to match sampling intervals of multiple datasets for merging.

**Note:** It is not possible to decrease the original sampling interval. Therefore, sampling interval needs to be adjusted to match with the dataset with the longest sampling interval.

- **Apply time shift** can be used to shift the time stamps of an experiment forward (into the future) by selecting ‘+’ (plus) or backwards (into the past) by selecting ‘-‘ (minus). The time shift can be defined as a custom number of days and/or hours, minutes and seconds.
- **Trim time** allows to shorten a dataset by adjusting the start and end time, and thereby matching the time frames and duration of individual experiments for merging.

**Note:** The start time cannot be a time point before the original start time or after the entered end time. In the same way, the end time cannot be a time point before the entered start time or after the original end of the experiment.

- **Exclude time** offers the possibility to exclude a customized time phase with a defined start and end time from the start, end or middle of a dataset to match the time frames of single datasets for merging.

**Note:** It is not possible to enter a start time for the excluded time phase that lies before the beginning of the experiment or after the end of the excluded time phase. The end time for the excluded time phase cannot be a date or time after the end of the experiment or before the start time of the excluded time phase.

- **Exclude animals** can be used to permanently remove selected animals from a dataset (animals selected to be removed are highlighted in blue).
- To apply changes defined in the _Adjust Dataset_ window to a dataset for merging, click **OK**.
- **Warning**: Changes regarding the trimming or exclusion of time phases as well as exclusion of animals cannot be undone once thay have been applied (by clicking **OK**).
- **Note:** Any changes applied to a dataset during the merging process will not affect the original dataset.

In addition to adjusting datasets individually, setting for merging can be selected on the right-hand side of the _Merge Datasets_ dialogue window.

The name of the merged dataset can be entered in the upper right corner under **Merged dataset name** (the default name for merged datasets is the name of the first selected dataset plus the suffix “(merged)”.

Merging can be performed using either the “Continuous” or “Overlap” mode, which can be selected under **Merging Mode**.

- “**Continuous**” mode:

Datasets are merged under consideration of the absolute time data stamps (date and time of the experiment) and are displayed one after each other if experiments have been performed after each other.

- “**Overlap**” mode:

Datasets are merged under consideration of relative stamps, i.e. time delta since the start of the experiment, and aligned according to their time bins. Datasets are displayed within the same time frame.

**Note**: If ‘Overlap’ mode is selected, the option ‘Add run number as suffix in animal names’ is available and can be activated by ticking the check box. Activating this option during merging is necessary, if animal names of the individual datasets are identical.

In addition, datasets can be merged as a single run (no differentiation between individual datasets after merging) or as individual runs (possibility to split merged dataset by run to distinguish between individual datasets during analysis). To merge datasets as a single run, the check box **Merge as a single run** needs to be ticked.

After adjusting settings in the _Merge Dataset_ dialogue window, click **OK** to create a merged dataset.

**Warning:** Settings for merging and adjusting individual datasets cannot be changed anymore, once the merged dataset has been created. Please ensure all adjustments and settings have been chosen correctly before clicking OK.

**Note**: Datasets can only be merged if the variables lists are identical. This applies to the individual variables contained in a dataset as well as variable settings specified in the _Variables_ widget (aggregation mode and selection of variables for outlier detection). In case of discrepancies between variable settings, aggregation modes and selection of variables for outlier detection can be reset to default by clicking **Reset** in the header of the _Variables_ widget.Start typing here...