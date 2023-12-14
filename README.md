# Stock Price Prediction using LSTM Neural Networks
Project 4 - Machine Learning

Languages used: Python <br />
Databases used: PySpark, Pandas, Matplotlib, Tensorflow, Numpy, Scikit Learn <br />
Visualization Program used: Tableau <br />

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
* Obtained 5 years' worth of stock data for S&P 500 stocks on Kaggle, including daily metrics like opening and closing prices, high and low, volume, dividends, and stock splits.
* Loaded the data into a data frame and narrowed it down to 10 healthcare stocks.
* Preprocessed the data using the Train and Test method, focusing on the closing price over the previous 5 years.
* Considered various machine learning models and narrowed down the selection to Linear Regression and Long Short-Term Memory (LSTM).
* Chose LSTM over Linear Regression for better accuracy, despite being slower.
* Developed an initial LSTM model with three layers of 50 units each and a dense layer with a single unit.
* Fit the data using 100 epochs and 64 batches, taking approximately 6 minutes per stock, achieving 97-98% accuracy.
* Recognized the need for optimization to improve both speed and accuracy of the model.

# Model Optimization:
The model underwent iterative optimization by adjusting layers and LSTM units, initially achieving R-squared values of .95 (training) and .77 (testing) within 30 seconds. Ultimately, after balancing complexity and runtime, the optimized model achieved an R-squared of .98 (training) and .90 (testing) within approximately 3 minutes, meeting project objectives despite the tradeoff between increased performance and computational resources.
* The program takes the last 100 data points from the test data, and reshape it into a NumPy array in preparation for making predictions
* We then convert it into a list. Using this list we create a while loop set for I<30. (Trying to predict 30 days into the future)
* we are using what is know as the sliding window technique for time series forecasting
* Using Matplot lib, we create a basic graph showing historical prices for the previous 100 days in blue, then plot another line for the following 30 days in yellow. (INSERT PREDICTION PIC)
* For comparison, we graphed available December data in tableau, placing prediction vs reality side by side.

# Prediction and visualization
The trained model is used to predict stock prices for the next 30 days. The results are visualized alongside the actual stock prices to assess the model's predictive accuracy. Following an analysis of our LSTM model for stock price prediction, we examined its performance on Johnson & Johnson and Pfizer stocks. While accurately forecasting a decline for JNJ, challenges arose with Pfizer, highlighting a 30% overall model accuracy. Recognizing the need for improvement, we acknowledge the impact of sudden market shifts and emphasize a strategic, risk-managed approach for real-life applications, emphasizing continuous model refinement and diversified investment decisions.

![Screenshot 2023-12-13 at 9 30 39 PM](https://github.com/samkimmmm/machine_learning_etf_price_prediction/assets/135805393/957c6776-16fc-4654-b757-02e917226599)

# Conclusion:
* Project Overview:The collaborative effort of our team culminated in a comprehensive project focused on forecasting stock prices, specifically within the healthcare sector.
* Historical Context:Explored the evolution of stock trading throughout history, offering a contextual foundation for our project's objectives.
* Utilizing Machine Learning:Employed the capabilities of machine learning, utilizing an LSTM model to predict future stock prices with precision.
* Technical Implementation:Illustrated the creation of our predictive model, employing the sliding window technique and Matplotlib for effective data visualization.
* Insights from Data Exploration:Shared key insights gained during the decision-making process, leading us to choose the LSTM model over Linear Regression, informed by a detailed exploration of our data.
* Optimizing Model Performance:Discussed the optimization process, ensuring a harmonious balance between accuracy and efficiency in our predictive model.
* Revealing Core Discoveries:Unveiled the effectiveness of the LSTM model in capturing sequential dependencies, serving as the foundational element of our predictive capabilities.
* Project Conclusion:Emphasized the robust capabilities of our LSTM model, offering valuable insights for investors and analysts navigating the intricate landscape of stock trading.

# Unquantifiable Factors:
* Presentation on historical performance trends of Johnson & Johnson (J&J) and Pfizer
* Focus on understanding factors shaping current stock prices and potential future impact
* Johnson & Johnson (J&J):
  * Demonstrated resilience amid market fluctuations
  * Diversified portfolio in pharmaceuticals, medical devices, and consumer health products
  * Consistent recovery despite legal issues related to some products
  * Steady growth with periodic dips linked to external events like lawsuits or regulatory concerns
* Pfizer:
  * Adaptability and growth, known for pharmaceutical breakthroughs
  * Market fluctuations influenced by product developments, patent expirations, and strategic decisions
  * Success driven by release of drugs and vaccines
  * Setbacks include patent expirations and challenges in drug development, but consistent rebounds
* Current stock prices influenced by recent events, particularly the global pandemic
* Factors influencing future stock performance:
  * Regulatory approvals, product pipelines, and market demand for healthcare products
  * Ongoing research and development efforts and adaptation to market dynamics
* Conclusion emphasizes resilience and ability of both companies to weather challenges
* Strategic decisions, innovations, and responses to external factors will shape future stock prices
* Importance for investors to understand dynamics in the pharmaceutical industry
