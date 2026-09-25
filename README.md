# Credit Card Fraud Detection System

## 📌 Project Overview

This project uses Machine Learning to detect fraudulent credit card transactions.

The objective is to classify credit card transactions into two classes:

- `0` → Legitimate Transaction
- `1` → Fraudulent Transaction

The project includes data preprocessing, exploratory data analysis, handling class imbalance, machine learning model training, model evaluation, feature importance analysis, and saving the trained model for future use.

---

## 📊 Dataset

This project uses the Credit Card Fraud Detection dataset from Kaggle.

**Dataset Link:**  
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

The dataset contains:

- 284,807 total transactions
- 492 fraudulent transactions
- 284,315 legitimate transactions
- 31 columns

The target variable is `Class`:

- `0` = Legitimate Transaction
- `1` = Fraudulent Transaction

The dataset is highly imbalanced because fraudulent transactions are much fewer than legitimate transactions.

> The dataset file (`creditcard.csv`) is not included in this GitHub repository because of its large file size. It can be downloaded from the Kaggle link above.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- Joblib
- Jupyter Notebook

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Understanding
   ↓
Exploratory Data Analysis
   ↓
Class Imbalance Analysis
   ↓
Data Preprocessing
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Handling Class Imbalance
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Feature Importance
   ↓
Model Saving
