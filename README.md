# Stock Price Prediction using LSTM Neural Networks
Project 4 - Machine Learning

Languages used: Python
Databases used: PySpark, Pandas, Matplotlib, Tensorflow, Numpy, Scikit Learn
Visualization Program used: Tableau

# Project Contributors
* Octavio Pinedo
* Alex Fok
* Andrea Aguilar
* Subha Barakoti
* West Burington
* Christian Deanda
* Sang Kim

# Introduction:
The history of stocks has become significantly popular after the dot-com boom. With the advancement of technology, anyone is able to access and trade.  The goal for this project is to uncover different patterns of past data to predict future stocks, specifically in the healthcare sector. 

# Model Selection:


# Model Optimization:
The model underwent iterative optimization by adjusting layers and LSTM units, initially achieving R-squared values of .95 (training) and .77 (testing) within 30 seconds. Ultimately, after balancing complexity and runtime, the optimized model achieved an R-squared of .98 (training) and .90 (testing) within approximately 3 minutes, meeting project objectives despite the tradeoff between increased performance and computational resources.
* The program takes the last 100 data points from the test data, and reshape it into a NumPy array in preparation for making predictions
* We then convert it into a list. Using this list we create a while loop set for I<30. (Trying to predict 30 days into the future)
* we are using what is know as the sliding window technique for time series forecasting
* Using Matplot lib, we create a basic graph showing historical prices for the previous 100 days in blue, then plot another line for the following 30 days in yellow. (INSERT PREDICTION PIC)
* For comparison, we graphed available December data in tableau, placing prediction vs reality side by side.

# Prediction and visualization
The trained model is used to predict stock prices for the next 30 days. The results are visualized alongside the actual stock prices to assess the model's predictive accuracy. Following an analysis of our LSTM model for stock price prediction, we examined its performance on Johnson & Johnson and Pfizer stocks. While accurately forecasting a decline for JNJ, challenges arose with Pfizer, highlighting a 30% overall model accuracy. Recognizing the need for improvement, we acknowledge the impact of sudden market shifts and emphasize a strategic, risk-managed approach for real-life applications, emphasizing continuous model refinement and diversified investment decisions.


# Training the Model:
The model is trained on the training dataset for 100 epochs with a batch size of 64. Training and validation performance metrics are monitored to ensure convergence.
# Model Evaluation:
The performance of the trained model is evaluated using the Root Mean Squared Error (RMSE) on both the training and testing datasets.
# Prediction and Visualization:
The trained model is used to predict stock prices for the next 30 days. The results are visualized alongside the actual stock prices to assess the model's predictive accuracy. Following an analysis of our LSTM model for stock price prediction, we examined its performance on Johnson & Johnson and Pfizer stocks. While accurately forecasting a decline for JNJ, challenges arose with Pfizer, highlighting a 30% overall model accuracy. Recognizing the need for improvement, we acknowledge the impact of sudden market shifts and emphasize a strategic, risk-managed approach for real-life applications, emphasizing continuous model refinement and diversified investment decisions.
# Conclusion:
The LSTM model demonstrates its effectiveness in capturing sequential dependencies in time-series data, making it a powerful tool for predicting stock prices. The choice of this model, along with proper data preprocessing and feature engineering, contributes to accurate and meaningful predictions. The visualizations provide insights into the model's ability to forecast stock prices, aiding decision-making processes for investors and analysts.
