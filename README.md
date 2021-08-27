# Credit_Risk_Analysis
Supervised Machine Learning

## Overview of Analysis

Using supervised machine learning models, the client has requested an analysis of their provide credit card dataset in order to determine credit risk. For this analysis, the Random Over Sampler, SMOTE, Cluster Centroids, and SMOTEEN algorithms were used to resample the data and predict credit risk. Finally, the ensembel classifier models, Balanced Random Forest Classifier and Easy Ensemble Classifier, were used to predict credit risk and evalute the accuracy of each model. The next section will analyze the results of each algorith and model. The last section will provide a summary of the analysis and a recommendation of which method to apply to evaluate credit risk in the future.

## Results

For each of the six models used in this analysis, the provided dataset was first cleaned and trained for statistical analysis. Using Pandas DataFrames, this involved transforming all categorical data into numerical data using the get_dummies() method, removing the target data column, loan status, from the DataFrame, and finally splitting the data into training and testing sets using train_test_split from the sklearn.model_selection library. Once these steps were completed, I was able to use

* Random Over Sampler

## Summary
