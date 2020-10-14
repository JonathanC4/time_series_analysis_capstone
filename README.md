# Capstone-Time-Series-Analysis

## Problem Statement
How effective is time series modeling? In this project, I explore basic ARIMA techniques and apply them to Tesla's stock prices with both exogenous and endogenous variables. In addition, I've constructed a rudimentary Long Short-Term Memory Recurrent Neural Network to contrast performance (forecasting error) between the two models.

## Overview
The primary focus of this project is the time series analysis methodology. I did not bring into consideration other factors that may have affected Tesla's stock price movement. Topics covered include:
  - Autocorrelation and Partial AC
  - Non-seasonal ARIMA models (p, d, q)
  - Time series deconstruction: trend, seasonality and white noise
  - Stationarity
  - LSTM RNN

## Findings
After analyzing the ACF and PACF charts, I concluded that the Tesla stock price could be represented with a geometric random walk model. The stock price movement showed an overall exponential growth rate and taking the natural log of the first difference of the data revealed a consistent day-to-day fluctuation in price expressed as a percentage change. From there, I was able to construct a 95% confidence interval for each successive day. A basic method to swing trading involves using the boundaries as indicators for shorting or buying a particular stock. For example, if the stock movement for that day trends towards the upward boundary, you know that the price is not likely to exceed a certain amount so that becomes an opportunity to short. Nonetheless, the nature of stock prices is wild and random when considering all exogenous factors. 
