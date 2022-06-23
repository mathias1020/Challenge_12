# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis was to build a model that is capable of accurately classifying the creditworthiness of a potential borrower based on historical data.  Standard loan data was used as the input for the analysis including: loan amount, interest rate, income, debt, and derogatory credit history.  The output of the model was binary, either the borrower was categorized as creditworthy or high-risk.  The challenge in the data is striking the right balance to be sensitive enough to correctly identify high risk loans, but not so sensitive that healthy loans are declined costing the company revenue.  Additionally, because most loans are healthy, there is an imbalance in the data that could bias the model.  To counter this, two models were trained.  One model with the original data, and one model with resampled data to address the imbalance.  

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Accuracy - 95.2%
  * Precision: 
      * Healthy - 99.7%
      * High Risk - 84.7%
  * Recall:
      * Healthy Loans - 99.5%
      * High Risk Loans - 90.9%

* Machine Learning Model 2:
   * Accuracy -  99.4%
   * Precision: 
      * Healthy - 99.98%
      * High Risk - 84.1%
   * Recall:
      * Healthy Loans - 99.4%
      * High Risk Loans: - 99.4%

## Summary

My recommendation is to use model 2 with resampled data.  The reason is that it strikes a healthy balance with regard to sensitivity to detecting high risk loans.  While the model did incorrectly identify an additional 14 loans as high risk, representing lost revenue to the company, it correctly identified an additional 52 loans as being high risk.  The assumption to my recommendation is that the the opportunity cost of the lost loans is more than offset by being able to accurately price or decline the additional 52 high risk loans in this analysis.  