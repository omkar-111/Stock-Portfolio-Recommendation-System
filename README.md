# 🧠 AlphaVue – AI-Powered Financial Portfolio Recommendation System  

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)  
[![Streamlit](https://img.shields.io/badge/Streamlit-App-red?logo=streamlit)](https://streamlit.io/)  
[![MySQL](https://img.shields.io/badge/MySQL-Database-blue?logo=mysql)](https://www.mysql.com/)  
[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=power-bi)](https://powerbi.microsoft.com/)  
[![Azure](https://img.shields.io/badge/Azure-Cloud-blue?logo=microsoft-azure)](https://azure.microsoft.com/)

---

## 🚀 Overview
**AlphaVue** is an **AI-driven investment recommendation system** that delivers **personalized portfolio suggestions** for stocks and mutual funds based on an investor’s risk profile and goals.  
It combines **machine learning**, **portfolio optimization**, and **financial forecasting**, with insights visualized through **Power BI dashboards**.  

---

## 🌟 Key Features

### 🔐 User Authentication
- Secure login/signup using **bcrypt** password hashing  
- Email & password validation with regex  
- Role-based access for users and admins  

### 🧩 Risk Profiling
- Predicts investor type: **Low / Medium / High Risk**  
- Built using **Random Forest Classifier** trained on demographic & behavioral inputs  

### 💼 Asset Allocation
- Uses **K-Means Clustering** to map optimal ratios across **Equity, Debt, and Gold**  
- Generates risk-adjusted allocation charts  

### 📈 Stock Portfolio Optimization
- Implements **Modern Portfolio Theory (MPT)**  
- Maximizes **Sharpe Ratio** for risk-adjusted returns  
- Displays expected annual return, volatility, and growth  

### 💰 Mutual Fund Recommendation
- Filters top-performing mutual funds by risk level  
- Supports **Lumpsum and SIP** modes with CAGR calculation  

### 📊 Forecasting & Visualization
- Forecasts asset performance using **Prophet**, **ARIMA**, and **LSTM** models  
- **Power BI dashboards** show:
  - Risk distribution  
  - Asset allocation  
  - Portfolio growth forecast  
  - Market insights  

---

## 🧱 System Architecture

1. **Data Sources:** CSV, JSON, and live market data via `yfinance`  
2. **Storage:** **Azure Blob Storage** for raw datasets  
3. **Processing:** **Azure Databricks** for data cleaning, ML training, and forecasting  
4. **Database:** **MySQL** for user and portfolio records  
5. **Frontend:** **Streamlit** for interactive web UI  
6. **Visualization:** **Power BI** dashboards for insights  

---

## 🗄️ Database Schema

| Table | Description |
|:------|:-------------|
| `users` | User info with email, hashed password, and role |
| `portfolios` | Core portfolio details (age, goal, risk appetite) |
| `portfolio_stocks` | Stock investment breakdown |
| `portfolio_mutual_funds` | Mutual fund allocations |
| `portfolio_summary` | Aggregated portfolio value, profit, and return rate |

---

## ⚙️ Tech Stack

| Layer | Technologies |
|:------|:-------------|
| **Frontend** | Streamlit |
| **Backend / ML** | Python, Pandas, NumPy, Scikit-learn, Prophet, TensorFlow |
| **Database** | MySQL |
| **Visualization** | Power BI |
| **Cloud** | Azure Blob Storage, Azure Databricks |
| **Security** | bcrypt, regex validation, email-validator |

---

## 🔍 Workflow

1. User **signs up / logs in**  
2. Provides inputs → **Risk profile** predicted  
3. System generates **Asset Allocation**  
4. Recommends **Stocks & Mutual Funds**  
5. Forecast models predict **future returns**  
6. Results visualized on **Power BI Dashboards**

---

