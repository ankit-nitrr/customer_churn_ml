# Customer Churn Prediction using Machine Learning

## Overview

Customer churn is one of the most critical challenges faced by subscription-based businesses. Acquiring a new customer is often more expensive than retaining an existing one. This project focuses on predicting whether a customer is likely to leave a telecom service provider based on demographic information, account details, and service usage patterns.

Using the IBM Telco Customer Churn dataset, exploratory data analysis (EDA), feature engineering, and machine learning techniques were applied to identify churn patterns and build predictive models.

---

## Problem Statement

The objective of this project is to develop a machine learning model capable of predicting customer churn.

The model helps businesses:

* Identify customers at risk of leaving.
* Improve customer retention strategies.
* Reduce revenue loss.
* Support data-driven business decisions.

---

## Dataset

Dataset: IBM Telco Customer Churn Dataset

### Dataset Information

* Total Customers: 7,043
* Features: 20+
* Target Variable: Churn
* Type: Binary Classification Problem

### Target Classes

* Yes → Customer Churned
* No → Customer Retained

---

## Project Workflow

### 1. Data Collection

The customer churn dataset was loaded and inspected for:

* Missing values
* Data types
* Feature distributions
* Class imbalance

---

### 2. Exploratory Data Analysis (EDA)

Several analyses were performed to understand customer behavior.

Key observations:

* Customers with shorter tenure showed higher churn rates.
* Customers with month-to-month contracts were more likely to churn.
* Higher monthly charges were associated with increased churn.
* Class distribution was imbalanced, requiring special handling during model training.

Visualizations included:

* Churn distribution
* Contract type analysis
* Tenure analysis
* Monthly charges distribution
* Correlation and feature exploration

---

### 3. Data Preprocessing

The following preprocessing steps were performed:

* Removal of unnecessary columns
* Handling categorical variables
* Feature encoding
* Train-test splitting
* Class imbalance treatment using SMOTE-ENN

Techniques Used:

* Label Encoding
* Data Cleaning
* Feature Transformation
* SMOTEENN Resampling

---

### 4. Model Building

Machine learning models were trained to classify customer churn.

Algorithms Used:

#### Decision Tree Classifier

* Criterion: Gini Index
* Max Depth: 6
* Minimum Samples Leaf: 8

#### Decision Tree with SMOTEENN

To improve performance on the imbalanced dataset, SMOTEENN was applied before model training.

Benefits:

* Better minority class learning
* Improved recall
* Reduced bias toward majority class

---

## Evaluation Metrics

Since churn prediction is an imbalanced classification problem, accuracy alone is not a reliable metric.

The following metrics were used:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

Special focus was placed on Recall and F1-Score because correctly identifying churned customers is more important than maximizing overall accuracy.

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Imbalanced-Learn

### Machine Learning

* Decision Tree Classifier
* SMOTEENN Resampling

---

## Project Structure

├── Churn Analysis - EDA.ipynb
├── Churn Analysis - Model Building.ipynb
├── model.sav
├── dataset.csv
├── README.md

---

## Business Impact

The developed churn prediction system can help telecom companies:

* Detect customers likely to leave.
* Prioritize retention campaigns.
* Improve customer satisfaction.
* Reduce customer acquisition costs.
* Increase long-term profitability.

---

## Future Improvements

Potential enhancements include:

* Random Forest Classifier
* XGBoost
* LightGBM
* Hyperparameter Tuning
* Feature Selection
* Model Deployment using Streamlit
* Real-time churn prediction dashboard

---

## Conclusion

This project demonstrates the complete machine learning lifecycle, including data analysis, preprocessing, handling class imbalance, model development, and performance evaluation. The resulting model provides valuable insights into customer behavior and serves as a foundation for predictive retention strategies in the telecom industry.
