# 📊 Customer Churn Prediction | Machine Learning Capstone

## 📌 Project Overview

Customer churn is a major business challenge, as retaining existing customers is often more valuable than continuously acquiring new ones.

This project develops an end-to-end Machine Learning solution to predict whether a customer is likely to churn based on demographic, financial, and behavioral characteristics.

The project covers the complete ML workflow — from exploratory data analysis and feature engineering to preprocessing, model comparison, evaluation, feature importance, and prediction for new customers.

---

## 🎯 Business Problem

The objective of this project is to identify customers who are at risk of leaving the organization.

By predicting potential churners in advance, businesses can:

- Identify high-risk customers
- Improve customer retention strategies
- Design targeted offers and campaigns
- Improve customer engagement
- Reduce revenue loss
- Support data-driven business decisions

---

## 🎯 Project Objectives

- Explore and understand customer behavior
- Analyze factors associated with customer churn
- Perform data preprocessing and feature engineering
- Build multiple Machine Learning classification models
- Compare models using cross-validation
- Select the best-performing model
- Evaluate the final model on unseen test data
- Identify important churn-driving features
- Save the trained ML pipeline
- Predict churn for new customers

---

## 📂 Dataset Features

The dataset contains customer-level information including:

| Feature | Description |
|---|---|
| `customer_id` | Unique customer identifier |
| `credit_score` | Customer credit score |
| `country` | Customer's country |
| `gender` | Customer gender |
| `age` | Customer age |
| `tenure` | Number of years with the organization |
| `balance` | Customer account balance |
| `products_number` | Number of products held |
| `credit_card` | Whether customer owns a credit card |
| `active_member` | Whether customer is an active member |
| `estimated_salary` | Estimated customer salary |
| `churn` | Target variable indicating customer churn |

---

## 🔍 Exploratory Data Analysis

The project performs extensive EDA to understand customer behavior and churn patterns.

Visualizations include:

- Numerical feature distributions by churn
- Pairwise feature relationships
- Age distribution by churn
- Tenure distribution
- Gender-wise churn analysis
- Country and customer characteristics vs churn
- Correlation heatmap
- Balance vs number of products
- Churn rate by number of products

---

## 🛠️ Feature Engineering

Additional features were created to improve the predictive information available to the models:

### Balance per Product
Measures the customer's account balance relative to the number of products held.

### Salary-to-Balance Ratio
Compares estimated salary with account balance.

### Age Group
Customers are grouped into meaningful age categories.

### Tenure Bucket
Customer tenure is converted into categorical ranges.

### High Balance Indicator
Identifies customers with relatively high account balances.

---

## ⚙️ Data Preprocessing

A Scikit-learn preprocessing pipeline was created using:

- Missing value imputation
- Median imputation for numerical variables
- Most-frequent imputation for categorical variables
- StandardScaler for numerical features
- OneHotEncoder for categorical features
- ColumnTransformer
- Scikit-learn Pipeline

This ensures consistent preprocessing during both model training and prediction.

---

## 🤖 Machine Learning Models

Five classification algorithms were trained and compared:

1. Logistic Regression
2. Random Forest Classifier
3. Gradient Boosting Classifier
4. AdaBoost Classifier
5. Support Vector Classifier (SVC)

---

## 🔄 Model Validation

The models were evaluated using:

- Stratified 5-Fold Cross-Validation
- ROC-AUC scoring

The model with the highest mean cross-validation ROC-AUC was automatically selected as the best model.

---

## 📊 Model Evaluation

The final model was evaluated on unseen test data using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Classification Report
- Confusion Matrix

---

## 🔎 Feature Importance

For tree-based models that support feature importance, the project extracts and visualizes the Top 20 most influential features.

This helps improve model interpretability and provides insights into the factors associated with customer churn.

---

## 💾 Model Deployment Artifact

The final trained preprocessing + Machine Learning pipeline is saved using Joblib:

`best_churn_pipeline.pkl`

This allows the trained model to be loaded and reused without retraining.

---

## 🔮 New Customer Churn Prediction

The final pipeline can predict churn for a completely new customer.

The prediction process:

Customer Information  
↓  
Feature Engineering  
↓  
Preprocessing  
↓  
Trained ML Model  
↓  
Churn Prediction + Probability

---

## 🧰 Tech Stack

| Technology | Usage |
|---|---|
| Python | Data analysis and ML |
| Pandas | Data manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine Learning |
| Joblib | Model serialization |
| Google Colab / Jupyter | Development environment |



## 🚀 Machine Learning Workflow

Data Collection  
→ Data Inspection  
→ Exploratory Data Analysis  
→ Feature Engineering  
→ Preprocessing  
→ Train/Test Split  
→ Model Training  
→ Cross-Validation  
→ Model Comparison  
→ Best Model Selection  
→ Model Evaluation  
→ Feature Importance  
→ Model Saving  
→ New Customer Prediction

---


## 👩‍💻 Author

**Kanishka Agarwal**

Aspiring Data Analyst | Python | SQL | Power BI | Excel | Tableau | Machine Learning
