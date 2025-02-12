# Customer Churn Prediction

## Overview

This project analyzes customer churn in a telecom dataset and builds predictive models to classify whether a customer is likely to churn. Various machine learning algorithms, including Logistic Regression, Random Forest, Support Vector Machine (SVM), AdaBoost, and XGBoost, are applied to predict churn with competitive accuracy scores.

## Dataset

The dataset used is Telco-Customer-Churn.csv, which contains customer demographic and service-related information. The target variable is Churn, where:

Yes (converted to 1) indicates the customer has churned.

No (converted to 0) indicates the customer remains with the company.

## Data Preprocessing

The following preprocessing steps are performed:

Convert TotalCharges to numeric, handling errors by coercing invalid values to NaN.

Remove missing values.

Encode categorical variables using one-hot encoding.

Normalize feature values using MinMaxScaler.

Split data into training and test sets (80%-20% for some models, 70%-30% for others).

## Exploratory Data Analysis (EDA)

Several visualizations help understand churn behavior:

Gender distribution among customers.

Churn correlation with various features.

Tenure distribution.

Contract type distribution.

Churn rate by contract type and seniority level.

Monthly and total charges distribution by churn status.

## Machine Learning Models & Performance

Several models are trained and evaluated on the dataset:

Random Forest - 80.95%

SVM - 82.02%

AdaBoost - 81.66%

XGBoost - 80.60%

### Training Process

Logistic Regression: Used as a baseline model.

Random Forest: Trained with 1000 estimators, using out-of-bag (OOB) score validation.

Support Vector Machine (SVM): Trained with a linear kernel.

AdaBoost: Boosted decision tree-based classifier.

XGBoost: Gradient boosting-based classifier.

## Key Insights

Customers on month-to-month contracts are more likely to churn.

Higher monthly charges increase churn probability.

Senior citizens tend to have a higher churn rate.

Customers with partners and dependents churn less frequently.

## Conclusion

This project effectively predicts customer churn using different machine learning techniques. SVM achieves the highest accuracy at 82.02%. The insights can help telecom businesses develop targeted retention strategies.

## Future Work

Experiment with hyperparameter tuning for improved accuracy.

Implement deep learning models for comparison.

Deploy the model using a web-based application for real-time predictions.
