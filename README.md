Customer Churn & Customer Lifetime Value Predictor

A machine learning project that predicts which customers are likely to churn and estimates their Customer Lifetime Value (CLV), helping businesses identify high-risk, high-value customers for targeted retention strategies.

🚀 Overview

This system combines churn classification with CLV estimation to give businesses a fuller understanding of customer behavior.
It includes data preprocessing, model training, explainability, and a simple interface where users can upload customer data and get instant churn risk scores and expected lifetime value.

🧠 Key Features

Churn Prediction:
Uses XGBoost/CatBoost models to classify customers as “likely to churn” or “likely to stay.”

CLV Estimation:
Computes expected lifetime value using churn probability and monthly charges (or alternative CLV formulas).

Explainability:
Highlights the top factors driving churn through feature importance.

Minimal Frontend UI:
Users can upload a CSV file and receive churn predictions, CLV scores, and suggested actions.

Exportable Models:
Trained models saved as .pkl files for deployment or integration.

🛠️ Tech Stack

Python, Pandas, NumPy

Scikit-learn, XGBoost, CatBoost

Matplotlib / Seaborn for EDA

Streamlit / Flask for predictions UI

Jupyter Notebook for development

📊 Modeling Workflow
1️⃣ Exploratory Data Analysis

Customer demographics

Contract type & billing patterns

Service usage

2️⃣ Preprocessing

Encoding categorical variables

Handling missing values

Outlier/invalid value correction

Feature scaling (if needed)

3️⃣ Churn Prediction Model

Trained using XGBoost & CatBoost

Evaluated using accuracy, precision, recall, F1-score

Achieved ~78% accuracy during testing

4️⃣ CLV Calculation using kaplan-meier survival function

5️⃣ Frontend Interface

Upload CSV → Get churn probability + CLV

Filter by high-risk, high-value customers

Shows top churn-driving features

▶️ How to Run
Install dependencies
pip install -r requirements.txt

Start the UI
streamlit run app.py

Upload your CSV

The tool returns churn labels, probabilities, CLV values, and explanations.

📌
