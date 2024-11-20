# Adjust

Several tools for editing and preprocessing a selected dataset are available in the header of the _Dataset_ widget. Those include **adjusting** a dataset in the _Adjust Dataset_ window, **removing** a dataset from the _Dataset_ widget, creating a copy (**cloning**) of a dataset and **merging** of datasets.

**Adjust Dataset**

The _Adjust Dataset_ window offers multipe tools for editing a dataset and selecting time phases and animals of interest. To open the _Adjust Dataset_ window, select the respective dataset from the dataset list (selected dataset highlighted in blue) and and click **Adjust** in the _Dataset_ header.

To select and activate a tool for editing the dataset, tick the check box of the respective tool. Available operations are:

- **Rename**: The dataset can be renamed by entering a new dataset name in the text field underneath.
- **Apply resampling**: A new sample interval can be defined by typing in a new time interval using the format ‘hh:mm:ss’ or by using the arrows on the right.

**Note**: New sample intervals cannot be shorter than the original sample interval during the measurement. ( need check with Anton)

- **Apply time shift**: The time stamps of an experiment can be shifted forward (into the future) by selecting ‘+’ (plus) or backwards (into the past) by selecting ‘-‘ (minus). The time shift can be defined as a custom number of days and/or hours, minutes and seconds.

**Note:** Adjusting the time will directly change the time stamps in the raw data table used by TSE Analytics and thereby manipulate your data and results artificially. Please only use this option if you have a particular reason to do so, e.g. if the time stamp in the original data file does not match the actual date or time of the experiment.

- **Trim time**: The date and time of the start and the end of a dataset can be changed here to shorten the time span covered by the dataset. Thereby, data from the beginning and the end of an experiment can be excluded.

**Note**: The start time cannot be a time before the actual start of the experiment and the end time cannot be a time after the actual end of the experiment.

The example below shows time trimming via the exclusion of a time phase at the beginning of an experiment (changing the start time).

- **Exclude time**: A custom time phase (at the beginning, the end or in the middle of an experiment) can be excluded by defining the start and the end time of the time phase that should be excluded.

**Note:** It is not possible to enter a start time for the excluded time phase that lies before the beginning of the experiment or after the end of the excluded time phase. The end time for the excluded time phase cannot be a date or time after the end of the experiment or before the start time of the excluded time phase.

- **Exclude animals**: Animals which should be permanently excluded from the dataset together with all associated data can be selected from the animals list. Selected animals are highlighted in blue.

To apply changes specified in the _Adjust Dataset_ window to the selected dataset, click **OK**.

**Warning**: Changes regarding the trimming or exclusion of time phases as well as exclusion of animals cannot be undone once thay have been applied (by clicking **OK**). It is recommended to create a clone of a dataset before making adjustments as a backup.

**Note**: All changes made via the _Adjust Dataset_ window will only be applied to the dataset within TSE Analytics but do not affect the original dataset stored outside of TSE Analytics.Start typing here...