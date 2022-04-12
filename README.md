# Inspiration
Through this project I wanted to explore how two wings of ML i.e. Sentiment Analysis and Time Series Forecasting go hand in hand.
**It can be seen as a hybrid model of NLP and TSF.**

# Steps
* As one of the column is highly skewed and transforming them will make our model more ininterpretable, so instead of using Linear Regression various Non-linear Regressor 
are used to find best RMSE value.
* Also while finding correlation heatmap, it was found that there was no strong correlation of variables with target variable, another resason to not go for Linear Regression.
 ![image](https://user-images.githubusercontent.com/102746816/163028700-f9be35ce-d80a-4a64-8fa3-9adde093cc6f.png)
* A SARIMAX model was built for 'Closing Price' which is our target variable
* The data from sentiment analysis is used as exogenous varibles to SARIMAX model.
