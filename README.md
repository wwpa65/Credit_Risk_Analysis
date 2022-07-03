# Credit_Risk_Analysis

## Overview:


ill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.



## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. 

Use screenshots of your outputs to support your results.


**1. Randon Oversampling**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 55 | 32 |
| Low Risk (Actual)   | 5455      |   11663 |      
       
       
![ROS](/images/ROS.png)


       
**SMOTE Oversampling**   
  
|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 53 | 34 |
| Low Risk (Actual)   | 6135      |   10983 |


![SMOTE](/images/SMOTE.png)

**Under sampling**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 52 | 35|
| Low Risk (Actual)   | 9681      |   7437 |

![Under Sampling](/images/UNDER.png)


**SMOTEEN (Combination of Over and Undersampling)**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 62 | 25 |
| Low Risk (Actual)   | 8008      |   9110 |

![SMOTEEN](/images/SMOTEEN.png)


**Balanced Random Forest Classifier**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 58 | 29 |
| Low Risk (Actual)   | 1560     |   15558 |

![BRF](/images/BRF.png)

**Easy Ensemble AdaBoost Classifier**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 79 | 8 |
| Low Risk (Actual)   | 979      |   16139 |

![EEC](/images/eec.png)


## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. 

If you do not recommend any of the models, justify your reasoning.

Overview of the loan prediction risk analysis:
The purpose of this analysis is well defined (4 pt)

Results:
There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)

Summary:
There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
