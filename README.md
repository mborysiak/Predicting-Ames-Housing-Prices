# Ames, Iowa Housing Price Predictions

### Overview
I completed this project as part of a Kaggle competition (see here: https://www.kaggle.com/c/house-prices-advanced-regression-techniques). I visualized the various aspects of the dataset prior to cleaning null values, feature engineering, and creating an ensemble model. 

I generated ensemble predictions consisting of the the Extreme Gradient Boosting (XGBoost) decision-tree algorithm and Ridge regression. Prior to creating the XGBoost model, I performed hyper-parameter grid search optimization to prevent over-fitting the training data during cross-validation. 

The metric used for scoring by Kaggle is the root mean squared logarithmic error (RMSLE). This metric is similar to the more common root mean squared error, but does not penalize as heavily for extreme differences between actual and predicted values due to the logarithm. My final RMSLE was 0.11824. When comparing my final result to other Kaggle competitors, my model places within the top 15% (~385 out of 2400) as of November 14th, 2017. 

Additional work with feature engineering, adding additional models to the ensemble, and improving the replacement of null values / outliers could potentially further improve this model.

### Key Results
My RMSLE of 0.11824 would place ~385 out of 2400 entries (top 30%) as of November 14th, 2017.

### Methods used
- seaborn for feature visualization
- pandas dummy variables for transforming nominal features
- XGBoost modeling and predictions
- Ridge Regression
