# Credit_Risk_Analysis

## Overview:

Thw aim of this project was to apply machine learning methods to solve a real-world challenge: credit card risk. Estimating credit risk is a challenging classification problem because good loans easily outnumber risky loans. A number of different techniques were employed to train and evaluate models with unbalanced classes. Imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling was employed using the SMOTEENN algorithm. Next, two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, were used to predict credit risk. Finally, the performance of these models were evaluated to make recommendation on whether these models  should be used to predict credit risk.

### Tools
- Methods: RandomOverSampler and SMOTE algorithms for over sampling, ClusterCentroids algorithm for undersampling, and SMOTEEN algorithm for combinatorial over and undersampling
- Python, Pandas
- Scikit Learn
- Imbalanced-learn
- Git

## Results:

Analysis results using Randon Oversampling, SMOTE Oversampling, Undersampling, SMOTEEN (Combination of Over and Undersampling), Balanced Random Forest Classifier, and Easy Ensemble AdaBoost Classifier algorithms are shown below. The confusion matrix and the balanced classification report is also included below. 

**1. Random Oversampling**
- Balanced accuracy score is 0.66
- Precisision for predicting lower risk is 1.0
- Precisision for predicting higher risk is 0.01
- Recall for predicting lower risk is 0.6
- Recall for predicting higher risk is 0.68
- F1 score for predicting lower risk is higher (0.81)
- F1 score for predicting higher risk is very poor (0.02)

So, it shows that this is not a good model for predicting higher credit risk

**1a. Confusion matrix for model with random oversampling**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        55         |        32        |
| Low Risk (Actual)  |       5455        |      11663       |      
       
 
**1b. Imbalanced classification report for model with random oversampling**

![ROS](/images/ROS.png)

       
**2. SMOTE Oversampling**
- Balanced accuracy score is 0.63 
- Precisision for predicting lower risk is 1.0
- Precisision for predicting higher risk is 0.01
- Recall for predicting lower risk is 0.61
- Recall for predicting higher risk is 0.64
- F1 score for predicting lower risk is 0.78
- F1 score for predicting higher risk is very poor (0.02)
       
So, it shows that this is not a good model for predicting higher credit risk

**2a. Confusion matrix for model with SMOTE Oversampling**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        53         |        34        |
| Low Risk (Actual)  |       6135        |      10983       |  


**2b. Imbalanced classification report for model with SMOTE Oversampling**

![SMOTE](/images/SMOTE.png)

       
**3. Undersampling**
- Balanced accuracy score is 0.52
- Precisision for predicting lower risk is 1.0
- Precisision for predicting higher risk is 0.01
- Recall for predicting lower risk is 0.43
- Recall for predicting higher risk is 0.60
- F1 score for predicting lower risk is 0.60
- F1 score for predicting higher risk is 0.02

So, it shows that this is not a good model for predicting higher credit risk

**3a. Confusion matrix for model with Undersampling**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        52         |        35        |
| Low Risk (Actual)  |       9681        |       7437       |  


**3b. Imbalanced classification report for model with Undersampling**

![Under Sampling](/images/UNDER.png)

       
**4. SMOTEENN (Combination of Over and Undersampling)**
- Balanced accuracy score is 0.62
- Precisision for predicting lower risk is higher (1.0)
- Precisision for predicting higher risk is very poor (0.01)
- Recall for predicting lower risk is 0.53
- Recall for predicting higher risk is 0.71
- F1 score for predicting lower risk is 0.69
- F1 score for predicting higher risk is very poor (0.02)

So, it shows that this is not a good model for predicting higher credit risk

**4a. Confusion matrix for model with combination of Over and Undersampling (SMOTEEN)**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        62         |        25        |
| Low Risk (Actual)  |       8008        |       9110       |  

**4b. Imbalanced classification report for model with combination of Over and Undersampling (SMOTEEN)**

![SMOTEEN](/images/SMOTEEN.png)

       
**5. Balanced Random Forest Classifier**
- Balanced accuracy score is 0.79
- Precisision for predicting lower risk is higher (1.0)
- Precisision for predicting higher risk is very poor (0.04)
- Recall for predicting lower risk is 0.67
- Recall for predicting higher risk is 0.91
- F1 score for predicting lower risk very poor (0.07)
- F1 score for predicting higher risk is higher (0.95)

This model seems to have a higher recall and F1 score. However, it does not have a good precision. 
So, it shows that this might not be a good model for predicting higher credit risk.

**5a. Confusion matrix for model with Balanced Random Forest Classification**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        58         |        29        |
| Low Risk (Actual)  |       1560        |      15558       |  


**5b. Imbalanced classification report for model with Balanced Random Forest Classifiier**

![BRF](/images/BRF.png)


**6. Easy Ensemble AdaBoost Classifier**
-  Balanced accuracy score is 0.93
-  for predicting lower risk is higher (1.0)
- Precisision for predicting higher risk is very poor (0.07)
- Recall for predicting lower risk is 0.94
- Recall for predicting higher risk is 0.91
- F1 score for predicting lower risk is higher (0.97)
- F1 score for predicting higher risk is very poor (0.14)

This model seems to have a higher recall for predicting lower and higher risks. However, it does not have a good precision for F1 score for predicting lower risk. 

So, it shows that this might not be a good model for predicting higher credit risk.


**6a. Confusion matrix for model with Easy Ensemble AdaBoost Classifier**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        79         |        35        |
| Low Risk (Actual)  |       979         |      16139       |  

**6b. Imbalanced classification report for model with Easy Ensemble AdaBoost Classifier**

![EEC](/images/eec.png)

Features important for prediction of credit risk in Balanced Random Forest Classifier are shown below.

![Features](/images/features.png)

![Feature_List](/images/feature_list.png)
 

## Summary:
IN SUMMARY, the model with the undersampling algorithm had the highest false positives (FP) and the lowest number of true negatives (TN, low risk). The Balanced Random Forest Classifier and the Easy Ensemble AdaBoost Classifier performed better when compared to other models.  The best model out of all 6 models is the model with Easy Ensemble AdaBoost Classifier. It had the highest number of TP (Higher risk), TN (Lower Risk), and a lower number of FP and FN (false negatives) compared with other models. However, this model was also not performing well for predicting credit card risk (higher or lower) because it also had a larger number of FP and FN. It may be worth trying to optimize this model by model parameters (e.g., number of iterations, selecting ONLY important features with high ranks etc.) 

None of these 6 models cannot be recomended to predict credit risk accurately because of the reasons outlined above. This further demonstrates the issu with imbalanced credit targets (lower or higher risk), because good loans outnumber bad loans.  
