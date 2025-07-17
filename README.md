
# Price Movement Prediction with LSTM
This project explores the use of deep learning techniques, particularly Long Short-Term Memory (LSTM) networks, for predicting stock price movements. It also applies classification techniques to categorize future price trends. Two Jupyter notebooks are included: one focused on data analysis and visualization, the other on LSTM-based forecasting and classification.

## Project Summary
Data Source: Yahoo Finance stock data for Apple (AAPL), Microsoft (MSFT), Netflix (NFLX), and Google (GOOG), covering the period from April 2023 to April 2024.

Tech Stack: Python, Jupyter Notebook, TensorFlow/Keras, Pandas, NumPy, Matplotlib

Prediction Targets:

Regression: Predicting stock closing prices.

Classification: Identifying movement direction (increase, decrease, unchanged).

## Methodology
### Data Collection:

Data is downloaded using the yfinance library.

Ticker symbols: ['GOOG', 'NFLX', 'MSFT', 'AAPL']

Time range: 2023-04-01 to 2024-04-01

### Data Preprocessing:

Missing value handling

Feature scaling

Feature selection: Open, High, Low, Close, Adj Close, Volume

### Model Architecture:

1D Convolutional Layer

Two LSTM Layers

Dense output layer

Lambda layer for custom output adjustment

### Evaluation:

Regression Metrics: MAE = 2.96, MSE = 3.558

Classification Accuracy: ~52.6%

Confusion matrix and visualizations for predicted vs. actual

### Trend Classification:

Increase: price rise > 0.005

Decrease: price drop > 0.005

Unchanged: price change within ±0.005

### Visualizations
Closing price over time

Volume distribution

Correlation heatmaps

LSTM prediction vs. real values

Confusion matrix for classification

## Developers
Sena Ezgi Anadollu

## About the Project
This project was developed as part of a Computational Finance course. The development was completed in April 2024.
