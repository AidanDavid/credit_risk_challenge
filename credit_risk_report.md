
# Credit Risk Analysis Report

## Overview of the Analysis

This analysis seeks to judge the accuracy and reliability of a logistic regression model in regards to predicting credit risk.

The dataset contains financial information about loans. With this data, the logistic regression model could predict whether a loan is at high risk of defaulting (loan_status = 1) or is healthy (loan_status = 0).

the machine learning process is as follows:

- Load and pre-process the data.
- Split the data into training and testing sets.
- Train a logistic regression model.
- Evaluate the model using accuracy, precision, recall, and a confusion matrix.

## Results

- **Accuracy Score:** High: 0.99. Thus, an overall strong performance.
- **Precision Score:**
  - High for healthy loans (0): 1.00, Thus, most predicted healthy loans are correct.
  - Lower for high-risk loans (1): 0.89. Thus, some predicted high-risk loans are actually healthy.
- **Recall Score:**
  - High for healthy loans (0): 1.00. Thus, most actual healthy loans are correctly identified.
  - Lower for high-risk loans (1): 0.93 Thus, some high-risk loans are missed.

### Confusion Matrix

The confusion matrix shows that the model correctly predicts most healthy loans but misses some actual high-risk loans, leading to false negatives.

## Summary

The logistic regression model performs well in predicting healthy loans (0), but has lower recall for high-risk loans (1). This means the model may fail to detect some high-risk loans. Thus, financial institutions making use of this model should consider the risk of failures regarding loan defaults.

- If overall accuracy and precision are the priority, the model is likely reliable.  
- However, if identifying high-risk loans is critical, improvements are needed to more accurately judge such risks.  

This model is useful for credit risk analysis, but requires improved recall for true reliability regarding high-risk loans.
