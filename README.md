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
```

---

## 🔍 Exploratory Data Analysis

The project performs Exploratory Data Analysis (EDA) to understand the dataset and identify important patterns.

The following analysis is included:

- Dataset shape and structure
- First and last few records
- Data types and information
- Statistical summary
- Missing value analysis
- Duplicate record analysis
- Class distribution
- Transaction amount distribution
- Correlation analysis

---

## ⚙️ Data Preprocessing

The dataset is divided into:

- **Features (`X`)**
- **Target variable (`y`)**

An **80:20 train-test split** is used with stratification to maintain the class distribution in both training and testing data.

The `Time` and `Amount` features are standardized using `StandardScaler`.

### Handling Class Imbalance

Since the dataset is highly imbalanced, different techniques are used:

- **SMOTE** is used for Logistic Regression.
- **Class Weighting** is used for Decision Tree.
- **Class Weighting** is used for Random Forest.

SMOTE is applied only to the training data to avoid data leakage into the test set.

---

## 🤖 Machine Learning Models

Three classification algorithms are trained and evaluated.

### 1. Logistic Regression

Logistic Regression is used as a baseline classification model for predicting whether a transaction is legitimate or fraudulent.

### 2. Decision Tree

Decision Tree is a tree-based classification algorithm that makes predictions using a series of feature-based decision rules.

### 3. Random Forest

Random Forest is an ensemble learning algorithm that combines multiple decision trees to perform classification.

---

## 📈 Model Evaluation

The models are evaluated using the following performance metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- PR-AUC

The project also includes:

- Confusion Matrix
- ROC Curve
- Precision-Recall Curve
- Random Forest Feature Importance

These evaluation methods help measure how effectively the models identify fraudulent transactions, especially in the presence of severe class imbalance.

---

## 💾 Saved Model Files

The trained model and preprocessing objects are saved using Joblib/Pickle files.

### Files

- `fraud_detection_model.pkl` → Trained fraud detection model
- `scaler.pkl` → Fitted StandardScaler
- `features.pkl` → Feature names and order

These files can be reused later for making predictions on new transaction data.

---

## 📁 Project Structure

```text
Credit-Card-Fraud-Detection/
│
├── Credit_Card_Fraud_Detection_Cleaned.ipynb
├── requirements.txt
├── features.pkl
├── scaler.pkl
└── fraud_detection_model.pkl
```

> The `creditcard.csv` dataset is not included in the repository because of its large file size.

---

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/bhaveshsalunke098/Credit-Card-Fraud-Detection.git
```

### Step 2: Open the Project Folder

```bash
cd Credit-Card-Fraud-Detection
```

### Step 3: Install Required Libraries

Make sure Python is installed, then run:

```bash
pip install -r requirements.txt
```

### Step 4: Download the Dataset

Download the Credit Card Fraud Detection dataset from Kaggle:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

After downloading, place the `creditcard.csv` file inside the project folder.

The folder should look like:

```text
Credit-Card-Fraud-Detection/
│
├── Credit_Card_Fraud_Detection_Cleaned.ipynb
├── creditcard.csv
├── requirements.txt
├── features.pkl
├── scaler.pkl
└── fraud_detection_model.pkl
```

### Step 5: Open Jupyter Notebook

Run:

```bash
jupyter notebook
```

Then open:

```text
Credit_Card_Fraud_Detection_Cleaned.ipynb
```

### Step 6: Run the Notebook

Run all the cells in the notebook in order.

---

## 🎯 Project Objective

The main objective of this project is to develop a Machine Learning-based system for detecting potentially fraudulent credit card transactions.

The project also demonstrates how to handle highly imbalanced datasets and compare different classification algorithms using appropriate evaluation metrics.

---

## 📚 Key Learnings

Through this project, the following concepts were applied:

- Data loading and preprocessing
- Exploratory Data Analysis
- Missing value and duplicate analysis
- Train-test splitting
- Feature scaling
- Handling imbalanced datasets
- SMOTE
- Classification algorithms
- Model evaluation
- Confusion Matrix
- ROC-AUC
- PR-AUC
- Feature importance
- Model serialization using Joblib/Pickle

---

## 👨‍💻 Author

**Bhavesh Salunke**

Machine Learning Project | Python | Machine Learning | Data Science

**GitHub:**  
https://github.com/bhaveshsalunke098
