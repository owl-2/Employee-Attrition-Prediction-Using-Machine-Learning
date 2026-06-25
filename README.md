##Employee Attrition Prediction Using Machine Learning

## Overview

Employee attrition is a major challenge for organizations, leading to increased recruitment costs, productivity loss, and disruption of business operations. Identifying employees who are at risk of leaving can help organizations implement proactive retention strategies.

This project develops a machine learning model to predict employee attrition using workforce, performance, and engagement-related data. The objective is to help HR teams identify high-risk employees and support data-driven retention initiatives.

---

## Business Problem

Employee turnover can significantly impact organizational performance and operational costs.

The challenge is to identify patterns associated with employee exits and develop a predictive system that can estimate the likelihood of attrition before employees leave.

### Business Objectives

* Predict employee attrition risk
* Identify key factors driving employee turnover
* Enable proactive retention strategies
* Reduce hiring and training costs
* Improve workforce planning and talent management

---

## Dataset

The dataset contains employee-related information including performance metrics, work history, satisfaction scores, and compensation data.

### Features

#### Employee Engagement

* Satisfaction Level
* Last Evaluation Score

#### Workload & Performance

* Number of Projects
* Average Monthly Hours

#### Employment History

* Years at Company
* Work Accident History
* Promotion in Last 5 Years

#### Organizational Information

* Department
* Salary Category

### Target Variable

**Employee Attrition (left)**

* 1 = Employee Left the Organization
* 0 = Employee Remained in the Organization

---

## Exploratory Data Analysis

Exploratory analysis was performed to understand workforce characteristics and attrition patterns.

Key areas investigated:

* Employee satisfaction distribution
* Attrition across salary categories
* Impact of workload on employee retention
* Relationship between tenure and attrition
* Department-wise attrition trends
* Promotion and retention analysis

---

## Data Preprocessing

### Data Quality Checks

* Missing value assessment
* Duplicate record identification
* Outlier detection using IQR methodology

### Feature Engineering

* Binary feature handling
* One-Hot Encoding of categorical variables
* Feature scaling using MinMaxScaler
* Train-Test Split with Stratification

### Class Imbalance Handling

Employee attrition datasets often contain class imbalance, making standard accuracy insufficient for model evaluation.

Class imbalance was addressed during model training to improve minority-class prediction performance.

---

## Machine Learning Approach

### Algorithm

**Random Forest Classifier**

Reasons for selection:

* Handles non-linear relationships effectively
* Robust against overfitting
* Suitable for mixed feature types
* Performs well on tabular business datasets
* Provides interpretable feature importance scores

### Hyperparameter Optimization

RandomizedSearchCV was used with 5-fold cross-validation to identify optimal model parameters.

Optimization Metric:

* ROC-AUC Score

---

## Model Evaluation

Model performance was assessed using:

* ROC-AUC
* Confusion Matrix
* Precision
* Recall
* F1 Score
* Cross Validation

### Why ROC-AUC?

ROC-AUC measures the model's ability to distinguish between employees who leave and those who stay across multiple classification thresholds.

This metric is particularly useful for imbalanced classification problems where prediction ranking is more important than overall accuracy.

---

## Project Workflow

Employee Data
       ↓
Data Cleaning
       ↓
Exploratory Data Analysis
       ↓
Feature Encoding
       ↓
Outlier Detection
       ↓
Feature Scaling
       ↓
Train-Test Split
       ↓
Random Forest Model
       ↓
Hyperparameter Optimization
       ↓
Model Evaluation
       ↓
Attrition Risk Prediction
```


## Business Insights

The model can support HR and People Analytics teams by:

* Identifying employees at high risk of attrition
* Improving workforce retention strategies
* Supporting evidence-based HR decisions
* Reducing recruitment and onboarding costs
* Enhancing employee engagement initiatives

Instead of reacting after employees resign, organizations can proactively intervene with targeted retention programs.

---

## Technical Stack

### Programming

* Python

### Data Analysis

* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn

### Machine Learning

* Scikit-Learn

### Model Selection

* RandomizedSearchCV
* Cross Validation

---

## Key Skills Demonstrated

* Exploratory Data Analysis (EDA)
* Data Cleaning & Preprocessing
* Outlier Detection
* Feature Encoding
* Machine Learning Classification
* Hyperparameter Optimization
* Model Evaluation
* Workforce Analytics
* Business Problem Solving

---

## Future Improvements

* SHAP-based model explainability
* XGBoost and LightGBM comparison
* Attrition probability scoring dashboard
* Employee segmentation analysis
* Deployment using Flask or FastAPI
* Workforce retention recommendation engine

---

## Author

**Narmathaa Palanisamy**

Aspiring Data Scientist with a background in Biotechnology and Data Analytics, applying machine learning and statistical modeling techniques to solve real-world business and healthcare challenges.
