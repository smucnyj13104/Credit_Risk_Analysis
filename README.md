# Credit_Risk_Analysis
##Overview of the analysis: Explain the purpose of this analysis.

- The purpose of this analysis was to compare the ability of various machine learning methods to predict credit risk using a credit card dataset from LendingClub using the many features available in the dataset.

##Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models.
## Use screenshots of your outputs to support your results.

### First I tried logistic regression with naive oversampling.
- The balanced accuracy score was 68%. Precision and recall for high risk were .01 and .74, respectively. Precision and recall for low risk were 1.00 and .63, respectively.

![alt text](https://github.com/smucnyj13104/Credit_Risk_Analysis/blob/main/LR_naive_oversampling.png?raw=true)

###  Next I tried logistic regression with SMOTE oversampling.
- The balanced accuracy score was 66%. Precision and recall for high risk were .01 and .64, respectively. Precision and recall for low risk were 1.00 and .67, respectively.

![alt text](https://github.com/smucnyj13104/Credit_Risk_Analysis/blob/main/LR_SMOTE_oversampling.png?raw=true)

###  Next I tried logistic regression with undersampling.
- The balanced accuracy score was 53%. Precision and recall for high risk were .01 and .67, respectively. Precision and recall for low risk were 1.00 and .40, respectively.

![alt text](https://github.com/smucnyj13104/Credit_Risk_Analysis/blob/main/LR_undersampling.png?raw=true)

###  Next I tried logistic regression with a combination of over and under sampling using the SMOTEEN algorithm.
- The balanced accuracy score was 64%. Precision and recall for high risk were .01 and .72, respectively. Precision and recall for low risk were 1.00 and .56, respectively.

![alt text](https://github.com/smucnyj13104/Credit_Risk_Analysis/blob/main/LR_combo.png?raw=true)

###  Next I tried ensemble learners, first with a balanced random forest algorithm.
- The balanced accuracy score was 72%. Precision and recall for high risk were .02 and .61, respectively. Precision and recall for low risk were 1.00 and .82, respectively.

![alt text](https://github.com/smucnyj13104/Credit_Risk_Analysis/blob/main/balancedrandomforest.png?raw=true)

###  Finally I tried easy ensemble with the AdaBoost Classifier.
- The balanced accuracy score was 74%. Precision and recall for high risk were .02 and .71, respectively. Precision and recall for low risk were 1.00 and .76, respectively.

![alt text](https://github.com/smucnyj13104/Credit_Risk_Analysis/blob/main/ensemble_Adaboost.png?raw=true)

##Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. 
##If you do not recommend any of the models, justify your reasoning.

- Overall precision was very low for high risk regardless of the method, suggesting a high number of false positives. Precision was perfect for low risk regardless of method. Recall was mediocre for all methods for high risk, with naive oversampling being the best for recall of high risk (.74) (this suggests that there were a good amount of false negatives regardless of method).  
- Based on balanced accuracy score I would recommend using the easy ensemble with the AdaBoost Classifier as this had the highest accuracy (74%).
