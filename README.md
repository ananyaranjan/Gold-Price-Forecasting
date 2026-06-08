# Gold-Price-Forecasting
Time series forecasting of gold prices (XAU/USD) using RNN, LSTM, and GRU neural networks.

## Overview

This project compares the performance of Recurrent Neural Network (RNN), Long Short-Term Memory (LSTM), and Gated Recurrent Unit (GRU) models for forecasting gold prices using historical XAU/USD daily closing price data. The objective is to analyze how different recurrent neural network architectures perform on time-series forecasting tasks and identify the most effective model for gold price prediction.

## Dataset
#### Dataset: Historical Gold (XAU/USD) Daily Closing Prices
#### Time Period: June 2011 – May 2026
#### Feature Used: Daily Closing Price
#### Source: Historical gold price dataset

## Methodology
#### Data preprocessing and normalization
#### Exploratory Data Analysis (EDA)
#### Sequence generation using sliding windows
#### Training RNN, LSTM, and GRU models
#### Model evaluation using MAE and RMSE
#### Comparison of model performance
#### Forecasting gold prices for 2026

## Models Used
#### Recurrent Neural Network (RNN)
#### Long Short-Term Memory (LSTM)
#### Gated Recurrent Unit (GRU)

## Evaluation Metrics
#### Mean Absolute Error (MAE)
#### Root Mean Squared Error (RMSE)

## Experiments
### Experiment 1: 80–20 Train-Test Split

#### The dataset was divided into 80% training data and 20% testing data to evaluate each model's predictive performance on unseen data.

### Experiment 2: 2026 Forecasting

#### Models were trained on historical data and used to forecast gold prices for the year 2026. Forecasts were compared using MAE and RMSE where actual values were available.

## Results

#### Two forecasting experiments were conducted using RNN, LSTM, and GRU models on historical gold price data.

#### Experiment 1 (80–20 Train-Test Split): LSTM achieved the lowest error (MAE: 1915.70, RMSE: 1927.39), followed by GRU (MAE: 2030.11, RMSE: 2039.21), while RNN performed the worst (MAE: 2818.30, RMSE: 2832.86).
#### Experiment 2 (2026 Forecasting): GRU achieved the best performance (MAE: 105.94, RMSE: 141.85), followed by LSTM (MAE: 162.69, RMSE: 211.79), while RNN again recorded the highest errors (MAE: 331.86, RMSE: 407.66).

#### The results indicate that gated recurrent architectures (LSTM and GRU) significantly outperform the vanilla RNN for gold price forecasting. While LSTM performed best on the standard train-test evaluation, GRU demonstrated stronger generalization in the out-of-sample 2026 forecasting experiment, making it the most robust model overall for this dataset.
