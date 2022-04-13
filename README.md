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
* The 'Time Varying Linear Regression' model gave the best result in terms of RMSE value.

 ![image](https://user-images.githubusercontent.com/102746816/163111816-af8ffb0a-759a-4fcd-ba84-d12f944c9e17.png)

* Also prediction for next 30 days are done and plotted along with their **confidence interval** as predicting robust numbers can be misleading.

![image](https://user-images.githubusercontent.com/102746816/163111974-0454efda-e3ce-4660-8921-d6c8e1e0e461.png)

# Conclusion
 It was observe when there is an auto-corelation between the entries of data, it's better to go for TSF instead of traditional regressors.

