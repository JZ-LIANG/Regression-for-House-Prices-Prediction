# Challenge: What is the future selling price of a home?

This challenge (adapted from [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)) aims at predicting selling prices of a number of houses. To predict these prices, we are given a training set (with known selling prices), and for each house, we are given around 79 characteristics (total area, building materials, number of floors, ...). 

### Our approach

We decided to really study the training dataset in depth before thinking about predicting. This data analysis aimed at understanding the statistics and correlation of the data features as well as what kind of features engineering and transforms need to be done before they are ready to be use for prediction. We spent quite a lot of time on analyzing and our data and perform features engineering. 

We decide to use regression model for prediction.  We choose different Regularizations and evaluate their performances using cross-validation. we also perform the Stacked Generalization models ensembling to avoid the regression overfiting problem.

Steps: 
 * Descriptive statistics about the data
 	* skewness analysis
 	* Features Splitting: Categorical/Ordinal/Numerical, and statistic for each group 
 	* features correlation
 * Data cleaning and pre-processing and features engineering
 	* missing data, outerliers, invalid data
 	* Outliers removal
 	* Features encoding
 	* Construct new features
 	* features normalization and rescaling
 * Training and evaluate baseline models
 	* Explore the effects of the different regularizations: apply Lasso, Ridge and ElasticNet.
 	* Using a grid search approach to find the best parameters.
 * Stack models to build final model
 	* XGboost 
 	* Stacked generalization
 * Validate the outcome of the model