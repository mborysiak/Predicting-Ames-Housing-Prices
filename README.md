# Ames, Iowa Housing Price Predictions

### Overview
I completed this project as part of a Kaggle competition (see here: https://www.kaggle.com/c/house-prices-advanced-regression-techniques). I visualized the various aspects of the dataset prior to cleaning null values, feature engineering, and creating an ensemble model. 

I generated ensemble predictions with the the Extreme Gradient Boosting (XGBoost) decision-tree algorithm and Ridge regression. Prior to creating the XGBoost model, I performed hyper-parameter grid search optimization to prevent over-fitting the training data during cross-validation. 

The metric used for scoring by Kaggle is the root mean squared logarithmic error (RMSLE). This metric is similar to the more common root mean squared error, but does not penalize as heavily for extreme differences between actual and predicted values due to the logarithm. 

The RMSLE for out-of-sample data with 10-fold cross-validation on the training set was 0.1129 and 0.1096 for the XGBoost and Ridge model respectively. Each model scored approximately 0.1220 separately on the un-labeled test set from Kaggle (with the Ridge performing slightly better). Combined, the models gave a final RMSLE was 0.11775 for the Kaggle test set. When comparing my final result to other Kaggle competitors, my model places within the top 15% (~365 out of 2410) as of November 16th, 2017 (username: markborysi). 

Additional work with feature engineering, including more models to the ensemble, and improving the replacement of null values / outliers could potentially further improve this model.

### Key Results
My RMSLE of 0.11775 would place ~365 out of 2410 entries (top 15%) as of November 16th, 2017.

### Methods used
- seaborn for feature visualization
- pandas dummy variables for transforming nominal features
- XGBoost modeling and predictions
- Ridge Regression
- Grid-search parameter optimization
