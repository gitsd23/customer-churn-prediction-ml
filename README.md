# 📊 Customer Churn Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on predicting whether a telecom customer is likely to churn using Machine Learning techniques.

The project was completed as part of my internship at **SkillINFyTech IT Solutions Private Limited**.

The system analyzes customer demographics, service subscriptions, contract information, and billing details to predict whether a customer is likely to leave the telecom service.

---

## 🎯 Objective

The main objectives of this project are:

- Analyze telecom customer churn data.
- Perform data preprocessing and feature selection.
- Encode categorical features for Machine Learning.
- Handle class imbalance.
- Train and compare Decision Tree and Random Forest models.
- Predict churn for new customers.
- Evaluate model performance using classification metrics and confusion matrices.

---

## 📂 Dataset

The dataset contains information about **7,043 telecom customers** and includes customer demographics, service subscriptions, contract details, billing information, and churn information.

The original dataset contains 33 columns, from which relevant features were selected for model training.

### Target Variable

- `0` → Customer Stayed
- `1` → Customer Churned

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab
- Jupyter Notebook

---

## 🤖 Machine Learning Models

Two primary Machine Learning models were trained:

1. Decision Tree Classifier
2. Random Forest Classifier

An additional Random Forest experiment with alternative class weighting was also performed to investigate the effect of class imbalance.

---

## ⚙️ Data Preprocessing

The project includes:

- Missing value handling
- Duplicate checking
- Feature selection
- Numerical data conversion
- Target variable encoding
- One-hot encoding of categorical features
- Train-test splitting
- Class imbalance handling using balanced class weights

---

## 📊 Model Results

| Model | Accuracy | Churn Recall | Churn F1-Score |
|---|---:|---:|---:|
| Decision Tree | 73.53% | 74% | 0.60 |
| Random Forest (Balanced) | **79.77%** | 52% | 0.58 |
| Random Forest (Churn Weight = 2) | 79.49% | 51% | 0.57 |

### Final Model

The **Random Forest Classifier with balanced class weights** was selected as the final model.

### Final Performance

- Accuracy: **79.77%**
- Churn Precision: **65%**
- Churn Recall: **52%**
- Churn F1-Score: **58%**

The model also provides churn probability predictions for new customers.

---

## 🔮 Custom Customer Prediction

The project includes a custom prediction system that accepts customer information and predicts:

- Whether the customer is likely to churn.
- Probability of staying.
- Probability of churning.

Example:

```text
Prediction: Customer Likely to Churn
Stay Probability: 26.50%
Churn Probability: 73.50%


⚠️ Limitations
The model achieved 79.77% overall accuracy, but the recall for the churned class was 52%.
The model may miss some customers who actually churn.
Performance may vary when applied to different telecom customer populations.
The model relies on historical customer data and may not fully capture future changes in customer behavior.
🔮 Future Improvements

Future versions of this project can include:

Hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
SMOTE and other resampling techniques.
Prediction threshold optimization to improve churn recall.
Advanced boosting algorithms such as XGBoost.
Feature importance and explainability analysis.
Interactive Streamlit web application.
Model deployment for real-time prediction.
📁 Project Structure
customer-churn-prediction-ml/
│
├── Customer_Churn_Prediction.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── images/
👨‍💻 Author

Soumadip Das

AI & Machine Learning Student
