# Stock Price Prediction and Strategy
## Overview
Welcome to the StockPricePrediction_SARIMAX repository! This project is a comprehensive exploration of stock price prediction and the formulation of winning trading strategies. We leverage SARIMAX for close price prediction and employ a wide array of features for improved forecasting accuracy.

## Data
We work with a dataset provided in the train.csv file, which contains crucial financial information such as open, close, volume, and a strategy column.
Our objective is to predict the best strategy for the test data based on forecasted close prices and other feature columns.
## Feature Engineering
For close price prediction using SARIMAX, we have meticulously engineered a set of features to enhance our model's performance. These features include:

* ### Percentage change of open and close prices (Open_pct_change, Volume_pct_change)
* ### Lagged percentage changes (Open_pct_change_lag1, Volume_pct_change_lag1, ..., Open_pct_change_lag7, Volume_pct_change_lag7)
* ### Rolling means (Open_rolling_mean, Volume_rolling_mean)\
* ### Differences (Open_diff, Volume_diff)
* ### Moving averages (Open_moving_average, Volume_moving_average)
* ### Temporal features (year, month, day)
* ### Decomposition components of open and volume, including trend, seasonal, and residual components (Open_trend, Open_seasonal, Open_residual, Volume_trend, Volume_seasonal, Volume_residual)


## SARIMAX Forecasting
We employ the SARIMAX model to forecast close prices, using the feature-engineered variables as exogenous factors. The primary prediction variable is "close."

## Strategy Formulation
To determine the best trading strategies, we've explored various techniques, including:

Recursive Feature Elimination (RFE) integrated with Logistic Regression with L2 regularization.
Technical indicators such as RSI (Relative Strength Index), Bollinger Bands, and Stochastic Oscillator.
Machine learning models, including Support Vector Classifier (SVC), XGBoost Voting Classifier, and Random Forest.

## Additional Insights
This repository showcases an in-depth analysis of the stock market, combining traditional time series forecasting techniques with machine learning approaches for strategy optimization.
Our experiments with a diverse set of prediction and trading strategies provide valuable insights for both beginners and experienced traders.

## Usage
To explore the code and replicate the experiments, follow the instructions provided in the repository.

## Contribution
Feel free to contribute by opening issues, suggesting improvements, or submitting pull requests.
Also ⭐

## Credits
This project was developed by [Rahul Rao](https://github.com/rahulrao9) and [Hemabhushan R](https://github.com/Hemabhushan-r).
