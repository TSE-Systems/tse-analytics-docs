# Decomposition

For **Decomposition**, further settings can be specified:
- One of three different Methods can be selected: **Naïve**, **STL** (Seasonal and Trend decomposition using Loess) and **MSTL** (Multiple Seasonal and Trend decomposition using Loess).
- If decomposition is performed using the ‘Naïve’ method, two different **Models** can be used: an additive model or a multiplicative model.
- The number of time bins defining the (expected) period of the seasonality, i.e. length of one time cycle, can be set under **Period**. Setting an appropriate period helps the software accurately detect repeating patterns and seasonal trends in the data.
- [//]: # (TODO: Above phragragh about time bins is right? need Anton help to modify...)

![Figure: Time Series Decomposition window](image_65.png)

*Time series analysis* using decomposition allows users to break down data into **observed**, **trend**, **seasonality** and **residual components**. It helps to visualize the different components of a time series and understand how each component affects the overall data.

- **Observed**:
  This represents the original time series data, showing the unprocessed and complete dataset.

- **Trend Component**:
  The trend component displays the long-term movement of the data. It reveals whether the data is gradually increasing, decreasing, or remaining stable over time.

- **Seasonal Component**:
  The seasonal component reflects periodic fluctuations in the data, typically occurring at fixed intervals.

![Figure: Example of timeseries decomposition window display](image_67.png)

[//]: # (TODO: The above figure is not good example, yes? which variable choose will be better...)
[//]: # (TODO: Need to add more expalnantion for software using of Naive, STL, MSTL...)
