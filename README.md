# Credit_Risk_Analysis

## Overview
### We will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we'll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we'll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we'll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally we will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

### Oversampling

### * Naive Random Sampling
#### ![image](https://github.com/slafton/Credit_Risk_Analysis/blob/main/Images/NaiveRandomOversampling.png)
#### The precision for high-risk is 1% while the precision for low-risk is 100%. The sensitivity for high-risk is 65% and the sensitivity for low-risk is 60%. This model has an f1 of 78%.

### * SMOTE Oversampling
#### ![image](https://github.com/slafton/Credit_Risk_Analysis/blob/main/Images/SMOTEOversampling.png)
#### The precision for high risk is 1% and the precision for low-risk is 100%. The sensitivity for high-risk is 66% and the sensitivity for low-risk is 64%. This model has an f1 of 79%.

### * Undersampling
#### ![image](https://github.com/slafton/Credit_Risk_Analysis/blob/main/Images/Undersampling.png)
#### The precision for high risk is 1% and the precision for low-risk is 100%. The sensitivity for high-risk is 43% and the sensitivity for low-risk is 60%. This model has an f1 of 60%.

### * Combination (Over and Under) Sampling
#### ![image](https://github.com/slafton/Credit_Risk_Analysis/blob/main/Images/CominationSampling.png)
#### The precision for high risk is 1% and the precision for low-risk is 100%. The sensitivity for high-risk is 54% and the sensitivity for low-risk is 69%. This model has an f1 of 70%.

### Ensemble Learners

### * Balanced Random Forest Classifier
#### ![image](https://github.com/slafton/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForestClassifier.png)
#### The precision for high risk is 4% and the precision for low-risk is 100%. The sensitivity for high-risk is 91% and the sensitivity for low-risk is 67%. This model has an f1 of 95%.

### * Easy Ensemble AdaBoost Classifier
#### ![image](https://github.com/slafton/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleAdaBoostClassifier.png)
#### The precision for high risk is 7% and the precision for low-risk is 100%. The sensitivity for high-risk is 94% and the sensitivity for low-risk is 91%. This model has an f1 of 97%.

## Summary
### The Ensemble Learners models showed the best results with the high-risk precision slightly better with high-risk sensitivity high as well. This also increased the f1 dramatically compared to the other models. The problem with such low precision is that a lot of low risk credits would be falsely detected. This could cause the lending institution to miss out on a lot of revenue by missing those borrowers falsely labeled as high-risk. Therefore, I would not recommend any of these models to predict credit risk.