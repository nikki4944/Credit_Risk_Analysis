# Credit_Risk_Analysis
Supervised Machine Learning

## Overview of Analysis

Using supervised machine learning models, the client has requested an analysis of their provide credit card dataset in order to determine credit risk. For this analysis, the Random Over Sampler, SMOTE, Cluster Centroids, and SMOTEEN algorithms were used to resample the data and predict credit risk. Finally, the ensembel classifier models, Balanced Random Forest Classifier and Easy Ensemble Classifier, were used to predict credit risk and evalute the accuracy of each model. The next section will analyze the results of each algorith and model. The last section will provide a summary of the analysis and a recommendation of which method to apply to evaluate credit risk in the future.

## Results

For each of the six models used in this analysis, the provided dataset was first cleaned and trained for statistical analysis. Using Pandas DataFrames, this involved transforming all categorical data into numerical data using the get_dummies() method, removing the target data column, loan status, from the DataFrame, and finally splitting the data into training and testing sets using train_test_split from the sklearn.model_selection library. Once these steps were completed, I was able to use

* __Random Over Sampler__: As shown in the following image, the Random Over Sampler algorithm oversampled the data to create a model with 64.5% accuracy, a precison of 99%, and a sensitivity of 62%. 
<img width="809" alt="Random Over Sampling" src="https://user-images.githubusercontent.com/82982901/131135335-df499ff5-120f-42b0-a843-be6529a54221.png">

* __SMOTE__: As shown in the following image, the SMOTE algorith oversampled the data to create a model with 66.2% accuracy, a precision of 99%, and a sensitivity of 69%.
<img width="807" alt="SMOTE Oversampling" src="https://user-images.githubusercontent.com/82982901/131135395-ab1c06dd-ea98-4032-a207-5403a6bea64f.png">

* __Cluster Centroids__: As shown in the following image, the Cluster Centroids algorithm undersampled the data to produce a model with 54.5% accuracy, a precision of 99%, and a sensitivity of 40%.
<img width="795" alt="Cluster Centroids Undersampling" src="https://user-images.githubusercontent.com/82982901/131135416-bcb83da3-368e-4055-98c0-b0aafed5570d.png">

* __SMOTEEN__: As shown in the following image, the SMOTEEN algorith used a combination of under- and oversampling the data to create a model with 67.1% accuracy, 99% precision, and 58% sensitivity.
<img width="798" alt="SMOTEEN Combination" src="https://user-images.githubusercontent.com/82982901/131135438-ad56cb61-a725-42d3-b977-c068eac9cb27.png">

* __Balanced Random Forest__: As shown in the following image, the Balanced Random Forest Classifier used the data to create a model with 78.8% accuracy, a precision of 99%, and a sensitivity of 87%.
<img width="808" alt="Balanced Random Forest" src="https://user-images.githubusercontent.com/82982901/131135456-66eceaaf-7b92-49c5-8f48-464e4337ca22.png">

* __Easy Ensemble__: As shown in the following image, the Easy Ensemble Classifier used the data to create a model with 93.2% accuracy, a precision of 99%, and a sensitivity of 94%.
<img width="805" alt="Easy Ensemble" src="https://user-images.githubusercontent.com/82982901/131135469-fde83789-8422-4f0c-8ddb-836a96fe2006.png">

## Summary

Since all of the models operated with an extremely high degree of precision, this is not a good indicator for determingin which model performed the best as all of the models were very precise. Precision is calculated by dividing all the true positives by the sum of the true positives and false positives shown in the confusion matrices. 

Sensitivity and precision often work with a strong degree of tension. Sensitivity percentages are agressive indicators meaning the model does well at detecting good credit risk but it also runs the risk of in high number of false positivies. Sensitivity percentage is calculated by dividing the true positives by the sum of the true positives and the false negatives produced by the confusion matrix. 

Based on the results of each of the models, it is recommended that the Easy Ensemble Classifier model be used to predict credit risk when evaluating loan applications in the future. This model operated with the highest degree of accuracy, precision and sensitivity.
