# Lead Conversion Model for X Education

This repository contains the code and analysis for developing a lead conversion model for X Education. The objective is to identify the most promising leads (hot leads) and improve the lead conversion rate from around 30% to approximately 80%.

## Table of Contents

1. [Introduction](#introduction)
2. [Data](#data)
3. [Methodology](#methodology)
4. [Feature Importance](#feature-importance)
5. [Model Evaluation](#model-evaluation)

## Introduction

X Education sells online courses to industry professionals. The goal is to build a predictive model to assign a lead score to each lead, helping the sales team focus on leads that are most likely to convert into paying customers.

## Data

The dataset provided contains around 9000 data points with various attributes such as:
- Lead Source
- Total Time Spent on Website
- Total Visits
- Last Activity
- Lead Origin
- and more...

The target variable is `Converted`, indicating whether a lead was converted (`1`) or not (`0`).

## Methodology

### Data Preprocessing

1. **Handling Missing Values**: Missing values were imputed or treated appropriately.
2. **Data Cleaning**: Irrelevant columns were removed.
3. **Encoding Categorical Variables**: Categorical features were converted to numerical values using one-hot encoding.
4. **Feature Scaling**: Numerical features were scaled using standardization.

### Exploratory Data Analysis (EDA)

1. **Distribution Analysis**: Analyzed the distribution of features and the target variable.
2. **Correlation Analysis**: Examined correlations between features and the target variable.
3. **Outlier Detection**: Identified and handled outliers in the dataset.

### Feature Engineering

1. **New Feature Creation**: Generated new features to improve model performance.
2. **Feature Selection**: Selected the most relevant features using techniques like Recursive Feature Elimination (RFE).
3. **Handling Multicollinearity**: Addressed multicollinearity among features.

### Model Building

1. **Model Selection**: Multiple logistic regression models were trained with different hyperparameters.
2. **Hyperparameter Tuning**: Used GridSearchCV for hyperparameter optimization.
3. **Model Evaluation**: Evaluated models using accuracy, precision, recall, F1-score, and AUC-ROC.

## Feature Importance

Key features influencing lead conversion:
- **Total Time Spent on Website**: Most significant predictor of conversion.
- **Occupation (Working Professional)**: Strong positive impact on conversion likelihood.
- **Last Activity (SMS Sent, Email Opened)**: Crucial for lead engagement.
- **Lead Origin (Lead Add Form, Landing Page Submission)**: Important sources of high-quality leads.
- **Lead Source (Olark Chat, Welingak Website)**: Effective lead generation channels.
- **Missing Data Indicators**: Absence of certain data fields correlated with higher conversion rates.

## Model Evaluation

- **Recall**: Focused on maximizing recall to ensure most potential leads are captured.
- **Precision**: Monitored to maintain a balance and avoid too many false positives.
- **F1-Score**: Used as a comprehensive metric to balance precision and recall.
- **AUC-ROC**: Evaluated the model's ability to distinguish between classes.

---

By following this structured approach, X Education can effectively identify and target high-potential leads, significantly improving their lead conversion rate and overall business performance. If you have any questions or need further assistance, feel free to reach out or open an issue on GitHub.
