# XAU-USD-LSTM
This is my attempt on building a LSTM model for XAU-USD forecasting as a project for Machine Learning.<br>
Thanks to those who had me on the team to make this group project happened.<br><br>

<b>Background</b>:<br>
<i>*(To shorten things up)</i><br>
Gold price forecasting is critical in financial decision-making, providing valuable insights for investors and stakeholders in the gold market.
With the help of a computer, forecasting gold can be made possible and highly accurate by building an AI model that fits for the task.
A popular traditional model is used for this specific task is ARIMA (Autoregressive Integrated Moving Average) and has shown that it is capable on forecasting on seasonal time series.
In the recent trend of Neural Network, Long Short-Term Memory (LSTM) showed its power on a time series regression and have outperformed the ARIMA model on most cases.
The LSTM model is more robust and suitable as it is capable on capturing the complex and dynamic pattern on a time series data, hence this project was created on trying to build the model.<br><br>

The dataset was gained from Yahoo Finance and unfortunately Yahoo's data on gold had only started being recorded from 7 Feb 2020. The data was then preprocessed in order to be learn by the model.
We only decided to use the 'Close' prices as the independent variable (value to be predicted) and the Date as the dependent variable.
We also trained other models such as GRU and RNN to do a comparison on which model performs the best.
After training all the models, the LSTM model did a great job on the test set with a Mean Squarred Error (MSE) of around 0.0014. Weirdly, the RNN model performs the best with MAE, MSE, RMSE, MAPE and R-squarred score being excel to those in LSTM and GRU. This will be a future reconsideration on what happened on the comparison, also trying to forecast on more of the variables (such as Open, Close, Low, High pricing) as well with more comparison such as the ARIMA model that has been brought up.
