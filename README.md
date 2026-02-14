# 🌫️ Air Quality Forecasting Using Machine Learning

> Time-series forecasting of air quality using Facebook Prophet and real-world environmental data.

This project analyzes historical air quality sensor data and builds a machine learning model to forecast future air quality trends. The goal is to demonstrate time-series preprocessing, feature engineering, forecasting, and visualization using Python.

---

## 🧠 Skills & Technologies Demonstrated

**Programming & Libraries**
- Python
- NumPy
- Pandas
- Matplotlib
- Prophet (Facebook/Meta)

**Core Concepts**
- Data cleaning & preprocessing
- Handling missing values
- Time-series forecasting
- Exploratory Data Analysis (EDA)
- Data visualization
- Predictive modeling

---

## 📊 Dataset

Dataset used: **Air Quality UCI Dataset**

The dataset contains hourly air quality measurements including:
- CO(GT)
- NOx(GT)
- NO2(GT)
- C6H6(GT)
- Temperature
- Relative Humidity
- Absolute Humidity

These readings were collected from chemical sensors in an urban environment.

---

## ✨ Project Workflow

### 1️⃣ Data Loading & Exploration
- Loaded CSV dataset using Pandas
- Explored dataset shape, data types, and summary statistics
- Checked missing values and anomalies

---

### 2️⃣ Data Cleaning & Preprocessing
Real-world datasets contain noise and invalid values.

Key preprocessing steps:
- Replaced invalid values (-200) with NaN
- Handled missing values using mean imputation
- Converted Date and Time columns into datetime format
- Combined date & time into a single timestamp feature

This step prepared the data for time-series modeling.

---

### 3️⃣ Feature Preparation for Forecasting
Prophet requires specific column names:
- **ds → timestamp**
- **y → target variable**

The model predicts **Relative Humidity (RH)** as the air quality indicator.

---

### 4️⃣ Time-Series Forecasting with Prophet
Used Facebook Prophet to:
- Train model on historical data
- Capture trend and seasonality
- Generate future predictions (365 hours ahead)

This demonstrates real-world time-series forecasting.

---

### 5️⃣ Forecast Visualization
Generated visualizations including:
- Forecast trend graph
- Confidence intervals
- Trend and weekly seasonality components

These plots help understand long-term air quality patterns.

---

## 📈 Model Output

The model produces:
- Future predictions (yhat)
- Lower and upper confidence intervals
- Trend and seasonal patterns

This allows analysis of how air quality may change over time.

---
