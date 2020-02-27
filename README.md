![](/art/Colorado-River-Storage-Project.png?raw=true)

## K-Nearest Neighbors Stochastic Streamflow Simulation

### 01. Streamflow Simulation

Rivers provide a range of valuable societal benefits, including hydropower, flood control, irrigation, navigation and recreation. Planning for risk and uncertainty requires an understanding of the variability of river streamflow and improves hydrological management.

Variable streamflows are usually modeled by stochastically generated sequences of streamflows, while preserving historic statistics. Such models usually assume stationary time series - that historical streamflow statistics are likely to be the same for future streamflow sequences.

### 02. Data Exploration and Modeling Methods

The 90 year sequence of historical Colorado River streamflow exhibit significant annual and monthly variability:

![Demo Animation](../plots/plotMNF.png?raw=true)

__Stochastic Streamflow Modeling__

Modeling future streamflows as a stationary ergodic stochastic process allows for the simulation of realistic future streamflows. The assumption of ergodicity allows time averages for corresponding ensembles of future flow sequences. A concern when modeling future streamflow sequence is to allow for the simulation of sequences not observed in the historical record but are possible based on statistical inference from historical flows.

Modeling streamflows as a stationary ergodic process allows the annual record of streamflows to be separated into monthly periods:

__Streamflow Distribution by Month__

![Demo Animation](../plots/plotMnthBplot.png?raw=true)

__Streamflow Histogram Distribution by Month__

![Demo Animation](../plots/plotMnthHist.png?raw=true)


### 03. Local Regression

Local regression is a non-parametric regression method that combines multiple regression models in a k-nearest-neighbor-based model. The streamflow local regression model estimates the conditional probability density function “locally” (e.g., the K-NN or the points within the kernel function) and simulate sequences from them. A local nonparametric regression is fitted to the successive monthly flows. Given the flow in the current month the fitted regression is used to obtain the mean flow of the next month.

![Demo Animation](../plots/plotLocfit.png?raw=true)

### 04. K-Nearest Neighbors Stochastic Simulation

K-NN time series resampling method approximates the conditional PDF using current value and one of the neighbors selected as the value for the next time step.

### 05. Streamflow Simulation Results

Simulated streamflows model historical statistics well: mean and standard deviation of streamflows are displayed below. Simulated data are plotted with box and whisker diagrams. Historical streamflow is plotted as a solid blue line.

![Demo Animation](../plots/plotSimMean.png?raw=true)

![Demo Animation](../plots/plotSimSD.png?raw=true)
