# credit_risk_resampling report

## Overview of the Analysis

Need to analyze historical data to build a model that predicts the credit worthiness of borrowers. The ultimate goal is to build a model that is not only accurate at predicting healthy loans but also accurate in predicting high-risk loans. Because there are far fewer high-risk loans the model needs to account for this imbalance. 

The data we analyzed included the loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total debt. Out of the historical data we analyzed there were 77,536 total loans, form which only 2,500 were high-risk. Because the data was imbalanced we ran the historical data through an 'over sampler' function that creates equal weighting for our next steps of modeling. We then ran logistic regression over the original data set and the balanced data set so we can compare which model has better results.

## Results

* Machine Learning Model 1 (Original Data):

Accuracy:  .952
Precision: .99
Recall:    .99

** High-Risk
Precision: .85
Recall:    .91


* Machine Learning Model 2 (Balanced Data):

Accuracy:  .994
Precision: .99
Recall:    .99

** High-Risk
Precision: .84
Recall:    .99

## Summary

Both models perform very well overall. Depending on the outcomes and purpose of the predictive model you would chose one over the other. If your goal is to find and predict all high-risk loans, and are comfortable with some healthy loans being flagged as high-risk then you should use the balanced model (model 2). If your goal is to limit that amount of healthy loans that are flagged as high-risk then you should chose the original model (model 1).

