# ⚡ Time Series Electricity Demand Forecasting  
### *Machine Learning & Deep Learning for Smart Grid Prediction*

This project builds a **time series forecasting model** using a real-world Kaggle dataset containing hourly electricity consumption and weather-related variables. The objective is to predict electricity demand for the next **2,160 hours (≈ 3 months)** using advanced machine learning and ensemble modeling techniques.

---

## 📌 Project Overview
The project focuses on developing forecasting models for energy consumption to support **smart-grid planning**, **resource allocation**, and **energy management**.  
The workflow includes:

- Data preprocessing & cleaning  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Model selection & hyperparameter tuning  
- Performance evaluation (RMSE & R²)  
- Forecasting future electricity demand  

This project was completed as part of the **Predictive Modeling & Time Series Analysis** coursework.

---

## 📂 Dataset
Dataset: **Hourly Electricity Consumption + Weather Data (Kaggle)**  
The dataset contains:
- Temperature, humidity, wind metrics  
- Hourly load demand  
- Timestamp (date-time) fields  
- Energy usage patterns across multiple seasons and weather conditions  

---

## 🛠️ Tech Stack
- **Python 3.x**
- Libraries:
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scikit-learn`
  - `catboost`
  - `xgboost`
  - `tensorflow` / `keras`
  - `statsmodels`

---

## 🔧 Workflow

### **1️⃣ Data Preprocessing**
- Handling missing values  
- Noise/outlier reduction  
- Date-time feature extraction  
- Categorical & numerical encoding  
- Scaling & normalization  
- Train-test splitting (80:20, 70:30, 60:40 scenarios)

### **2️⃣ Exploratory Data Analysis**
- Time series decomposition  
- Seasonal pattern identification  
- Correlation with weather variables  
- Trend & cyclical component analysis  

### **3️⃣ Feature Engineering**
- Lag features  
- Rolling statistics  
- Time-based predictors (hour, day, month, season)  
- Weather-based power consumption factors  

---

## 🤖 Machine Learning Models

### ✔ XGBoost Regressor  
Tree-based gradient boosting model optimized for tabular time series.

### ✔ CatBoost Regressor  
Handles categorical and numerical features efficiently with minimal preprocessing.

### ✔ Ensemble Stacking Model (LSTM + CatBoost)  
Combines the strengths of:
- **LSTM**: sequential pattern learning  
- **CatBoost**: tree-based non-linear relationships  
This hybrid model produced the **best performance**.

---

## 📊 Evaluation Metrics
Models were evaluated using:

| Metric | Description |
|--------|-------------|
| **RMSE** | Measures average prediction error |
| **R² Score** | Measures how much variance is explained by the model |

The **Ensemble LSTM–CatBoost model** achieved:
- 📉 **Lowest RMSE** across all train-test splits  
- 📈 **Consistently high R²** indicating strong predictive capability  

---

## 🔮 Forecasting Output
The best model was used to forecast **2,160 hours (≈ 3 months)** of future demand.  
Forecast results can support:
- Smart-grid energy distribution  
- Resource optimization  
- Load balancing  
- Seasonal demand planning  

---

## ▶️ How to Run

Clone repository:
```bash
git clone github.com/kaylapm/Time-Series-Electricity-Demand-Forecasting-Project.git
cd electricity-demand-forecasting
