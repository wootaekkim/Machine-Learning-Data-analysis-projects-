# Data-analysis-projects-

Here we have three data analysis projects. Below illustrates brief introduction of each proejcts

1.Bank Customer Churn Prediction
This is done using dataset from Kaggle.
Here what I have done is predict whether customer would leave or not based on the features.
In the process of doing so, I have used XGBoost, LightGBM, AdaBoost and Logistic Regression.

2. Monitor Deals Price Prediction
This is also done using dataset from Kaggle.
Our main goal was to predict price of computer monitors based on the data.
Here, the main difficulty was dealing with missing data. I have removed all the feautres that had more than 40% missing rate.
Then to fill missing values, I filled them in with mean of that feature of which belongs to same category in other feature.
For prediction, I have mainly used tree based algorithms such as XGBoost and LightGBM as distribution of the features were very far from normal distribution. Yet I still used boxcox to increase prediction accuracy.

4. Steam Release Ratings Prediction
Just as above two projects, this is also done using dataset from Kaggle.
Goal of this project was to predict ratings of the games released on Steam which is a video game digital distribution service.
Here I have combined two features which had high correlation coefficients Which turned out to have highest features importance.
For prediction, I mostlyt used tree based models such as XGBoost and LightGBM then combined them all using stacked model.
