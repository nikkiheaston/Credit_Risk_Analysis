# Credit Risk Analysis

## Purpose

The purpose of this analysis is to compare the results of six different machine learning models to determine the best one to use in examining credit risk, specifically high-risk applications. Values for balanced accuracy, and precision and recall are highlighted below. I used Python supervised machine learning models - from scikit-learn and imbalanced-learn libraries - in this repo.

## Results

### Balanced Accuracy Scores
 - Naive Random Oversampling - 0.66
 - SMOTE Oversampling - 0.66
 - Cluster Centroid Undersampling - 0.55  
 - Combination (Over and Under) Sampling SMOTEENN - 0.67
 - Balanced Random Forest Classifier - 0.79
 - Easy Ensemble AdaBoost Classifier - 0.93

### Precision & Recall Scores

Below are screenshots taken from each model's classification report:

Naive Random Oversampling

![Naive Random Oversampling](https://github.com/nikkiheaston/Credit_Risk_Analysis/blob/main/Resources/Naive%20Random%20Oversampling.PNG)

SMOTE Oversampling

![SMOTE Oversampling](https://github.com/nikkiheaston/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20Oversampling.PNG)

Cluster Centroid Undersampling

![Undersampling Cluster Centroids](https://github.com/nikkiheaston/Credit_Risk_Analysis/blob/main/Resources/Undersampling%20Cluster%20Centroids.PNG)

Combination Sampling SMOTEENN

![Combination Sampling SMOTEENN](https://github.com/nikkiheaston/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN.PNG)

Balanced Random Forest Classifier

![Balanced Random Forest Classifier](https://github.com/nikkiheaston/Credit_Risk_Analysis/blob/main/Resources/Balanced%20Random%20Forest%20Classifier.PNG)

Easy Ensemble AdaBoost Classifier

![Easy Ensemble AdaBoost Classifier](https://github.com/nikkiheaston/Credit_Risk_Analysis/blob/main/Resources/Easy%20Ensemble%20AdaBoost%20Classifier.PNG)

The following is a list of precision and recall scores for each model: 
 - Naive Random Oversampling
    - Precision: 0.01 
    - Recall: 0.72

 - SMOTE Oversampling 
    - Precision: 0.01 
    - Recall: 0.62

 - Cluster Centroid Undersampling 
    - Precision: 0.01 
    - Recall: 0.69

 - Combination (Over and Under) Sampling SMOTEENN 
    - Precision: 0.01 
    - Recall: 0.77

 - Balanced Random Forest Classifier 
    - Precision: 0.03 
    - Recall: 0.70

 - Easy Ensemble AdaBoost Classifier 
    - Precision: 0.09 
    - Recall: 0.92





## Summary

As is shown above, all six models have produced poor precision scores. The balanced accuracy scores for the ensemble learing models are better than the others, with AdaBoost performing the best. Recall scores tend to be the highest overall scores across all six models; the best model being AdaBoost. Because lending is such a lucrative business I would not recommend using any of these models and continue searching. Although these models are pretty good at minimizing incorrectly predicted low risk applications that are actually high risk, lenders could miss out on a lot of dollars by predicting such a high number of false positives. 
