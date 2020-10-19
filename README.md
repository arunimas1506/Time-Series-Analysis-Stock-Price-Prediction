# Time-Series-Analysis-Stock-Price-Prediction

Objective:
The objective is to use machine learning algorithms to make predictions about the direction
and magnitude of the price.

Description:
Given the data of historical stock prices, predict the direction and potentially magnitude of the
move. Overall, this is an event modeling exercise where each event contains actual result,
forecasted result and previous result. We think that the bigger the difference between actual vs.
forecast, the bigger the impact on item # 7.
The problem is that, you have to predict # 7 (or potentially log difference between 5 shifted by
1), if on the day you will have actual, forecast, rolling_std, z-score and 1.

Input:
Given set of input data files
• stock price [1: open, 5: close, 6: volume, 7: log difference between successive close]
• derived features [rolling_std, z-score, 7]
You’re given two set of files n.csv and o.csv and the goal is to fit two different models.

Output:
Model

Code:
The code should contain following parts
1. Model generation
2. Model save
3. Model retrieval and prediction function
4. Train | Test split and accuracy

NOTE:
Overall, in order to predict for next day you may want to lag the data by 1 day. Also, for the
purposes of prediction you can even ignore the date.

