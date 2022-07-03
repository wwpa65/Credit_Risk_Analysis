# Credit_Risk_Analysis


The report should contain the following:
## Overview of the analysis: Explain the purpose of this analysis.

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. 

Use screenshots of your outputs to support your results.


**Randon Oversampling**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 53 | 34 |
| Low Risk (Actual)   | 5335      |   11783 |      
       
       
**SMOTE Oversampling**     
  
 
|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 51 | 36 |
| Low Risk (Actual)   | 6605      |   11053 |


**Under sampling**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 52 | 35|
| Low Risk (Actual)   | 9681      |   7437 |


**SMOTENN (Combination of Over and Undersampling)**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 61 | 26 |
| Low Risk (Actual)   | 7839      |   9279 |

**Balanced Random Forest Classifier**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 58 | 29 |
| Low Risk (Actual)   | 1560     |   15558 |

**Easy Ensemble AdaBoost Classifier**

|               |  High Risk (Pred.)          | Low Risk (Pred.)  |
| ------------- |:-------------:| -----:|
| High Risk (Actual)     | 79 | 8 |
| Low Risk (Actual)   | 979      |   16139 |


## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. 

If you do not recommend any of the models, justify your reasoning.

Overview of the loan prediction risk analysis:
The purpose of this analysis is well defined (4 pt)

Results:
There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)

Summary:
There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
