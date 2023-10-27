# **Stock Price Prediction**
# ***Enhancing Stock Price Prediction: A Transition from Linear Regression to CNN***
# About Dataset
## Context
Tata Steel Limited is an Indian multinational steel-making company based in Jamshedpur, India. It is a subsidiary of the Tata Group.
Tata Steel historic stock dataset can be used for EDA, stock performance and stock price forecasting.

## Content
Dataset contains daily Opening price, High price, Low price, Closing price, Number of shares, Number of trades, etc. of TATA STEEL Ltd stock from (03-july-2015 till 02-july-2021).

Other Features : Date, Open Price, High Price, Low Price, WAP, No.of Shares, No. of Trades, Total Turnover, Deliverable Quantity, Deli. Qty to Traded Qty, Spread High-Low, Spread Close-Open

Target Feature : Close price

# Implementations
1.  Importing all the required libraries
2.  Data Extraction - Collected the data from Kaggle.
3.  Data Preprocessing - Null Values and checking features datatypes
4.  Exploratory Data Analysis - Used Seaborn & Matplotlib
5.  Feature Scaling - Normalizing the top corelated data with Minmax Scaler
6.  Data split - 80:20 split as Train-Test Split.
7.  Prediction Model - Linear Regression, ANN, CNN
8.  Model Evaluation - Calculated the metric Accuracy
9.  Model Comparison - Compared the accuracy of all models
10. Converting data - To a time series format
11. Prediction Model - LSTM, ANN, CNN
12. Model Evaluation - Calculated the metric Accuracy
13. Model Comparison - Compared the accuracy of all models

# ***What is the Stock Market?*** 

The stock market refers to the collection of markets and exchanges where regular activities of buying, selling, and issuance of shares of publicly-held companies take place. Such financial activities are conducted through institutionalized formal exchanges or over-the-counter (OTC) marketplaces which operate under a defined set of regulations. There can be multiple stock trading venues in a country or a region which allow transactions in stocks and other forms of securities.

# ***Understanding the Problem Statement***

Broadly, stock market analysis is divided into two parts – Fundamental Analysis and Technical Analysis.

1. Fundamental Analysis involves analyzing the company’s future profitability on the basis of its current business environment and financial performance.
2. Technical Analysis, on the other hand, includes reading the charts and using statistical figures to identify the trends in the stock market.

My focus is on the technical analysis part.

# ***Major Points of Understanding***

- There are multiple variables in the dataset – Date, Open, High, Low, Close and volume.

- The columns Open and Close represent the starting and final price at which the stock is traded on a particular day.

- High and Low represent the maximum and minimum price of the share for the day.

- Deliverable Quantity is the number of shares bought or sold in the day.

- The profit or loss calculation is usually determined by the closing price of a stock for the day, hence we will consider the closing price as the target variable.

- Created a "Change" column  which contains the percentage change from the "Open" price to the "Close" price, rounded to two decimal places, with 100 subtracted to express it as a percentage relative to the "Open" price.

# ***Converting data - To a time series format***
- Converting normal data to a time series format is necessary when the data has a temporal component or exhibits time-dependent trends.
- Time series data captures sequential dependencies, enabling forecasting and anomaly detection.
- This conversion helps uncover hidden patterns and facilitates effective visualization of temporal changes.

# ***Conclusion***
The transition from linear regression to CNN for stock price prediction can be attributed to the following factors:

- **Complex Patterns:** Stock prices exhibit intricate, non-linear patterns and dependencies. Linear regression struggles to capture such complexity, while CNN excels in identifying intricate spatial and temporal patterns.

- **Temporal Transformation:** Converting data to a time series format highlights the significance of temporal dependencies. LSTM and CNN models are specifically designed for time series data, enabling them to leverage temporal information effectively.

- **Automatic Feature Extraction:** CNNs automatically learn and extract relevant features from the raw data, providing better representation of intricate stock price patterns.

- **Nonlinearity:** CNNs are inherently non-linear models, making them more suitable for modeling the non-linear relationships in stock prices.

- **Model Capacity:** CNNs have greater model complexity and capacity to capture complex, multi-dimensional relationships, which is beneficial for capturing the intricate behavior of stock prices.
