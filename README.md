# Credit Risk Analysis Report

## Overview of Analysis 
Credit risk presents a significant problem for all portions of the financial services industry (banks, financial management companies, credit card companies, etc) and it is important to develop as clear and concise of an evaluation of risk as possible.  In this particular analysis, we take a dataset of loan status performance (Loan_Status2019Q1.csv) that was provided by LendingClub in order to establish machine learning that will be able to assist with making reliable predictions with regards to credit risk.  Multiple algorithms obtained from Python libraries in order to determine/predict credit risk including RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.  For each algorithm, the Balanced Accuracy, Precision, and Recall Scores were calculated to show a representation of accuracy of prediction for the given algorithm.  Balanced accuracy scores are a calculated average  of the proportion of correct predictions for the dataset.  It is measured on a scale between 0 and 1, with 1 being complete accuracy.  The precision score is the ratio of correctly predicted positive observations to the total predicted positives (TP/(TP+FP)).  The recall score is the number of true positive divided by the total number of true positives and false negatives (TP/(TP+FN)).  



###  Resources:
*  Data: 
    *  Credit card credit dataset obtained from LendingClub (a peer-to-peer lending services company)
    *  LoanStatus_2019Q1.csv
*  Software:
    *  Jupyter Notebook, Python

##  Results of Analysis
(Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.)
*  RandomOverSampler:
    *  Balanced Accuracy Score:
    
    ![ROS balanced accuracy score](https://user-images.githubusercontent.com/85641017/138126120-6a8be898-17a8-4d81-8de7-8e75953adb4c.png)
    
    This graphic shows that the RandomOverSampler algorithm produced an accuracy score of approximately .65, meaning that it is accurate approximately 65% of the time.

    *  Precision and Recall Score:
    
    ![ROS precision and recall scores](https://user-images.githubusercontent.com/85641017/138126334-a0efb4be-1216-431a-83b3-295a80fa1c28.png)
    
    This graphic shows that the RandomOverSampler algorithm produced a precision score of .01 and a recall score of .67 for high risk and a precision score of 1.0 and recall score of .64 for low risk.  

*  SMOTE:
    *  Balanced Accuracy Score:
    
    ![SMOTE balanced accuracy score](https://user-images.githubusercontent.com/85641017/138129475-56ad3556-7405-4540-b37c-cdd63c5fa68d.png)

    This graphic shows that the SMOTE algorithm produced an accuracy score of approximately .63, meaning that it is accurate approximately 65% of the time.
    
    *  Precision and Recall Score:
    
    ![SMOTE precision and recall scores](https://user-images.githubusercontent.com/85641017/138129657-adb96976-caad-4d57-b00d-df28e8bcc346.png)

    This graphic shows that the SMOTE algorithm produced a precision score of .01 and a recall score of .61 for high risk and a precision score of 1.0 and recall score of .64 for low risk.
    
*  ClusterCentroids:
    *  Balanced Accuracy Score:
    
    ![Centroids balanced accuracy score](https://user-images.githubusercontent.com/85641017/138129930-b2ba2ba2-3dcc-4f0a-b762-a7623468764c.png)

    This graphic shows that the ClusterCentroids algorithm produced an accuracy score of approximately .51, meaning that it is accuracy approximately 51% of the time.
   
    *  Precision and Recall Score:
    
    ![Centroids precision and recall scores](https://user-images.githubusercontent.com/85641017/138130062-2abdbcfc-6f4f-4af0-b2f9-4a3f428b07ad.png)

    This graphic shows that the ClusterCentroids algorithm produced a precision score of .01 and a recall score of .59 for high risk and a precision score of 1 and a recall score of .43 for low risk.
    
*  SMOTEENN
    *  Balanced Accuracy Score:
    
    ![SMOTEENN balanced accuracy score](https://user-images.githubusercontent.com/85641017/138130208-d54763eb-d006-48a1-9204-96fd4ee28f63.png)

    This graphic shows that the SMOTEENN alorgirthm produced an accuracy score of approximatle .63, meaning that it is accurate approximately 63% of the time.
    
    *  Precision and Recall Score:
    
    ![SMOTEENN precision and recall scores](https://user-images.githubusercontent.com/85641017/138130358-af023d11-f48e-4413-a427-d2f593439b49.png)

    This graphic shows that the SMOTEEN algorithm produced a precision score of .01 and a recall score of .68 for high risk and a precision score of 1 and a recall score of .58 for low risk.
    
   *  Conclusions for Risk Resamplers:
   For the risk resampler algorithms, there appears to be a significant level of similarity with regards to the accuracy of the given algorithms with accuracies between .63 and .65.  The exception to this is the ClusterCentroids algorithm which shows an accuracy score of only approximately .51.  The precision scores for all 4 algorithms are virtually identical with scores of .01 for identifying high risk and 1 for identifying low risk.  This would indicate that these algorithms are all extremely strong with correctly identifying low risk, but struggle with correctly identifying high risk.  
*  BalancedRandomForestClassifier
    *  Balanced Accuracy Score:
    
    ![ForestClassifier balanced accuracy score](https://user-images.githubusercontent.com/85641017/138130556-7b3692d5-eac8-4a3a-a0dd-ddf14bfbc195.png)

    This graphic shows that the BalancedRandomForestClassifier algorithm produced an accuracy score of approximately .79, meaning that it is accurate approximately 79% of the time.
    
    *  Precision and Recall Score:
    
    ![ForestClassifier precision and recall scores](https://user-images.githubusercontent.com/85641017/138130718-29f030f1-56d5-4456-99bf-5c04936a25f6.png)

    This graphic shows that the BalancedRandomForestClassifier algorithm produced a precision score of approximately .04 and a recall score of .67 for high risk and a precision score of 1 and a recall score of .91 for low risk.
    
*  EasyEnsembleClassifier:
    *  Balanced Accuracy Score:
    
    ![EasyEnsemble balanced accuracy score](https://user-images.githubusercontent.com/85641017/138130926-35e1e2b1-54b8-4ad8-bb32-88e7029aa013.png)

    This graphic shows that the EasyEnsembleClassifier algorithm produced an accuracy score of approximately .93, meaning that it is accurate approximately 93% of the time.
    
    *  Precision and Recall Score:
    
    ![EasyEnsemble precision and recall scores](https://user-images.githubusercontent.com/85641017/138131095-381d0c1b-5012-4ef6-9859-2f7bd1a2c010.png)

    This graphic shows that the EasyEnsembleClassifier algorithm produced a precision score of .07 and a recall score of .91 for high risk and a precision score of 1 and a recall score of .94 for low risk.
    
##  Summary of Results
