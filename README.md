# Data-analysis-projects-

Here we have three data analysis projects focused on data cleaning, feature engineering, and use of machine learning algorithms.<br>
Below are brief introduction of each project.


### 1. Bank Customer Churn Prediction

This is done using dataset from Kaggle.<br />
Here my goal was to predict whether customer would leave or not based on the features.<br />
In the process of doing so, I have used XGBoost, LightGBM, AdaBoost and Logistic Regression. Then, I used Stacked model which gave me the best result of False Positive Rate of 16.8%. The reason I used False Positive Rate as my measure of performance of models was beacause Falsely predicting that a customer would stay would create more lost thatn falsely predicting customer would leave as loosing a customer would create more loss to the company. This is because high false positive rate means company will loose customer without being able to foreseeing or being able handle them before hand. 

### 2. Monitor Deals Price Prediction

This is also done using dataset from Kaggle.<br />
My main goal was to predict price of computer monitors based on the data.<br />
Here, the main difficulty was dealing with missing data and cleaning data. In the processes of cleaning data the biggest task was combining all the same companies from Manufacturer feature to one. To do so, I capitalized all the letter so that I can better detect the same companies. Then I used pandas to combine same companies as one category. To continue, in terms of dealing with missing data, I have removed all the feautres that had more than 40% missing rate. To fill missing values remaining features, I filled them in with mean of that feature of which belongs to same Manufacturer and same price range(+/-20).<br />
For prediction/modeling process, I have mainly used tree based algorithms such as XGBoost, LightGBM and Gradient Boosting algorithm as distribution of the features were very far from normal distribution. Yet I still used boxcox to increase prediction accuracy. As a result of train and prediction of date using various models, I got the best performance of RMSE score 0.41 from using Gradient Boosting Algorithm.

### 3. Steam Release Ratings Prediction

Just as above two projects, this is also done using dataset from Kaggle.<br />
Goal of this project was to predict ratings of the games released on Steam which is a video game digital distribution service.
Here, as part of feature engneering process I have combined two features which were number of positive review and negative reviews. I changed them into positive/negative ratios and this turned out to be the most influential feature for predicting ratings of released games. There were also two other features with high correlation; number total reviews and peak players.I did not remove one of them as doing so led to decrease in accuracy of predictions. Another reason was that high correlation of two features does no reduce the accuracy of tree based models which I chose to predict ratings for this case. <br />
Tree based models I used for prediction were LGBM, XGBoost. The reason I chose tree based model was beacuase most of the features of the dataset were far from normal distribution.
Then to increase accuracy, I used stacked model of all tree based model I used. t After trials of train and prediction preocesses using various models, I got the best result from Stacked model with RMSE score 0.097. 
