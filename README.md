Problem Statement

Cryptocurrency prices move fast and often behave unpredictably, which makes forecasting a challenging task. Traditional statistical models usually fall short when markets become volatile. This project aims to forecast Ethereum prices using deep learning models such as RNN, LSTM and GRU. The goal is to build and compare these architectures to see which one provides the most reliable short-term predictions for ETH.

📘 Project Summary

This project looks at how well different Recurrent Neural Network models can forecast Ethereum’s price movements. It focuses on SimpleRNN, LSTM and GRU and examines how each model deals with the volatility and long-term patterns found in crypto markets. 

The notebook takes you through the complete process: downloading the data, exploring price trends, preparing the data for supervised learning, training the models and comparing their performance. Along the way, it shows how these networks learn from past price behavior and where each model performs best or struggles.

📊 Objectives

Download Ethereum price data using yfinance

Explore price trends, moving averages and volatility

Prepare data using scaling and sliding windows

Train RNN, LSTM and GRU models

Measure performance using RMSE and MAE

Plot actual vs predicted prices for comparison

Although the main models in this project focus on RNN, LSTM and GRU, time series forecasting can be improved further using an Encoder–Decoder structure with an Attention mechanism. This approach is common in sequence-to-sequence tasks and is now widely used in advanced forecasting models.


🧩 Workflow Summary
1. Data Collection

Source: Ethereum historical price data from yfinance

Ticker: ETH-USD

Includes: Open, High, Low, Close, Adj Close, Volume and Date

2. Data Preprocessing

Cleaned timestamps and handled missing values

Scaled features using MinMaxScaler

Created look-back windows to convert the time series into supervised sequences

3. Exploratory Data Analysis

Visualized ETH closing price over time

Added 7-day and 30-day moving averages

Studied volatility using rolling statistics

Checked correlations across price-related features

4. Model Building

Built and trained three RNN-based models:

SimpleRNN – A basic sequential model

LSTM – Designed to capture long-term dependencies

GRU – A faster, more efficient alternative to LSTM

All models were trained on the same dataset for a fair comparison.

5. Evaluation Metrics

Models were evaluated using:

RMSE

MAE

Training vs validation loss curves were also reviewed to understand learning stability.

6. Visualization

Plotted predicted vs actual Ethereum prices

Compared lag, variation and trend accuracy

Highlighted each model’s strengths and weak spots

🧠 Key Learnings

Built a complete forecasting pipeline from raw data to predictions

Gained practical experience with RNN, LSTM and GRU architectures

Learned how scaling and window sizes impact predictions

Improved understanding of hyperparameter tuning

Observed how crypto volatility challenges deep learning models

🧮 Results

All models captured the general movement of Ethereum’s price

LSTM and GRU delivered smoother and more accurate forecasts than SimpleRNN

GRU achieved strong accuracy with faster training times

Predicted curves aligned well with actual prices, especially for LSTM and GRU
