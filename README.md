# Credit_Risk_Analysis

## Overview
### We will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we'll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we'll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we'll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally we will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
### * Random Over Sampler Model
#### ![image]()
#### The balanced accuracy score is 65%.The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only. Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### * SMOTE Model
#### ![image]()
#### 
## Summary
