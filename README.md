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
# Data Splitting and Feature Engineering:
The dataset is split into training and testing sets. The time-series data is then converted into sequences of input features (X) and corresponding output labels (y). This process involves creating a sliding window over the time-series data, where each window represents a set of input features and their corresponding output label.
# LSTM Model Architecture:
The LSTM model is constructed using the Keras API, which is integrated into TensorFlow. The architecture consists of multiple LSTM layers followed by a Dense output layer. The model is compiled using the Mean Squared Error (MSE) loss function and the Adam optimizer.
# Training the Model:
The model is trained on the training dataset for 100 epochs with a batch size of 64. Training and validation performance metrics are monitored to ensure convergence.
# Model Evaluation:
The performance of the trained model is evaluated using the Root Mean Squared Error (RMSE) on both the training and testing datasets.
# Prediction and Visualization:
The trained model is used to predict stock prices for the next 30 days. The predicted values are then inverse-transformed to the original scale for meaningful interpretation. The results are visualized alongside the actual stock prices to assess the model's predictive accuracy.
# Conclusion:
The LSTM model demonstrates its effectiveness in capturing sequential dependencies in time-series data, making it a powerful tool for predicting stock prices. The choice of this model, along with proper data preprocessing and feature engineering, contributes to accurate and meaningful predictions. The visualizations provide insights into the model's ability to forecast stock prices, aiding decision-making processes for investors and analysts.
