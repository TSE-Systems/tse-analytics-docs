# Factors

![factors.png](factors.png)

## Data analysis pipeline

Almost all widgets (with some exceptions mentioned later) work with the preprocessed data that passed through the
internal data analysis pipeline.

1. Raw data first goes into *Animal Filter* pipe operator. This unit obtains data only for the selected set
   of animals. Animals can be selected in **Animals** widget.
2. Second step is the outliers removal in the *Outliers* pipe operator. This unit can be activated/deactivated in the
   **Outliers** widget (see details below).
3. Last step in the preprocessing data pipeline is *time binning* operation.

> **Note**: If you observe some strange results during your analysis, please check that proper animals are selected in
> **Animals** widget!
Start typing here...