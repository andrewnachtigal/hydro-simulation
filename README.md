## K-Nearest Neighbors Stochastic Streamflow Simulation

### 01. River Streamflow Simulation 

Rivers provide a range of valuable societal benefits, including hydropower, flood control, irrigation, navigation and recreation. Planning and management of river systems requires an understanding of the variability of river streamflow, which are climate-dependent and vary from month to month. Modeling streamflow variability allows for the analysis of risk and uncertainty and improved hydrological management. 

Variable streamflows are usually modeled by stochastically generated sequences of synthetic streamflows, while preserving historic statistics and possibly higher order statistics. Such models assume stationary time series, that historical streamflow statistics are likely to be the same for future streamflow sequences.

### 02. Data Set Exploration and Modeling Methods

* Stochastic Streamflow Modeling

Modeling future streamflow sequences depends on the assumption that future flows will exhibit characteristics observed in the past. Future streamflows are modeled as a stationary ergodic stochastic process, which allows for the simulation of realistic future streamflows. The assumption of ergodicity allows time averages for corresponding ensembles of future flow sequences.

A stationary process is a stochastic process whose unconditional joint probability distribution does not change over time (so monthly mean is constant). An ergodic process is one for which statistical properties can be inferred from a single long random sample of the process. Stochastic methods refers to the random element incorporated in these methods, and try to predict the value of some variable at non-observed times or at non-observed locations, while also stating how uncertain we are when making these predictions.

Stochastic stremflow models are meant to capture the evolution over time of real phenomena for which randomness is inherent. A concern when modeling future streamflow sequence is to allow for the simulation of sequences that are not observed in the historical record but are possible based on statistical inference from historical flows.

Annual Streamflow Time Series
![Demo Animation](../plots/plotWY.png?raw=true) . 

Monthly Streamflow Time Series
![Demo Animation](../plots/plotMNF.png?raw=true) . 

The time series plot of monthly streamflows exhibit significant annual and monthly variability.

* Streamflow Boxplot Distribution by Month

![Demo Animation](../plots/plotMnthBplot.png?raw=true)

* Streamflow Histogram Distribution by Month

![Demo Animation](../plots/plotMnthHist.png?raw=true)

### 03. Local Regression



### 04. K-Nearest Neighbors Stochastic Simulation

### 05. Results
