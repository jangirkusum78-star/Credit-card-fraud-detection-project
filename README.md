# Credit-card-fraud-detection-project



## Project Overview
This project focuses on detecting fraudulent credit card transactions using Machine Learning algorithms. The project was developed using Python in Google Colab.

The main objective is to identify potentially fraudulent transactions from a highly imbalanced dataset.

## Dataset Information
- Dataset: European Credit Card Fraud Detection
- Source: Kaggle
- Original Records: 284,807
- Total Columns: 31
- Target Column: Class
- 0 = Genuine Transaction
- 1 = Fraudulent Transaction

After removing duplicate records:
- Genuine Transactions: 283,253
- Fraudulent Transactions: 473
- Total Records: 283,726

Dataset Link:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

## Technologies Used
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Random Forest
- XGBoost
- SHAP

## Project Workflow

1. Data Loading and Understanding
2. Data Cleaning and Duplicate Removal
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Handling Imbalanced Data
6. Train-Test Split
7. Model Building
8. Hyperparameter Tuning
9. Threshold Optimization
10. Model Evaluation
11. Feature Importance and SHAP Analysis

## Machine Learning Models

Three machine learning algorithms were implemented:

1. Logistic Regression
2. Random Forest
3. XGBoost

## Model Comparison

| Model | Accuracy | Precision | Recall | F1-Score | PR-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 99.93% | 83.53% | 74.74% | 78.89% | 70.06% |
| Random Forest | 99.95% | 91.03% | 74.74% | 82.08% | 79.76% |
| XGBoost | 99.95% | 91.03% | 74.74% | 82.08% | 82.55% |

## Best Model

XGBoost achieved the highest PR-AUC of 82.55% among the evaluated models.

It was selected as the leading model based on its overall precision-recall performance.

## SHAP Analysis

SHAP was used to understand feature contributions to the XGBoost model predictions.

Top influential features based on mean absolute SHAP values:

1. V14
2. V4
3. V12
4. V8
5. V11

Note: V1 to V28 are anonymized PCA-transformed features.

## Key Learnings

- Understanding highly imbalanced datasets.
- Performing data cleaning and EDA.
- Feature engineering and data preprocessing.
- Training and comparing classification models.
- Hyperparameter tuning and threshold optimization.
- Evaluating models using precision, recall, F1-score and PR-AUC.
- Understanding model predictions using SHAP.

## Future Improvements

- Develop a Streamlit application for CSV-based fraud prediction.
- Create an interactive dashboard.
- Enable downloading prediction results.
- Deploy the application using Microsoft Azure.
- Implement real-time fraud detection and model monitoring.

## Limitations

- The dataset contains anonymized PCA features.
- The model requires compatible input features and preprocessing.
- The project is an educational prototype and is not production-ready.
- Further evaluation on an untouched holdout dataset is recommended.

## Repository Structure

credit-card-fraud-detection/
│
├── notebooks/
│   └── credit_card_fraud_detection.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore


Machine Learning Project - Credit Card Fraud Detection

