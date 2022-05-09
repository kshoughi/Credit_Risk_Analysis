# Credit_Risk_Analysis
## Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, employing different techniques to train and evaluate models with unbalanced classes is necessary. The purpose of this project is to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, I evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.

## Results
The summary of the balanced accuracy score, precision and recall for different methods are described below:  

### Random Oversampling:   
- balanced_accuracy_score: 0.6605  
- Precision: high risk 0.01, low risk 1.00  
- Recall: high risk 0.68, low risk 0.64

### SMOTE Oversampling
- balanced_accuracy_score: 0.655  
- Precision: high risk 0.01, low risk 1.00   
- Recall: high risk 0.61, low risk 0.70

### Undersampling
- balanced_accuracy_score: 0.655  
- Precision: high risk 0.01, low risk 1.00  
- Recall: high risk 0.69, low risk 0.40

### Combination 
- balanced_accuracy_score: 0.645  
- Precision: high risk 0.01, low risk 1.00   
- Recall: high risk 0.72, low risk 0.57

### Balanced Random Forest
- balanced_accuracy_score: 0.788  
- Precision: high risk 0.03, low risk 1.00  
- Recall: high risk 0.70, low risk 0.87

### Easy Ensemble AdaBoost 
- balanced_accuracy_score: 0.931  
- Precision: high risk 0.09, low risk 1.00   
- Recall: high risk 0.92, low risk 0.94


## Summary
It can be seen that Easy Ensemble AdaBoost method is superior compared to other methods. It results in higher balanced accuracy score, precision, and recall as shown below: 

![img1](https://github.com/amirimah/Credit_Risk_Analysis/blob/main/Screenshots/Easy%20Ensemble%20AdaBoost.png?raw=true)  
  
However, precision for high-risk group is still very low (ie. 0.09). Since precision is a measure of how reliable a positive classification is, I would recommend neither of these methods as none are reliable for high-risk groups. Therefore, more data is needed for a reliable recommendation. 

## 
**Contact:**  
**E-mail: mahtab.2010am@gmail.com**
