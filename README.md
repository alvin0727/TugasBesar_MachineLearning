# 🏦 Bank Marketing Campaign Analysis

This project focuses on analyzing the **Bank Marketing Dataset**, which is related to a marketing campaign conducted by a Portuguese banking institution. The campaign was based on phone calls, and the dataset is widely used for predictive modeling to determine whether a client will subscribe to a term deposit.

The dataset is sourced from the **UC Irvine Machine Learning Repository**:  
[Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)

---

## 📊 Dataset Overview

### General Information
The dataset contains information about clients and the marketing campaign. It includes the following key columns:
- **`age`**: Age of the client.
- **`job`**: Type of job.
- **`marital`**: Marital status.
- **`education`**: Education level.
- **`balance`**: Average yearly balance.
- **`housing`**: Whether the client has a housing loan.
- **`loan`**: Whether the client has a personal loan.
- **`contact`**: Communication type (e.g., cellular, telephone).
- **`day`**: Last contact day of the month.
- **`month`**: Last contact month of the year.
- **`duration`**: Duration of the last contact in seconds.
- **`campaign`**: Number of contacts performed during this campaign.
- **`pdays`**: Number of days since the client was last contacted.
- **`previous`**: Number of contacts performed before this campaign.
- **`poutcome`**: Outcome of the previous marketing campaign.
- **`y`**: Target variable (whether the client subscribed to a term deposit).

---

## 🛠️ Project Goal

The goal of this project is to analyze the dataset and build a predictive model to determine whether a client will subscribe to a term deposit. We use **Sequential Feature Selection**, a greedy algorithm that iteratively selects the best features from the dataset to improve the performance of the predictive model.

---

# Model Analysis in Bank Marketing Campaign

## 1. Support Vector Machine (SVM)

### **Evaluation Results**
After performing hyperparameter tuning using **GridSearchCV**, the best **C value** obtained was **10**. The evaluation results of the model on the validation set are:

- **Accuracy**: 87.69%
- **Precision**: 69.34%
- **Recall**: 54.65%
- **F1-Score**: 61.12%
- **ROC AUC**: 74.72%

## 2. Decision Tree Classifier

### **Evaluation Results**
After performing grid search with cross-validation, the **best parameters** obtained were:
- **max_depth**: 3
- **min_samples_leaf**: 10

The evaluation results of the model on the test set are:

- **Accuracy**: 87.95%
- **Precision**: 70.09%
- **Recall**: 55.76%
- **F1-Score**: 62.11%
- **ROC AUC**: 75.32%

---

## 3. Customer Segmentation using K-Means

### **Cluster Analysis**
We have identified **four clusters** represented by red, green, purple, and blue colors:

![K-Means](https://github.com/alvin0727/TugasBesar_MachineLearning/blob/main/images/image1.png)

- **Red Cluster**: Includes customers aged **20 to 35 years old**. The most common occupations in this group are **students (12)** and **administrators (7)**, with the majority being **single**.
- **Green Cluster**: Includes customers aged **28 to 39 years old**. The most frequent occupations in this group are **management (0)** and **technician (1)**, with most individuals being **married**.
- **Purple Cluster**: Includes customers aged **39 to 47 years old**. The predominant occupations in this cluster are **admin, services, self-employed, and unemployed**, with the majority being **married**.
- **Blue Cluster**: Includes customers aged **48 to 58 years old**. The most common occupations in this group are **management, technician, entrepreneur, blue-collar, admin, services, and unemployed**, with most individuals being **married**.

These insights help in understanding customer segmentation, which can be used to target specific demographics for future marketing campaigns.

---

Thank you for reading! We appreciate your interest in this analysis. 😊