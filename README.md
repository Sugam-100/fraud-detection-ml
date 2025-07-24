# 🛡️ Credit Card Fraud Detection Using Machine Learning

This project aims to detect fraudulent transactions using a real-world dataset. The pipeline includes EDA, feature engineering, model building with Random Forest, and model export.

## 📌 Objective

To identify fraudulent credit card transactions using a supervised ML model and highlight behavior patterns leading to fraud.


- **Features:** transaction type, amount, old & new balances, fraud flags  
- **Target:** `isFraud` (0 = not fraud, 1 = fraud)

## 🔍 Key Features

- Imbalance-aware EDA with fraud percentage tracking
- New balance difference features engineered (`balanceDiffOrig`, `balanceDiffDest`)
- Visualizations: transaction type vs fraud, fraud by time, and correlations
- End-to-end ML pipeline: preprocessing + modeling + export

## 🧠 ML Pipeline

- Preprocessing: StandardScaler + OneHotEncoder (ColumnTransformer)
- Classifier: Random Forest (n=100)
- Evaluation: Confusion matrix, accuracy score
- Export: `fraud_detection_pipeline.pkl` via joblib

## 🖼 Sample Visuals

- 📊 Fraud over time steps
- 📦 Amount distribution (log scale)
- 🔍 Fraud rates by transaction type

