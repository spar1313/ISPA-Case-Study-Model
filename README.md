Project Overview
Tis repository analyzes customer churn using machine learning models (Decision Trees and Logistic Regression) to identify key factors driving attrition and help design targeted retention strategies. It includes data preprocessing, feature engineering, modeling, validation, model comparison, and interpretability with business-focused evaluation metrics like gains and lift charts.

Data
Source: Kaggle

Features: Age, Tenure, Usage Frequency, Support Calls, Payment Delay, Total Spend, Last Interaction, categorical/demographic features, and target variable 'Churn'.

Getting Started
Prerequisites
Python >= 3.8

pandas

numpy

scikit-learn

matplotlib

Model Pipeline / Structure
Preprocessing: Handles missing values, bins continuous variables, encodes categorical features

Models:

CART Decision Tree (interpretable, captures complex splits)

Logistic Regression (fast, interpretable, baseline)

Validation: Stratified split into train/test, accuracy, ROC-AUC, and classification report

Interpretability: Extract high-confidence decision rules for business action

Business Impact: Segments and prioritizes customers for retention efforts using gains/lift charts

Results
ROC-AUC: Logistic Regression (0.83), CART (0.81)

Top Decile Lift: Over 2× random, meaning focused targeting is twice as effective as random selection

Key Drivers: contract type, monthly spend, tenure, and service usage

Visualizations
Churn class distribution, numeric feature histograms, correlation heatmap

Cumulative gains & lift charts (located in /charts folder)
