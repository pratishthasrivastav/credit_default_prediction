# 🧠 Credit Card Default Prediction System

This project aims to predict whether a customer will default on their credit card payment in the next month using data science and machine learning techniques. It is based on the UCI Credit Card Default dataset and follows the CRISP-DM methodology for solving real-world classification problems.

> 🔍 By [Pratishtha Srivastava]

---

## 🧩 Problem Statement

Credit card default is a major concern for financial institutions. Predicting customers who are likely to default can help banks minimize losses, adjust credit policies, and manage risk.

**Objective**: Build and evaluate machine learning models that classify whether a customer will default in the next billing cycle based on financial history and behavioral variables.

---

## 📊 Dataset Summary

- **Source**: UCI Machine Learning Repository  
- **Records**: 30,000 credit card holders  
- **Target Variable**: `default payment next month` (1 = default, 0 = non-default)  
- **Features**: Credit limit, demographic info, past payments, bill amounts, etc.

---

## 🧠 CRISP-DM Pipeline Followed

### 1. Business Understanding
Defined the financial impact and importance of accurately predicting defaults.

### 2. Data Understanding
Explored distribution, outliers, and feature correlation.

### 3. Data Preparation
- Dropped unnecessary columns (e.g., ID)
- Handled missing data
- Scaled numerical features using `StandardScaler`
- Split data into training and testing sets (80/20)

### 4. Modeling
Trained and compared:
- **Logistic Regression**  
- **Random Forest Classifier**

### 5. Evaluation
- Evaluated models using Accuracy, Precision, Recall, F1-score, ROC AUC
- **Random Forest achieved better recall (36%) and ROC AUC (0.75)** compared to logistic regression
- Used confusion matrix and classification reports for analysis

### 6. Insights
- Class imbalance significantly impacts recall
- `PAY_0`, `LIMIT_BAL`, and recent bill/payment amounts were key predictors
- Feature correlation and importance were visualized using heatmaps and bar charts

---

## 📌 Key Technologies Used

- Python  
- Pandas, NumPy  
- Seaborn, Matplotlib  
- Scikit-learn  
- Jupyter Notebooks (VS Code)

---

## ✅ Outcome

Successfully built a baseline classification model to detect potential defaulters. The Random Forest model outperformed Logistic Regression and can help banks identify high-risk customers more effectively.

---

## 📈 Next Steps

- Improve recall by handling class imbalance (e.g., SMOTE or class weights)
- Use XGBoost or LightGBM for higher performance
- Deploy model using Flask or Streamlit

---

## 🙋‍♀️ Author

**Pratishtha Srivastava**  
Data Science & AI Enthusiast  
[LinkedIn](https://www.linkedin.com/in/pratishtha-srivastava-3974b5249)

---

> ⭐ If you found this project interesting, feel free to star it and connect!

