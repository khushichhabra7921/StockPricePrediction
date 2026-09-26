# 📈 Stock Market Prediction with Time Series ML

###
A comprehensive machine learning project for predicting stock prices using time series analysis and multiple ML algorithms. This project automatically fetches real-time stock data, engineers technical indicators, trains multiple models, and provides next-day price predictions.
---
# 🚀 Features
###
Real-time Data Collection: Fetches live stock data from Yahoo Finance

Advanced Feature Engineering: 30+ technical indicators including moving averages, RSI, MACD, Bollinger Bands

Multiple ML Models: Linear Regression, Random Forest, Gradient Boosting, SVR, and LSTM

Time Series Aware: Proper time series validation to prevent data leakage

Honest Evaluation: predicts next-day returns and compares RMSE against a "price won't change" baseline, plus directional (up/down) accuracy

Next-day Predictions: Automated price predictions with confidence intervals

Multi-stock Comparison: Compare prediction performance across multiple stocks

---

# 📊 Technical Indicators
### The project automatically calculates 30+ technical indicators:
---
# Price-based Indicators
###
Simple Moving Average (SMA): 5, 10, 20, 50, 200 days

Exponential Moving Average (EMA): 5, 10, 20, 50, 200 days

Price Returns and Log Returns

Price Position indicators

---
# Technical Oscillators
###
RSI (Relative Strength Index): Momentum oscillator

MACD: Moving Average Convergence Divergence

Bollinger Bands: Volatility bands with position indicators

---
# Volume Indicators
###
Volume Moving Average

Volume Ratios

Volume-Price Trend

---
# Volatility Measures
###
Rolling Standard Deviation

Average True Range (if TA-Lib available)

---
# Lagged Features
###
Historical price lags (1, 2, 3, 5, 10 days)
---
Volume lags

Returns lags

---

# 🤖 Machine Learning Models

# Traditional ML Models
###
Linear Regression: Baseline linear model

Ridge Regression: Regularized linear model

Random Forest: Ensemble of decision trees

Gradient Boosting: Sequential boosting algorithm

Support Vector Regression: Non-linear regression with RBF kernel

---
# Deep Learning Models
###
LSTM Neural Network: Long Short-Term Memory for sequential data

2-layer LSTM with dropout

Optimized for time series prediction

---

# 📈 Model Evaluation
# Metrics Used
###
Directional Accuracy: share of days where the predicted up/down move matches reality (primary metric for model selection; 50% = coin flip)

RMSE (Root Mean Square Error): Error on next-day return, reported next to a no-change baseline RMSE

MAE (Mean Absolute Error): Absolute prediction error

R² Score: Explained variance ratio (expected to be around zero or negative for daily returns)

---
# Validation Strategy
###
Time Series Split: Prevents data leakage by respecting temporal order

Walk-forward Validation: Tests on future unseen data

Performance Comparison: Automatic best model selection

---

