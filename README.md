# telco-customer-churn-analysis
Customer churn analysis using EDA and machine learning (Logistic Regression, Random Forest)
# Telco Customer Churn Analysis

## Overview
This project analyzes customer churn in a telecommunications dataset and builds machine learning models to predict which customers are likely to leave. The goal is to identify key factors driving churn and provide actionable insights to improve customer retention.

---

## Dataset
The dataset contains information on 7,043 customers, including:
- Demographics (gender, senior citizen status, dependents)
- Account details (tenure, contract type, payment method)
- Services (internet service, tech support, security features)
- Billing (monthly and total charges)

Target variable:
- **Churn** (Yes/No → converted to 1/0)

---

## Objectives
- Perform data cleaning and preprocessing
- Conduct exploratory data analysis (EDA)
- Identify key drivers of customer churn
- Build and evaluate machine learning models
- Provide business insights for retention strategies

---

## Key Insights
- Customers on **month-to-month contracts** have the highest churn
- **New customers (low tenure)** are significantly more likely to churn
- Higher **monthly charges** are associated with increased churn
- Longer-term contracts (1-year, 2-year) improve retention
- Services like **tech support and online security** reduce churn risk

---

## Models Used
- Logistic Regression
- Random Forest (with hyperparameter tuning)

---

## Model Performance
Final model: **Logistic Regression (balanced + scaled)**

- Recall (Churn): **0.79**
- AUC Score: **0.83**
- Accuracy: **0.73**

The model prioritizes identifying customers at risk of churn, making it suitable for retention-focused applications.

---

## Key Techniques
- Data cleaning and preprocessing
- One-hot encoding for categorical variables
- Feature scaling (StandardScaler)
- Handling class imbalance (class_weight='balanced')
- Model comparison and evaluation
- ROC Curve and AUC analysis
- Threshold tuning for improved recall

---

## Project Structure
telco-customer-churn-analysis/
│
├── data/
│   └── telco_customer_churn.csv
│
├── telco_customer_churn_analysis.ipynb
├── README.md
