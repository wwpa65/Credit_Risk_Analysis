# Credit_Risk_Analysis

## Overview:

Thw aim of this project was to apply machine learning methods to solve a real-world challenge: credit card risk. Estimating credit risk is a challenging classification problem because good loans easily outnumber risky loans. A number of different techniques were employed to train and evaluate models with unbalanced classes. Imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling was employed using the SMOTEENN algorithm. Next, two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, were used to predict credit risk. Finally, the performance of these models were evaluated to make recommendation on whether these models  should be used to predict credit risk.

**Tools**
- Methods: RandomOverSampler and SMOTE algorithms for over sampling, ClusterCentroids algorithm for undersampling, and SMOTEEN algorithm for combinatorial over and undersampling
- Python, Pandas
- Scikit Learn
- Imbalanced-learn
- Git

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. 

Analysis results using Randon Oversampling, SMOTE Oversampling, Undersampling, SMOTEEN (Combination of Over and Undersampling), Balanced Random Forest Classifier, and Easy Ensemble AdaBoost Classifier algorithms are shown below.

- RandoM Oversampling
-      Precisision for predicting lower risk is higher (1.0)






- Precisision for predicting higher risk is very poor (0.01)
       - Recall for predicting lower risk is 0.63
       - Recall for predicting higher risk is 0.68
       - F1 score for predicting lower risk is higher (0.81)
       - F1 score for predicting higher risk is very poor (0.02)
       - So, it shows that this is not a good model for predicting higher credit risk
       
- SMOTE Oversampling
       - Precisision for predicting lower risk is higher (1.0)
       - Precisision for predicting higher risk is very poor (0.01)
       - Recall for predicting lower risk is 0.61
       - Recall for predicting higher risk is 0.64
       - F1 score for predicting lower risk is higher (0.78)
       - F1 score for predicting higher risk is very poor (0.02)
       - So, it shows that this is not a good model for predicting higher credit risk
       
- Undersampling

       - Precisision for predicting lower risk is higher (1.0)
       - Precisision for predicting higher risk is very poor (0.01)
       - Recall for predicting lower risk is 0.43
       - Recall for predicting higher risk is 0.60
       - F1 score for predicting lower risk is higher (0.60)
       - F1 score for predicting higher risk is very poor (0.02)
       - So, it shows that this is not a good model for predicting higher credit risk
       
 - SMOTEENN (Combination of Over and Undersampling)
       - Precisision for predicting lower risk is higher (1.0)
       - Precisision for predicting higher risk is very poor (0.01)
       - Recall for predicting lower risk is 0.53
       - Recall for predicting higher risk is 0.71
       - F1 score for predicting lower risk is higher (0.69)
       - F1 score for predicting higher risk is very poor (0.02)
       - So, it shows that this is not a good model for predicting higher credit risk
       
- Balanced Random Forest Classifier
       - Precisision for predicting lower risk is higher (1.0)
       - Precisision for predicting higher risk is very poor (0.04)
       - Recall for predicting lower risk is 0.67
       - Recall for predicting higher risk is 0.91
       - F1 score for predicting lower risk is higher (0.07)
       - F1 score for predicting higher risk is very poor (0.95)
       - So, it shows that this is not a good model for predicting higher credit risk

- Easy Ensemble AdaBoost Classifier
       - Precisision for predicting lower risk is higher (1.0)
       - Precisision for predicting higher risk is very poor (0.07)
       - Recall for predicting lower risk is 0.94
       - Recall for predicting higher risk is 0.91
       - F1 score for predicting lower risk is higher (0.97)
       - F1 score for predicting higher risk is very poor (0.14)
       - So, it shows that this is not a good model for predicting higher credit risk


**1. Randon Oversampling**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        55         |        32        |
| Low Risk (Actual)  |       5455        |      11663       |      
       
       
![ROS](/images/ROS.png)


       
**2. SMOTE Oversampling**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        53         |        34        |
| Low Risk (Actual)  |       6135        |      10983       |  

![SMOTE](/images/SMOTE.png)

**3. Undersampling**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        52         |        35        |
| Low Risk (Actual)  |       9681        |       7437       |  



![Under Sampling](/images/UNDER.png)


**4. SMOTEEN (Combination of Over and Undersampling)**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        62         |        25        |
| Low Risk (Actual)  |       8008        |       9110       |  

![SMOTEEN](/images/SMOTEEN.png)


**5. Balanced Random Forest Classifier**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        58         |        29        |
| Low Risk (Actual)  |       1560        |      15558       |  



![BRF](/images/BRF.png)

**6. Easy Ensemble AdaBoost Classifier**

|                    |  High Risk (Pred.)| Low Risk (Pred.) |
| -----------------  |:-----------------:|:----------------:|
| High Risk (Actual) |        79         |        35        |
| Low Risk (Actual)  |       979         |      16139       |  

![EEC](/images/eec.png)


## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. 

Results:
There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)

Summary:
There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
