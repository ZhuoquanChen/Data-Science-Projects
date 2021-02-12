# Stock Forecasting

## Background
Technology has become an integral part of finance. Many financial firms are now growing into technology companies instead of staying in the traditional aspect. The frequency of financial transactions generates large data volumes, which make financial firms paid more and more attention to technology over the years. Today, technology is one of the main pushers in finance.

## Problem Statement
This is a project about stock price prediction. This project fully reflects how the difference between using technology and traditional methods for financial analysis. In this project, I am using apple stock data for the past 5 years, which contains market analysis and close price prediction. In the market analysis part, I am able to calculate the stock return in daily, weekly, monthly and even quarterly, and also using trading strategy. In the price prediction part, I used the time series model ARIMA and tried to find the best p, d, q to fit the model for predicting the price movements, and used mean squared error as evaluation function of this model.

## Data
- AAPL and GOOG, 2015 - 2020, download from yfinance.

## Methodology:
- Time series processing
- Check time whether miss or not

## Exploratory Data Analysis:
- Historical close price (daily, weekly, monthly)
- The return rate of AAPL in 2020
- Moving windows
- Volatility
- Trading Strategy

## Modeling
1. time series model: ARIMA
- Data stationarity
  - P-value
  - difference
- ACF & PACF (p, q) / AIC

2. SVM
3. Linear Regression

## Results
- Prediction
- rmse is 0.7067031040119878
- SVM Regression Model: 0.9848634030591281
- Linear Regression Model: 0.9825983604828592

## Conclusions
The purpose of this analysis only for study instead of any financial advice. Even ARIMA model performs pretty well in time series, such as stock, a variety of calculations, analysis, and trading strategy seem reasonable. However, many other factors can impact stocks' price, such as national policies, corporation internal issues, etc. and this eventually can not be predictable and computable. What we can do is improving the trading strategies, algorithms, or models.

## Next Steps
In the term of analysis, I will try to do more trading strategies for a further insight or analysis, such as inversion strategy, forecasting strategy and High-Frequency Trading (HFT) strategy. In the term of model and predition, I will try to use another technology, such as Long Short Term Memory, to see how they perform different, then find out a best solution.

