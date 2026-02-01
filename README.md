# HR Employee Attrition Prediction 🏃‍♂️💼

This project predicts the likelihood of employees leaving a company (Attrition) using machine learning techniques to handle imbalanced data.

## 📌 Project Overview

The goal is to analyze HR data and build a model that can identify employees likely to resign, allowing for better retention strategies.

## 🛠️ Tech Stack

* **Python**
* **Pandas**: For data manipulation and loading.
* **Scikit-Learn**: For preprocessing, modeling, and evaluation.
* **Imbalanced-learn (SMOTE)**: For balancing the dataset classes.

## 🏗️ Project Workflow

### 1. Data Loading

* Loading the dataset: `WA_Fn-UseC_-HR-Employee-Attrition.csv`.

### 2. Data Preprocessing

* **Dropping Unnecessary Columns**: Removed irrelevant features like `EmployeeCount`, `Over18`, `StandardHours`, and `EmployeeNumber`.
* **Label Encoding**: Used `LabelEncoder` to convert all categorical text columns and the target variable (`Attrition`) into numerical values.

### 3. Handling Class Imbalance

* Applied **SMOTE** (Synthetic Minority Over-sampling Technique) to the training data to fix the imbalance between employees who stay and those who leave.

### 4. Machine Learning Modeling

Two main models were trained and compared:

* **Support Vector Classifier (SVC)**
* **Logistic Regression**

### 5. Model Evaluation

The performance was evaluated using:

* **Accuracy Score** (for both Training and Testing sets).
* **Classification Report** (Precision, Recall, and F1-Score).
