# 🧠 Consumer Churn Prediction using Machine Learning

## 📘 Course Info

- **Course Title:** Artificial Intelligence  
- **Course Code:** CSE422 
- **University:** BRAC University, Dhaka, Bangladesh  

---

## 📌 Project Overview

This lab project focuses on **developing a consumer classification model** to predict customer churn using machine learning algorithms. The objective is to improve traditional segmentation methods by leveraging modern classification techniques to enhance targeted marketing and customer relationship strategies.

---

## 📂 Dataset Description

- **File Name:** `consumer_classification_dataset.csv`  
- **Total Entries:** 1500  
- **Input Features:** 8 (5 quantitative, 3 categorical)  
- **Output Feature:** `Churn` (binary: 0 = not churned, 1 = churned)  
- **Data Source:** [Google Drive Link](https://drive.google.com/file/d/1pg5z2_6OJsdd7VxGEfa8oXAihYq1KYtV/view)  
- **Balance:** Dataset is balanced (757 class 0, 743 class 1)

### 🔍 Correlation Insights

- Weak individual predictors.
- Slight negative correlation with `Num_purchases` and `Membership_years`.
- Moderate correlation between `Income` and `Credit_score`.

---

## 🧹 Data Preprocessing

- **Missing Value Handling:** Median imputation for `Age`, `Income`, and `Credit_score` (5% missing).
- **Categorical Encoding:** One-Hot Encoding (drop first to avoid multicollinearity).
- **Feature Scaling:** Min-Max Normalization on all numerical features.

---

## ✂️ Dataset Splitting

- **Method:** Stratified Sampling  
- **Train-Test Ratio:** 70% - 30%  
- Maintains proportional distribution of `Churn` classes.

---

## 🤖 Machine Learning Models

### 1. K-Nearest Neighbors (KNN)

- **K value:** 5  
- **Evaluation Metrics:** Accuracy, Confusion Matrix, Precision, Recall  
- **Performance:** Decent but sensitive to feature scaling.

### 2. Logistic Regression

- **Strengths:** Interpretable, solid baseline  
- **Metrics Used:** Accuracy, F1 Score, Confusion Matrix  
- **Performance:** Good, handles binary classification well.

### 3. Neural Network (MLP)

- **Structure:** Input layer → Hidden Layer(s) with ReLU → Output layer with Sigmoid  
- **Metrics:** Accuracy, Precision, Recall, AUC  
- **Performance:** Best overall in terms of accuracy and AUC.

---

## 📊 Model Comparison

| Model              | Accuracy | Best At                        |
|--------------------|----------|--------------------------------|
| KNN                | Moderate | Simple structure, fast testing |
| Logistic Regression| Good     | Interpretability               |
| Neural Network     | Best     | Capturing non-linear patterns  |

- **ROC Curve**, **AUC**, and **confusion matrices** were used for performance comparison.

---

## ✅ Conclusion

- **Best Performer:** Neural Network (due to non-linear capabilities)  
- **Baseline:** Logistic Regression (robust and interpretable)  
- **Lesson Learned:** Importance of preprocessing, model selection, and proper evaluation  
- **Challenges:** Handling missing data, feature scaling, hyperparameter tuning

---

