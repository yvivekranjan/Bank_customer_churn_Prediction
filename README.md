# 🏦 Bank_customer_churn_Prediction
This repository contains an end-to-end machine learning pipeline to predict customer churn in retail banking. Identifying at-risk accounts allows financial institutions to proactively manage portfolios, mitigate credit risk, and optimize core KPIs.
📊 Dataset & Feature Engineering
The analysis is based on a dataset of 10,000 bank customer records. To extract deeper insights into customer behavior, several custom financial features were engineered:  

Credit Utilization: The ratio of a customer's balance to their credit score.  

Interaction Score: A composite metric evaluating engagement based on active membership, product usage, and credit card possession.  

Balance-to-Salary Ratio: An indicator of how significant the account balance is relative to the customer's estimated income.  

Credit Score & Age Interaction: A term designed to capture the combined behavioral impact of age and credit health.  

🛠️ Methodology
Exploratory Data Analysis (EDA): Identified key demographic and financial trends, noting that older customers and those with higher balances showed a higher propensity to churn, while active members were more likely to stay.  

Data Preprocessing: Applied standard scaling to numerical features and label encoding to categorical variables.  

Handling Imbalance: Utilized SMOTE (Synthetic Minority Over-sampling Technique) to ensure the models trained effectively on the imbalanced churn target variable.  

Model Selection: Trained and evaluated multiple classification algorithms, including Logistic Regression, Random Forest, K-Nearest Neighbors, Support Vector Machines, XGBoost, and Gradient Boosting.  

🏆 Key Results
The models were rigorously evaluated using Accuracy, Recall, F1 Score, and ROC AUC metrics to account for the class imbalance.

Gradient Boosting emerged as the best-performing model, achieving the highest F1 Score (0.598) and ROC AUC Score (0.859).  

XGBoost also delivered strong predictive performance, closely following Gradient Boosting.  

Traditional models like Logistic Regression underperformed in capturing the complex, non-linear relationships driving customer churn.  

💻 Tech Stack
Language: Python  

Data Manipulation & Analysis: Pandas, NumPy  

Visualization: Matplotlib, Seaborn  

Machine Learning: Scikit-Learn, XGBoost, Imbalanced-Learn (SMOTE)
