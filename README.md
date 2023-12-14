# Stock Price Prediction using LSTM Neural Networks
Project 4 - Machine Learning

# Project Proposal
The aim of our project is to uncover the patterns in the stock market with the purpose of predicting future performance. Specifically in the healthcare sector. We will examine previous stock market performance to indicate future performance.

# Project Contributors
* Octavio Pinedo
* Alex Fok
* Andrea Aguilar
* Subha Barakoti
* West Burington
* Christian Deanda
* Sang Kim

# Introduction
The objective of this project is to predict the stock prices for the next 30 days of the top healthcare companies using machine learning. The chosen model for this prediction is based on Long Short-Term Memory (LSTM) neural networks, a type of recurrent neural network (RNN). The LSTM model is particularly suitable for sequential data like time-series, making it a valuable choice for predicting stock prices over time.
# Model Selection:
The LSTM model is selected for its ability to capture and learn patterns in sequential data, making it well-suited for time-series forecasting. Unlike traditional feedforward neural networks, LSTMs can remember information over long periods, which is crucial for predicting stock prices where past data points hold significant influence.
# Data Preparation:
The data used for training and testing the model is sourced from a 5-year stock dataset for healthcare companies. The dataset is loaded into a Pandas DataFrame, and a specific stock (company) is selected based on user input. The closing prices of the selected stock are then extracted for further analysis.
# Data Scaling:
Before feeding the data into the LSTM model, it is essential to normalize the data. The Min-Max scaling technique is applied to rescale the closing prices to a range between 0 and 1. This normalization ensures that the model can effectively learn from the data without being affected by the varying scales of the input features.


