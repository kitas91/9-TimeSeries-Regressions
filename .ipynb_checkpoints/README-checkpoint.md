# TimeSeries-Regressions
Time Series Forecasting &amp; Linear Regression Forecasting 


Background
-----

Using a Hodrick-Prescott Filter, decompose the Settle price into a trend and noise. The Hodrick–Prescott filter (also known as Hodrick–Prescott decomposition) is a mathematical tool used in macroeconomics, especially in real business cycle theory, to remove the cyclical component of a time series from raw data. It is used to obtain a smoothed-curve representation of a time series, one that is more sensitive to long-term than to short-term fluctuations. The adjustment of the sensitivity of the trend to short-term fluctuations is achieved by modifying a multiplier.

Throughout this assignment, we used time series analysis and linear regressions to make predictions of the Japanese Yen movements against the USD.

In our analysis we used ARMA, ARIMA, & GARCH models to estimate the relationships between the Yen's performance against the USD.

Autoregressive integrated moving average (ARIMA) model is a generalization of an autoregressive moving average (ARMA) model. Both of these models are fitted to time series data either to better understand the data or to predict future points in the series (forecasting). ARIMA models are applied in some cases where data show evidence of non-stationarity, where an initial differencing step (corresponding to the "integrated" part of the model) can be applied one or more times to eliminate the non-stationarity. ARMA model was used to forecast returns. 

The AR part of ARIMA indicates that the evolving variable of interest is regressed on its own lagged (i.e., prior) values. The MA part indicates that the regression error is actually a linear combination of error terms whose values occurred contemporaneously and at various times in the past. The I (for "integrated") indicates that the data values have been replaced with the difference between their values and the previous values (and this differencing process may have been performed more than once). The purpose of each of these features is to make the model fit the data as well as possible. ARIMA model was used to forecast price. 

Non-seasonal ARIMA models are generally denoted ARIMA(p,d,q) where parameters p, d, and q are non-negative integers, p is the order (number of time lags) of the autoregressive model, d is the degree of differencing (the number of times the data have had past values subtracted), and q is the order of the moving-average model. Seasonal ARIMA models are usually denoted ARIMA(p,d,q)(P,D,Q)m, where m refers to the number of periods in each season, and the uppercase P,D,Q refer to the autoregressive, differencing, and moving average terms for the seasonal part of the ARIMA model.

In econometrics, the autoregressive conditional heteroscedasticity (ARCH) model is a statistical model for time series data that describes the variance of the current error term or innovation as a function of the actual sizes of the previous time periods' error terms; often the variance is related to the squares of the previous innovations. The ARCH model is appropriate when the error variance in a time series follows an autoregressive (AR) model; if an autoregressive moving average (ARMA) model is assumed for the error variance, the model is a generalized autoregressive conditional heteroskedasticity (GARCH) model. GARCH model was used to forecast volatility. 

------

Based on the results of above models, it would seem that the Yen should depreciate over time and its volatility will continue high. With the volatility present within the underlying asset, I would not take a long strategy. It would have to be monitored on a daily basis however, the model is not accurate enough for me to trust the results. 

After training the model with the data from 1990 – 2018, we found that the root mean squared error for the out-of-sample application was lower than that of the in-sample application; indicating that this was a fairly effective model in predicting future values.
