# AI-Powered-Sales-Forecasting-Platform-Microsoft-Fabric-XGBoost-Power-BI-
# 🚀 AI-Powered Sales Forecasting Platform (Microsoft Fabric + XGBoost + Power BI)

---

## 📌 Project Overview

This project is an **end-to-end AI-driven analytics platform** designed to forecast retail sales and provide business insights through an interactive dashboard.

It integrates:

* **Data Engineering (Microsoft Fabric Lakehouse)**
* **Machine Learning (XGBoost Forecasting Model)**
* **Business Intelligence (Power BI Dashboard)**

The goal is to simulate a **real-world enterprise analytics pipeline**, enabling organizations to make **data-driven decisions**.

---

## 🎯 Business Problem

Retail businesses often struggle with:

* Inaccurate sales forecasting
* Lack of visibility into store-level performance
* Difficulty identifying trends and anomalies

👉 This project solves these problems by:

* Predicting future sales using ML
* Comparing actual vs predicted performance
* Highlighting error patterns and insights

---

## 🏗️ System Architecture

```text
Raw Data → Fabric Lakehouse → PySpark Processing → Feature Engineering → ML Model (XGBoost)
→ Predictions Stored → Power BI Dashboard
```

---

## 🛠️ Tech Stack

### 🔹 Data Engineering

* Microsoft Fabric (Lakehouse)
* OneLake Storage
* PySpark (Data Processing)

### 🔹 Machine Learning

* Python
* Scikit-learn
* XGBoost (Final Model)

### 🔹 Data Visualization

* Power BI
* DAX (KPIs, RMSE)

---

## 📂 Dataset Description

Used **Walmart Retail Dataset** with features:

* Store, Department
* Weekly Sales (Target Variable)
* Temperature, Fuel Price
* CPI, Unemployment
* Holiday Indicator

---

## ⚙️ Project Workflow

---

### 🔹 1. Data Ingestion (Fabric Lakehouse)

* Uploaded CSV datasets into OneLake
* Loaded data using PySpark
* Created structured tables

---

### 🔹 2. Data Cleaning & Transformation

* Handled missing values
* Converted data types
* Joined datasets (sales + external features)
* Ensured time-series consistency

---

### 🔹 3. Feature Engineering

Key features created:

* `lag_1` → Previous week's sales
* `rolling_avg` → Moving average trend
* Time-based ordering

👉 These features helped capture **temporal dependencies**

---

### 🔹 4. Model Development

#### ✅ Baseline Model:

* Random Forest Regressor

#### 🚀 Final Model:

* XGBoost Regressor

Reasons for choosing XGBoost:

* Handles non-linear patterns
* Learns from residual errors
* Better performance on structured data

---

### 🔹 5. Model Evaluation

Metric used:

👉 **RMSE (Root Mean Squared Error)**

```text
Random Forest RMSE: 13002  
XGBoost RMSE: 12338
```

✔ XGBoost selected due to lower error

---

### 🔹 6. Prediction Output

Created:

* `Predicted_Sales`
* `Error = Actual - Predicted`

Stored in:

```text
sales_forecast_dashboard (Lakehouse Table)
```

---

### 🔹 7. Power BI Dashboard

Built an interactive dashboard with:

#### 📊 Key Visuals

* Actual vs Predicted Sales Trend (Line Chart)
* Store-wise Sales Distribution
* Error Analysis by Store
* KPI Cards (Total Sales, Predicted Sales, RMSE, Avg Error)

#### 🎛️ Filters

* Store
* Department
* Date Range
* Holiday Indicator

---

## 📈 Key Insights

* Identified stores with high forecasting error
* Observed seasonal sales spikes
* Compared model performance over time
* Enabled interactive business exploration

---

## 🧠 Key Learnings

* Built end-to-end pipeline using Microsoft Fabric
* Applied feature engineering for time-series forecasting
* Compared ML models and optimized performance
* Designed professional BI dashboards
* Integrated ML outputs into business reporting

---

## 🚀 Future Enhancements

* LSTM-based deep learning forecasting
* Real-time streaming pipeline
* Azure ML deployment for live predictions
* Customer churn prediction module
* NLP-based sentiment analysis

---

## 📊 Dashboard Preview

> Interactive Power BI dashboard showing sales trends, predictions, and performance metrics.

---

## ▶️ How to Run

1. Upload datasets to Microsoft Fabric Lakehouse
2. Run PySpark notebook for preprocessing
3. Train ML model (Random Forest → XGBoost)
4. Save predictions into Lakehouse table
5. Connect Power BI using SQL Endpoint
6. Build dashboard

---

## 💡 Project Highlights

✔ End-to-end pipeline (Data → ML → BI)
✔ Real-world business problem
✔ Model comparison and optimization
✔ Production-style architecture
✔ Clean and interactive dashboard

---

## 👨‍💻 Author

**Harshit Prakash Pandey**

* Data Analytics & Machine Learning Enthusiast
* Skilled in Python, SQL, Power BI, Microsoft Fabric

---

## ⭐ If you found this useful

Give this repo a ⭐ and feel free to connect!

---
