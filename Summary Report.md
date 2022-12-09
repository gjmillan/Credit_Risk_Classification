## Credit Risk Analysis Report

# Purpose of Analysis

With historical lending data, the goal is to build a logistical regression model, using python and its libraries, in order to properly predict the status of the loan.

This is done by classifying the status of the loan into two categories:
  1. Healthy Loan - Referred to in the data as "0".
  2. High-Risk Loan - Referred to in the data as "1".
  * This data classification is found under the "loan_status" section of the data.
  
With this data in hand, we wanted to also the capability to predict the status of the loans by randomazing and resampling the data to test and generate results with better predictions.
As you will see through the model, this was done with Random Over Sampler, Logistic Regression, and Confusion Matrix.

There are two key stages in this model where Machine Learning was applied.
The first stage is the classification model where Logistic Regression was applied. This was used to train the model with the original data.
The second stage is the prediction model, where the Predict function was used in order to generate the predictions which was then used to evaluate the model vs. the original.
The key methods used in order to perform this analysis were: 
  * sklearn.linear_model.LogisticRegression 
  * imblearn.over_sampling.RandomOverSampler
  
# Results of Analysis

With the two models of Machine Learning noted above the resuts of the analysis are as follow:

* Model 1: Machine Learning
 * Balanced Accuracy Score: 0.9520479254722232 or 95% accuracy
 * 0/Healthy Loans:
        * Precision Score: 1.00/100% precision
        * Recall Score: 0.99/99% recall
 * 1/High-Risk Loans:
        * Precision Score: 0.85 or 85% precision
        * Recall Score: 0.91 or 91% recall
        
* Model 2: Machine Learning
 * Balanced Accuracy Score: 0.99/99% accuracy
 * 0/Healthy Loans:
        * Precision Score: 1.00/100% precision
        * Recall Score: 0.99/99% recall
 * 1/High-Risk Loans:
        * Precision Score: 0.85/85% precision
        * Recall Score: 0.99/99% recall

# Summary of Analysis
Based on the analysis and results of the models, we can conclude that the performance of models and data returned a high level of accuracy for Healthy and High-Risk Loans. In a worse case scenario, the model is able to predict the status of the loan at an 85% accuracy or above.
