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

### Gender distribution among customers.
![image](https://github.com/user-attachments/assets/d5b082a0-79ee-4727-84a8-49128c0f1b35)


### Churn correlation with various features.
![image](https://github.com/user-attachments/assets/2ec50b56-3821-49a5-b03e-99d88f3277f6)
![image](https://github.com/user-attachments/assets/56f9aa18-bedb-4a8f-a5bb-6a61c96c0c37)

### Tenure distribution.
![image](https://github.com/user-attachments/assets/bbbdd0c1-7a28-4855-b394-f8cd4f8840d7)
![image](https://github.com/user-attachments/assets/219777f9-26b8-4e43-b573-f399b15e0f12)

![image](https://github.com/user-attachments/assets/23846170-f718-4234-bd99-74353ab2aa29)
![image](https://github.com/user-attachments/assets/c214354c-210c-4055-983c-86c165c5bdda)



### Contract type distribution.

![image](https://github.com/user-attachments/assets/aea58ce2-9011-477e-8773-af245d120ca1)
![image](https://github.com/user-attachments/assets/2a38cc8a-937b-4e05-b909-9c2061357ccc)


### Churn rate by contract type and seniority level.
![image](https://github.com/user-attachments/assets/38ed2785-bc17-4267-b0de-941d08f233c5)
![image](https://github.com/user-attachments/assets/9d516cf0-2dca-4216-a346-4d73c9c7d594)
![image](https://github.com/user-attachments/assets/658e32ad-30fc-48d1-80d7-f6b4f4e98f2f)
![image](https://github.com/user-attachments/assets/f276adc5-dc19-4f76-a5c2-9306cfff43fe)



### Monthly and total charges distribution by churn status.
![image](https://github.com/user-attachments/assets/0d52b33b-0b21-4882-bd67-e302da55a13f)
![image](https://github.com/user-attachments/assets/2d890899-053c-49f5-b573-9411d8a24ad5)


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
