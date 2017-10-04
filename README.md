# Ames, Iowa Housing Price Predictions

### Overview
I completed this project as part of a Kaggle competition (see here: https://www.kaggle.com/c/house-prices-advanced-regression-techniques). I visualized the various aspects of the dataset prior to cleaning null values and performing feature engineering. The main feature engineering work was to transform nominal features into numeric (boolean) features using pandas dummy variables, followed by empirical filtering of null values and correlation with the target value. The Extreme Gradient Boosting (XGBoost) decision-tree algorithm was used for modeling and prediction.

The metric used for scoring by Kaggle is the root mean squared logarithmic error (RMSLE). This metric is similar to the more common root mean squared error, but does not penalize as heavily for extreme differences between actual and predicted values due to the logarithm. My final RMSLE was 0.12189. When comparing my final result to other Kaggle competitors, my model places within the top 30% (~520 out of 1800) as of October 4th, 2017.

While this model could be further improved by additional feature engineering and more computational intensive machine learning algorithms, I was able to write this code from scratch in less than 5 hours. It's a relatively compact code that still achieves above average performance, with straight forward implemntation.

### Key Results
My RMSLE of 0.12189 would place ~520 out of 1800 entries (top 30%) as of October 4th, 2017.

### Methods used
seaborn for feature visualization
pandas dummy variables for transforming nominal features
XGBoost modeling and predictions
