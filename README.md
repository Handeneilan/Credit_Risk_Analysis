# Credit_Risk_Analysis

## Overview of the Project
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. We have been asked to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results

### Naive Random Oversampling
![Naive Random Oversampling](https://user-images.githubusercontent.com/104239978/203693516-d4ebc649-ee08-40d1-a51a-0aa0531de198.png)

The balanced accuracy score is 0.6515938052705158
The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### SMOTE Oversampling
![SMOTE oversampling](https://user-images.githubusercontent.com/104239978/203694219-b2cd8d16-bdb6-4309-a84a-cc8813a08096.png)

The balanced accuracy score is 0.6241876870888075
The high_risk precision is about 1% only with 59% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.

### Under Sampling
![under sampling](https://user-images.githubusercontent.com/104239978/203696609-5b22f226-c7a0-4bd8-b091-dd0a9c6c3034.png)

The balanced accuracy score is 0.6241876870888075
The high_risk precision is about 1% only with 60% sensitivity which makes a F1 of 1% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 43%.

### Combination Sampling
![combination sampling](https://user-images.githubusercontent.com/104239978/203696921-8d2248cb-5e91-4bde-a438-a0f303ac74ae.png)

The balanced accuracy score is 0.5159904274991842
The high_risk precision is about 1% only with 70% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 58%.

### Balanced Random Forest Classifier
![balanced random forest classfier](https://user-images.githubusercontent.com/104239978/203697158-2103a89e-1a9f-408b-a71a-25441d6f668b.png)

The balanced accuracy score is 0.7877672625306695
The high_risk precision is about 4% with 67% sensitivity which makes a F1 of 7% only.
Now the low_risk sensitivity is down to 91% with 100% presicion because of the number of false-positives

### Easy Ensemble AdaBoost Classifier
![easy ensemble adaboost classifier](https://user-images.githubusercontent.com/104239978/203697688-d5f0b6a9-f82b-4db7-9f76-50597235b3f6.png)

The balanced accuracy score is 0.925427358175101
The high_risk precision is about 7% with 91% sensitivity which makes a F1 of 14% only.
Now the low_risk sensitivity is now litte bit higher and is 94% with 100% presicion because of the number of false-positives.

## Summary
Based on the data set, I would recommend using the ADABoost Classifier since it has the highest recall rate and highest accuracy score.






