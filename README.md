# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2 : Ames Housing Price Predictions (Kaggle Challenge)


## Problem Statement
The main objective of this project is to create a regression model based on the Ames Housing Dataset. This model will predict the price of a house at sale using the data provided. Using the Ames Housing Dataset, we will create a regression model that predicts the prices of houses in Ames, Iowa. Dataset consists of features that are continuous, discrete, ordinal, and nominal.



## Executive Summary
The Ames Housing Data Set contains information from the Ames Assessor’s Office used in computing the value of individual residential properties sold in Ames, Iowa from 2006 to 2010, as well as the actual eventual sale prices for the properties.

The data set contains information for more than 2900 properties. The data dictionary outlines more than 75 descriptive variables. Some are nominal (categorical), meaning they are non-numerical and lack clear-cut order (Examples: Neighborhood, Type of roofing). Some are ordinal, meaning they are categorical but have a clear order (Example: Heating Quality (Excellent, Good, Average, Poor)). Some are discrete, meaning they are numerical but at set intervals (Year Built, Number of Fireplaces). The rest are continuous, meaning they are numerical and can theoretically take any value in a range (1st Floor Square Feet).

In this project, I have attempted to craft as accurate a model as possible for predicting housing sale prices, using regression techniques, enhanced by feature engineering, feature selection, and regularization. This project was connected to a private Kaggle competition. The Ames data set was divided into a labeled training set, and an unlabeled test set (the labels exist, but are withheld). I aim to accurately predict the withheld sale prices for the test set, based on the features and prices in the training set. This exercise mimics real-world modeling scenarios.

This Jupyter notebook walks through the clean up of the train dataset, explores various sample statistics, trends and correlations. It includes creating a regression model based on the Ames Housing Dataset, to predict the prices of houses at sale. The success of the model will be evaluated by scores obtained. The main metrics used to evaluate the success of the model is the R2 and RMSE values.



## Contents
- Data Import
- Data Cleaning
- Explanatory Data Analysis
- Modeling and Preprocessing
- Conclusions and Recommendations



## Data Dictionary
Data Dictionary can be found at this link: https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/data


## Conclusions and Recommendations

Our key findings from this project were:
- There were a large number of null values in the dataset. Instead of dropping them, we filled them methodically, always having a logical reason behind why we are filling a certain value in.
- The remaining features left in our final model consisted of some of our feature engineered columns (total_area, total_baths, house_age) along with some mainstay features like 'overall_qual', '1st_flr_sf', 'garage_area', 'neighborhood', 'mas_vnr_area'.
- Many of the initial featuers were heavily skewed in their data distribution and hence would not be strong predictors of house prices in our models.


Recommendations for future analysis:
- Include more feature engineered features into initial modeling stages
- Conduct further qualitative research into connumer preferences that would affect housing demand and prices in the Ames area.
- Try different sets of features in our models to have a wider set of model scores to choose from.
