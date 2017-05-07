# Time Series Analysis
----
### Autoregressive models
AR models use data from previous time points to predict the next time point
* This essentially creates a linear regression using the (t-1) period
  * Also can include the t-2 period as a second term
* The coefficient values are the unscaled correlation (the covariance) between the periods - that coefficient will add a percentage
  * Common version of this is CAGR - think of CAGR as the coefficient, and the constant as some "base" or starting value
* This model is known as AR(*p*) because it includes the previous *p* values of *Y*
  * Time units all need to be the same
  * Most common is AR(1) - which includes just one time period; explanatory value of throwing lots of prior times into the model has quickly diminishing returns

Core assumptions - that the data is highly dependent on previous values

### Moving average model
Moving average models predict values based on the overall average of how *incorrect* or prior models were - the error of previous predictions, vs the predictions themselves
* Incorporating more prior values will help improve the average error calculation
* The average of the dataset is our constant term
* Model checks an order term *q* and calls the moving average model MA(*q*)
* More complex fitting procedure than AR models
* Characterized by random jumps around the mean value
**Very important: MOVING AVERAGE MODEL DOES NOT USE THE MOVING AVERAGE, IT USES THE PREVIOUS ERRORS**
Moving average models take, as inputs, previous errors; moving averages just average recent Y values.

### ARMA Models
ARMA(*p,q*) models combine the autoregressive and moving average models
* Can add the &beta;0 and &mu; of dataset

### Stationarity
**Stationarity** means we decompose our time series, eliminating out the trend, so that we can see just the seasonal changes

### Implementation
* The difference between an AR model that is grouped by week and one grouped by day with a lag of 7 is twofold:
  1. The groupby week will result in the sum of the full week
  2. The groupby day will include a term *for each day* that is included in the model
* The autocorrelation function checks the current period vs the *n* lag day; but using the AR function will build in a term for each of the days going back to the *n* day
  * To get around this **reframe the database** as a series of differences between various points in time
----
## Intro to Forecasting
### ARIMA
**ARIMA** - AutoRegressive Integrated Moving Average models

The *"Integrated"* component models the difference between our lagged data

The differencing allows us to de-trend our data as we approach stationarity

ARIMA(*p,d,q*), where *d* is the amount of difference for any set of points
- *d* = 1 may cause stationarity
- *d* = 2 may capture exponential movement

### Seasonal ARIMA
Seasonal ARIMA builds two portions - the seasonal and non-seasonal components

### Partial ACF
Partial autocorrelative function - the way a variable correlates to the *y* independent of all the other variables; the average signal that any period's lag provides
- they tell you the added value of every additional lag

**AR signature** - slowly drifting AR terms, and PACF has a clear, sharp dropoff - it tells you to to add AR terms (as many as the notable PACF spikes) to better capture things

**MA signature** - slowly drifting AR terms, with a clear *spike* after it, followed by a dropoff - want to soak up that spike using a *q* term

### Evaluating models
1. Plot the residuals, look at them; if there's no pattern, you've succeeded
2. Ljung-Box Test - mathematical test of the residual plotting we did above
3. Akaike Information Criteria - relative measure of info gained from the model; lower is better

### Dickey-Fuller test for Stationarity
The test hypothesizes that there is a unit root that is influencing our data - **we want to reject that null hypothesis**
