# 🏦 Bankruptcy Prevention & Prediction using Machine Learning

## 📌 Project Overview
Bankruptcy is a critical financial condition where a company is unable to repay its debts, often leading to liquidation or restructuring. Early prediction of bankruptcy helps investors, banks, and policymakers reduce financial risk and make informed decisions.

This project focuses on building a **Machine Learning–based Bankruptcy Prediction System** that classifies companies as **Bankrupt** or **Non-Bankrupt** using financial and operational risk indicators.

---

## 🎯 Objectives
- Analyze financial and operational risk data of companies  
- Identify key factors influencing bankruptcy  
- Build and compare multiple Machine Learning models  
- Select the best-performing model for prediction  
- Deploy the model using a **Streamlit web application**

---

## 🧠 Problem Statement
- Financial datasets are complex and vary across industries  
- Economic conditions change rapidly  
- Traditional statistical methods fail to capture non-linear patterns  
- Accurate early bankruptcy detection is crucial to reduce losses  

---

## 📊 Dataset Information
- **Type:** Classification (Binary)
- **Total Companies:** ~250
- **Target Variable:** `class` (Bankruptcy / Non-Bankruptcy)

### 🔑 Features
| Feature | Description |
|------|------------|
| industrial_risk | Industrial risk level (0 = Low, 0.5 = Medium, 1 = High) |
| management_risk | Management risk level |
| financial_flexibility | Financial flexibility level |
| credibility | Company credibility |
| competitiveness | Market competitiveness |
| operating_risk | Operational risk |
| class | Target variable |

---

## 🔍 Exploratory Data Analysis
- Checked for missing values (No null values found)
- Statistical summary analysis
- Correlation analysis using heatmap

### 📈 Key Insights
**Strong Positive Correlation**
- Competitiveness → Class (0.90)
- Credibility → Class (0.76)
- Financial Flexibility → Class (0.75)

**Weak / Negative Correlation**
- Industrial Risk → Class (-0.23)
- Management Risk → Class (-0.37)
- Operating Risk → Class (-0.28)

---

## 🤖 Machine Learning Models Used
- **Logistic Regression** – Simple and interpretable  
- **Random Forest** – Handles non-linear data, provides feature importance  
- **LightGBM** – Fast and efficient gradient boosting model  
- **K-Nearest Neighbors (KNN)** – Distance-based classification  

Models were evaluated using **accuracy and confusion matrix comparison**, and the **best-performing model** was selected.

---

## 🚀 Model Deployment
A **Streamlit Web Application** was built to allow users to input risk values and get real-time bankruptcy predictions.

### 🖥️ Application Features
- User-friendly UI  
- Accepts six financial risk inputs  
- Displays prediction result:
  - **Bankruptcy**
  - **Non-Bankruptcy**

