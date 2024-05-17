# CreditCard_FraudDetection
A Machine learning predictive model for identifying fraudlent transactions

## Overview
In today's digital landscape, financial institutions face significant challenges in mitigating fraudulent activities. The rise of online transactions and electronic payments has increased the complexity and frequency of fraudulent behavior. Detecting and preventing fraudulent transactions is crucial to safeguarding both the institution's assets and maintaining customer trust.
The project purpose is to build a machine learning model for predicting and identifying fraudlent transactions.
Three models were trained which are:

- RandomForest.
- XGBOOST.
- Deep learning model.

the champion model was XGBOOST with F1-score 0.991 on the validation set , and 0.972 on the testing set.

## Business Understanding

Guardian Banking Systems , a leading financial institution committed to providing secure and reliable services to its customers. The primary goal is to leverage machine learning techniques to develop an effective fraud detection system that can identify potentially fraudulent transactions in real-time.

The objective of this project is to build a robust machine learning model capable of detecting fraudulent transactions accurately and efficiently. The model will analyze historical transaction data to identify patterns and indicators associated with fraudulent behavior

## Data Understanding

The Credit Card Transactions Fraud Detection Dataset from kaggle by KARTIK SHENOY consisted of 1,852,394 rows and 23 features(Before Feature Engineering). The features included information on customers trips such as:

- trans_date_trans_time -----> transaction date and time
- merchant -----> merchant at which the transaction occured
- category -----> which category the transaction related to (home , shopping , travel etc.)               
- amt -----> the transaction ammount
- gender ------> person gender
- dob -------> person date of birth
- is_fraud -----> Target variable
and more

## Modeling and Evaluation

We trained three models which are:

- RandomForest.
- XGBOOST.
- Deep learning model.
  
Cross Validation technique was applied , the dataset was splitted to 70% for training , 15% for validation and 15% for unseen testing data which will be used to evaluate our champion model.

considering accuracy measures , for each model , we output a confusion matrix and four accuracy measures , they are

- Accuracy
- Precision
- Recall
- F1 Score
Considering the given Scenario:

False positives: A false positive occurs when the model incorrectly predicts a transaction as fraudulent when it is actually legitimate..
False negatives: A false negative occurs when the model fails to detect a fraudulent transaction and predicts it as legitimate.

False positives can lead to inconvenience for customers if legitimate transactions are flagged as fraudulent. This may result in declined transactions, customer dissatisfaction, and potential loss of business, The cost associated with false positives includes potential customer attrition, increased customer service inquiries, and missed revenue opportunities.

False negatives can be more detrimental as they allow fraudulent activities to go undetected, potentially leading to financial losses for the institution and erosion of customer trust, The cost associated with false negatives includes financial losses due to fraudulent transactions, regulatory penalties, and reputational damage.

Both False positive and False Negative costs are high , so we will evaluate the model based on a balance between both of them , which is F1-score

The champion model was XGBOOST with F1-score 0.991 on the validation set.

The model Scored 0.972 on the unseen testing set which is great.

## Conclusion
- model conclusions
  RandomForest ,  XGBOOST and Deep learning were used for modeling , however XGBOOST scored higher than RandomForest and Deep learning model on the validation set.
  XGBOOST scored really well on the unseen test set with f1-score 0.972 , so we might be confident in applying and deploying this model in fraud detection , however we may work on other feature engineering and tuning tasks to increase the model performance later on , but for now , it's great.

- Project conclusions:
  Increase fraud detection systems in online shopping and grocery stores
  verify persons holding credit cards before performing transactions , specially middle aged persons.
  keep an eye on small transactions , as most of fraudlent transactions come from small amounts
  
   




