# Data-analysis-projects-

Here we have three data analysis projects focused on data cleaning, feature engineering, and use of machine learning algorithms.<br>
Below are brief introduction of each project.


1. Bank Customer Churn Prediction

This is done using dataset from Kaggle.
Here what I have done is predict whether customer would leave or not based on the features.
In the process of doing so, I have used XGBoost, LightGBM, AdaBoost and Logistic Regression. Lastly, I used Stacked model which gave me the best result of False Positive Rate of 16.8%. The reason I used False Positive Rate as my measure of performance of models is beacause Falsely predicting that a customer would stay would create more lost thatn falsely predicting customer would leave as loosing a customer would create more loss to the company. This is because high false positive rate means company will loose customer without being able to foreseeing or being able handle them before hand. 

2. Monitor Deals Price Prediction

This is also done using dataset from Kaggle.
Our main goal was to predict price of computer monitors based on the data.
Here, the main difficulty was dealing with missing data. I have removed all the feautres that had more than 40% missing rate.
Then to fill missing values, I filled them in with mean of that feature of which belongs to same category in other feature.
For prediction, I have mainly used tree based algorithms such as XGBoost and LightGBM as distribution of the features were very far from normal distribution. Yet I still used boxcox to increase prediction accuracy. As a result of train and prediction of date using various models, I got the best performance of RMSE score 0.41 from using Gradient Boosting Algorithm.

3. Steam Release Ratings Prediction

Just as above two projects, this is also done using dataset from Kaggle.
Goal of this project was to predict ratings of the games released on Steam which is a video game digital distribution service.
Here, as part of feature engneering process I have combined two features which had high correlation coefficients Which turned out to have the highest features importance.
For prediction, I mostly used tree based models such as XGBoost and LightGBM then combined them all using stacked model. After trials of train and prediction preocesses using various models, I got the best result from Stacked model with RMSE score 0.097. 
