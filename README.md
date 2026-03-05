                                                               Customer Churn Prediction Project

A complete end-to-end Machine Learning project that predicts whether a bank customer will churn (leave the bank) using classification models and a deployed Flask web application.

📌 Project Overview
Customer churn — when a customer stops using a product or service — is a major concern for businesses.
In this project, we analyzed the Churn_Modelling dataset from Kaggle to understand the factors driving churn and built machine learning models to predict which customers are likely to leave.The goal is to help businesses proactively target high-risk customers and reduce churn, improving revenue and customer retention.
This project:
Performs Exploratory Data Analysis (EDA)
Handles class imbalance using SMOTE
Trains multiple ML models
Selects the best model using ROC-AUC
Deploys the model using Flask
Provides real-time churn prediction via web interface

📂 Dataset
File: Churn_Modelling.csv
Total Records: 10,000

Target Variable: Exited
1 → Customer Will Churn ,
0 → Customer Will Not Churn

🧠Features Used
CreditScore,Geography,Gender,Age,Tenure,Balance,NumOfProducts,HasCrCard,IsActiveMember,EstimatedSalary
Categorical variables were encoded using One-Hot Encoding.

🔎 Exploratory Data Analysis
Key Insights:
Customers from Germany show higher churn rate.
Customers with 3 or 4 products have extremely high churn.
Inactive members are more likely to churn.
Older customers have higher churn probability.

⚙️ Machine Learning Models Used
Logistic Regression
Random Forest
XGBoost

🏆 Best Model: Random Forest
Cross Validation ROC-AUC: Random Forest → 0.963
Final Test Results: Accuracy → 84%
                    ROC-AUC → 0.85
                    Recall (Churn Class) → 0.59

⚖️ Handling Imbalanced Data
Since churn class was only ~20%, SMOTE was used to balance the training dataset

📊 Model Evaluation
Confusion Matrix
ROC Curve
Precision-Recall Curve
Feature Importance Plot

🛠️ Tech Stack: Python, Pandas, NumPy, Scikit-Learn (Random Forest), XGBoost, SMOTE (Imbalanced-Learn), Matplotlib, Seaborn, Flask, Pickle.
