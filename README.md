# Time_Series_Analysis
![image](https://user-images.githubusercontent.com/109471364/179458093-46e8a783-1c92-4832-a95a-dcf86b9207e9.png)
## Background
Over $40 billion worth of cryptocurrencies are traded every day. They are among the most popular assets for speculation and investment, yet have proven wildly volatile. Fast-fluctuating prices have made millionaires of a lucky few, and delivered crushing losses to others. Could someof these price movements have been predicted in advance?

We have amassed a dataset of millions of rows of high-frequency market data dating back to 2018 which you can use to build your model. The simultaneous activity of thousands of traders ensures that most signals will be transitory, persistent alpha will be exceptionally difficult to find, and the danger of overfitting will be considerable. In addition, since 2018, interest in the crypto markethas exploded, so the volatility and correlation structure in our data are likely to be highly non-stationary.

Download the dataset from: https://www.kaggle.com/competitions/g-research-crypto-forecasting/data
## Tasks
1. Import asset_details.csv and train.csv after downloading the dataset from (https://www.kaggle.com/competitions/g-research-crypto-forecasting/data), state whether you need to perform any data preprocessing including outliers detection and handling missing values on this dataset, and also check for missing data for the timestamp column if any is missing values impute the data with appropriate methods and do other standard preprocessing steps if needed.
2. Make three subgroups of the data, consisting of the information of the following three cryptocurrencies: Bitcoin (Asset id:1 ), Ethereum (Asset id: 6), and Dogecoin (Asset id: 4). Split the time series datasets into a train (70%) and a test (30%).
3. Plot autocorrelation plots and decompose the sub-group data sets using the seasonal decompose function (statsmodels) and explain your key takeaways from plots in the report.
4. Explain the concepts of moving averages, and auto-regression in your report and construct the moving average and Arima equation for predicting the close and target for Bitcoin, Ethereum, and Dogecoin. Optimize the hyperparameters (p,d, and q) of ARIMA model to achieve the best accuracy in terms of MAPE (Mean Absolute percentage error).
5. Find RMSE(Root Mean Square Error) and MAPE (Mean Absolute percentage error) of predicted value and actual value from the test dataset.
6. Develop a machine learning model of your choice (ex: SVM, random forest regression) except linear regression and optimize the key hyperparameter to achieve the best accuracy to predict the close and target for Bitcoin, Ethereum, and Dogecoin. Repeat step 5 for the machine learning model and find RMSE and MAPE.
7. Plot bar chart of the accuracy of (RMSE and MAPE) of ARIMA and machine learning model for the different cryptocurrencies you have obtained from steps 4 and step 6.
8. Predict the next 10 days of future values of Bitcoin with your optimized machine learning and ARIMA models and plot the result.
