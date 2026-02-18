# Streaming-Data-Management-and-Time-Series

This project explores the application of both classical statistical methods and modern machine learning algorithms for Time Series Analysis and Forecasting. The primary goal is to predict daily values for a specific timeframe (2015-04-01 to 2015-11-07) by comparing the predictive accuracy of linear models against ensemble learning techniques.

## 1. Models & Methodologies

The project incorporates three distinct families of forecasting models:
- Statistical & State-Space ModelsARIMA (Auto-Regressive Integrated Moving Average): Specifically an $ARIMA(1,0,4)(0,1,3)_7$ model to capture both short-term dependencies and weekly seasonality.
- UCM (Unobserved Components Model): A state-space approach utilizing a local linear trend and a weekly seasonality component to decompose the signal.

Machine Learning ModelsThese models utilize lag values (autoregressive features) to transform the time series into a supervised learning problem:

- Random Forest: Evaluated both as a standard regressor and with cross-validation to ensure stability.k-Nearest Neighbours 
- (k-NN): Implemented using recursive forecasting and transformed training samples.
- eXtreme Gradient Boost (XGBoost): Leveraged for its high performance in handling non-linear patterns, tested with and without cross-validation.
