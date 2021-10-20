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
    
    The RandomOverSampler algorithm demonstrates a significantly low level of precision for identifying high risk individuals with a score of .01.  It does, however, demonstrate a high level of precision for low risk with a score of 1.  The sensitivity level for both high and low risk and relatively similar with scores of .67 and .64 respectively, meaning that it has a moderate level of potential for missing or misidentifying credit levels for both categories.  

*  SMOTE:
    *  Balanced Accuracy Score:
    
    ![SMOTE balanced accuracy score](https://user-images.githubusercontent.com/85641017/138129475-56ad3556-7405-4540-b37c-cdd63c5fa68d.png)

    This graphic shows that the SMOTE algorithm produced an accuracy score of approximately .63, meaning that it is accurate approximately 65% of the time.
    
    *  Precision and Recall Score:
    
    ![SMOTE precision and recall scores](https://user-images.githubusercontent.com/85641017/138129657-adb96976-caad-4d57-b00d-df28e8bcc346.png)

    The SMOTE algorithm demonstrates a significantly low level of precision for identifying high risk individuals with a score of .01.  It does, however, demonstrates a high level of precision for low risk with a score of 1.  The sensitivity level for both high and low risk and relatively similar with scores of .61 and .64 respectively, meaning that it has a moderate level of potential for missing or misidentifying credit levels for both categories.
    
*  ClusterCentroids:
    *  Balanced Accuracy Score:
    
    ![Centroids balanced accuracy score](https://user-images.githubusercontent.com/85641017/138129930-b2ba2ba2-3dcc-4f0a-b762-a7623468764c.png)

    This graphic shows that the ClusterCentroids algorithm produced an accuracy score of approximately .51, meaning that it is accuracy approximately 51% of the time.
   
    *  Precision and Recall Score:
    
    ![Centroids precision and recall scores](https://user-images.githubusercontent.com/85641017/138130062-2abdbcfc-6f4f-4af0-b2f9-4a3f428b07ad.png)

    The ClusterCentroids algorithm demonstrates a significantly low level of precision for identifying high risk individuals with a score of .01.  It does, however, demonstrate a high level of precision for low risk with a score of 1.  The sensitivity level for high risk is moderate with a score of .59, but low for low risk with a score of .43.
    
*  SMOTEENN
    *  Balanced Accuracy Score:
    
    ![SMOTEENN balanced accuracy score](https://user-images.githubusercontent.com/85641017/138130208-d54763eb-d006-48a1-9204-96fd4ee28f63.png)

    This graphic shows that the SMOTEENN alorgirthm produced an accuracy score of approximatle .63, meaning that it is accurate approximately 63% of the time.
    
    *  Precision and Recall Score:
    
    ![SMOTEENN precision and recall scores](https://user-images.githubusercontent.com/85641017/138130358-af023d11-f48e-4413-a427-d2f593439b49.png)

    The SMOTEENN algorithm demonstrates a significantly low level of precision for identifying high risk individuals with a score of .01.  It does, however, demonstrate a high level of precision for low risk with a score of 1.  The sensitivity level for both high and low risk and relatively similar with scores of .68 and .58 respectively, meaning that it has a moderate level of potential for missing or misidentifying credit levels for both categories.
    
 
*  BalancedRandomForestClassifier
    *  Balanced Accuracy Score:
    
    ![ForestClassifier balanced accuracy score](https://user-images.githubusercontent.com/85641017/138130556-7b3692d5-eac8-4a3a-a0dd-ddf14bfbc195.png)

    This graphic shows that the BalancedRandomForestClassifier algorithm produced an accuracy score of approximately .79, meaning that it is accurate approximately 79% of the time.
    
    *  Precision and Recall Score:
    
    ![ForestClassifier precision and recall scores](https://user-images.githubusercontent.com/85641017/138130718-29f030f1-56d5-4456-99bf-5c04936a25f6.png)

    The BalancedRandomForestClassifier algorithm demonstrates a significantly low level of precision for identifying high risk individuals with a score of .04.  It does, however, demonstrate a high level of precision for low risk with a score of 1.  The sensitivity level for high credit risk is on the higher end of moderate with a score of .67.  It has an extremely high sensitivity level for identifying low risk with a score of .91.
    
*  EasyEnsembleClassifier:
    *  Balanced Accuracy Score:
    
    ![EasyEnsemble balanced accuracy score](https://user-images.githubusercontent.com/85641017/138130926-35e1e2b1-54b8-4ad8-bb32-88e7029aa013.png)

    This graphic shows that the EasyEnsembleClassifier algorithm produced an accuracy score of approximately .93, meaning that it is accurate approximately 93% of the time.
    
    *  Precision and Recall Score:
    
    ![EasyEnsemble precision and recall scores](https://user-images.githubusercontent.com/85641017/138131095-381d0c1b-5012-4ef6-9859-2f7bd1a2c010.png)

    The EasyEnsembleClassifier algorithm demonstrates a significantly low level of precision for identifying high risk individuals with a score of .07.  It does, however, demonstrate a high level of precision for low risk with a score of 1.  The sensitivity level for both high and low risk are very high with scores of .94 and .91, respectively, indicating a high degree of identifying both categories.
    
##  Summary of Results
After running all six of the identified predictive algorithms, one of the first observations that becomes immediately apparent is that there is a low precision potential for correctly identifying true positive for high credit risk.  The most significant, in that regard, is the EasyEnsembleClassification model.  All models show the same predictive score for low risk meaning that for those that are identified as low risk, they are more likely to be truly low risk.  However, another significant concern identified for all models is the level of relative sensitivity with 5 of the six models demonstrating a sensitivity score of less than .70.  The one exception to this would be the EasyEnsembleClassifier model which shows sensitivity rates of .94 and .91 for high and low risk respectively.  This indicates a much higher potential for catching both high and low risk; accurately doing so between 91-94% of the time.  Since we are considering credit risk and the potential financial impact on a lender, it is important to not only identify the low risk individuals, those that will be a "good customer" for lending and will repay loans as dictated, but also to accurately identify the high risk individuals, those that represent a potential negative financial impact on the lender.  After reviewing all six of the given mdoels, the EasyEnsembleClassifier model presents with consistent levels of precision, but more importantly, extremely high levels of sensitivity, something that the other models are lacking.  Based on this observation, the EasyEnsembleClassifier model is the best option for predicting credit risk.
