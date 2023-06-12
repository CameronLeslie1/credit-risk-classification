# Module 20 Report Template

## Overview of the Analysis

Lending institutions extend loans or assets to borrowers with the expectation that they will be returned or repaid. However, there is a risk involved when borrowers fail to meet these obligations, resulting in financial losses for the lenders. To assess this credit risk, lenders employ different methods. In this analysis, we will use Machine Learning techniques to examine a dataset that consists of historical lending data from a peer-to-peer lending services company. My objective is to build a model that can accurately evaluate the creditworthiness of borrowers.

In this analysis I employed a machine learning model to analyze the loan status provided by the lender and classify the loans as either healthy or non-healthy. In order to complete this task, the data was split into training and test sets with variables defined in order to create two different regression models using both the original data set and a randomly oversampled data set. Then the performance of both models was compared.

## Results

* Machine Learning Model 1:
  * Model 1 was a Logistic Regression model that was trained on the imbalanced data set and achieved a accuracy of 87%. The model was significantly more accurate at predicting healthy loans than non-healthy loans.

* Machine Learning Model 2:
  * This model is another Logistic Regression Model but fitted with balanced, or oversampled, data. The model achieved a perfect prediction rate of 100% for healthy loans and an 84% prediction rate for non-healthy loans. Based on the recall scores, it had a 1% error rate in predicting both healthy loans and non-healthy loans. The balanced dataset had a accuracy score of 99%.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* The Logistic Regression model trained on the oversampled data outperformed the model trained on the imbalanced data. The balanced dataset led to a higher accuracy score an an improved recall which indicates the model's ability to reduce errors when classifying non-healthy loans.
* The inbalanced data model had 80 instances of False Positives, where the actual value was healthy but the model predicted value was unhealthy. There were 67 instances classified as False Negatives where the actual value was non-healthy but the model predicted the value was healthy.
* In contrast, the model fitted with balanced data only had 2 instances classified as False Positives and 91 instances were classified as False Negatives.
* Given the value at risk of a False Negative vs a False Positive for a Lender, we would prefer a lower number of False Positives.
* Based on the analyses, there is a significant reduction in the number of False positives in the second machine learning model. Therefore, I would recommend utilizing Model 2 over Model 1, however this should not be the full extent of the analysis a Lender conducts as there are likely hidden biases and additional variables to consider when analyzing a loan's credit quality.

