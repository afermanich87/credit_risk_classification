# credit_risk_classification

## Intro
In this Challenge, various techniques were used to train and evaluate a model based on loan risk. A dataset of historical lending activity was used to build a model that can identify the creditworthiness of borrowers. In the following analysis, machine learning was used for the credit risk model. 


## An overview of the analysis: 

The data for this analysis was loaded from the `lending_data.csv`. The variable `y` was set to the "loan_status", which was classified as either 0 or 1. 
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting. All other remaining columns in this data were set to the `X` variable. The data was first analyzed using the Logistic Regression technique. Then the resampled data was analyzed second. 

## The results: 

Logistic Regression Model (original data)
  * Accuracy score: ~ 0.95
  * Precision score: 0 = 1.00 and 1 = 0.85
  * Recall score: 0 = 0.99 and 1 = 0.91

Logistic Regression Model with Resampled Data
  * Accuracy score: ~ 0.99
  * Precision score: 0 = 1.00 and 1 = 0.84
  * Recall score: 0 = 0.99 and 1 = 0.99

## A summary: 

For precision, the resampled data and original logistic regression were good at predicting healthy loans (1.0) and less accurate at predicting high-risk loans (0.85 vs 0.84).

For recall, the original data showed a less accurate prediction for high-risk loans when compared to the resampled data that shows an increase from 0.91 to 0.99. This supports the conclusion that the resampled data had a higher accuracy than the original data for high-risk loans. 

The total credit risk classification is imbalanced due to the nature of the business. There are fewer high-risk loans compared to healthy loans. The total number of healthy loans in this data is 75036, while the total number of high-risk loans is 2500. Given that the precision score was lower for the high-risk loans, this model using logistic regression would not be a good model to use. I do not recommend using this model as you would want to see the precision score for high-risk loans be higher than 0.85 and 0.84 respectively. 

Since the high-risk loans are of more concern to the lender, this is the number that you would want to see be as close to 1 as possible. 


## Conclusion

Received help from TA's during office hours. Used the activites from module 20 as a guide for setting up my train and test prediction models. 
Our instructor provided more information on resampling data as well. 




