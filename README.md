# 📈 Mathematical & AI-Based Stock Market Analysis

## 📌 Project Overview
This project performs a comprehensive mathematical and statistical analysis of
one year of historical daily stock-market data (OHLCV) for five large-cap
technology companies — **Apple, Amazon, Google, Microsoft, and Tesla**.

By integrating **linear algebra**, **dimensionality reduction**, **feature selection**,
**time-series forecasting**, and **multivariate statistical inference**, the project
aims to uncover latent market structure, identify predictive features, and build
interpretable forecasting models for short-term stock price behavior.

---

## 🎯 Problem Statement
Perform a comprehensive mathematical analysis of one year of historical daily
stock-market data and apply:
- Linear algebra operations
- Dimensionality reduction
- Time-series modeling
- Multivariate statistical inference
- Feature-selection techniques  
to extract insights and build forecasting models.
---

## 🧠 Key Concepts & Techniques Used

### 1️⃣ Data Preprocessing
- Daily OHLCV data collected using **Yahoo Finance (yfinance)**
- Combined dataset with **30 numerical features**
- Missing values handled and data standardized for analysis
---

### 2️⃣ Linear Algebraic Analysis
- Matrix formulation of the stock dataset
- Covariance and correlation matrix computation
- Eigenvalue–eigenvector analysis
- Singular Value Decomposition (SVD)
- Low-rank approximations to identify dominant latent factors

📌 **Insight:**  
A small number of principal components explain a majority of variance, indicating
strong shared market-wide movements among large-cap tech stocks.

---

### 3️⃣ Dimensionality Reduction (PCA & SVD)
- Principal Component Analysis (PCA)
- Scree plot and explained variance analysis
- Interpretation of principal component loadings

📌 **Observation:**  
The first principal component largely represents **overall market movement**,
while subsequent components capture **company-specific behavior**.

---

### 4️⃣ Feature Engineering & Feature Selection
Derived features:
- Daily returns
- Rolling volatility
- Moving averages (MA)
- Price range
- RSI (Relative Strength Index)

Feature-selection techniques:
- Correlation filtering
- Mutual Information
- Random Forest feature importance
- Recursive Feature Elimination (RFE)

📌 **Key Finding:**  
Price-based features (Open, High, Low, Moving Averages) dominate predictive
power, while volume-based features show relatively lower influence.

---

### 5️⃣ Time-Series Forecasting Models
Applied and compared:
- **ARIMA** – univariate forecasting
- **SARIMA** – seasonality-aware forecasting
- **VAR (Vector Autoregression)** – multivariate modeling across stocks

📌 **Insight:**  
Univariate models capture individual trends well, while VAR reveals **cross-stock
dependencies and spillover effects**.

---

### 6️⃣ Multivariate Statistical Inference
- Cross-correlation analysis between stock pairs
- VAR impulse response analysis
- Residual correlation analysis

📌 **Observation:**  
Large-cap technology stocks exhibit significant correlation, confirming strong
sectoral coupling rather than independent movement.
---

## 📊 Dataset Information
- **Source:** Yahoo Finance
- **Period:** 2024 – 2025
- **Frequency:** Daily trading data
- **Records:** ~252 trading days
- **Features:** Open, High, Low, Close, Adjusted Close, Volume (for 5 stocks)

📌 *Adjusted Close is used for return-based analysis as it accounts for corporate
actions such as splits and dividends.*
---

## 🧪 Results & Observations
- Market data is **highly correlated across tech stocks**
- PCA reveals **low intrinsic dimensionality**
- Feature-selection methods consistently highlight **price-based indicators**
- ARIMA/SARIMA provide stable short-term forecasts
- VAR confirms **inter-stock influence**, especially among Apple, Microsoft,
  and Google
---

## ✅ Conclusions
- Linear algebra techniques effectively reveal latent market structure
- Dimensionality reduction simplifies complex financial datasets without
  significant information loss
- Feature selection improves interpretability and model robustness
- Multivariate models provide deeper insights than isolated univariate forecasting
  
This study demonstrates how **mathematics and AI together** can enhance
financial data understanding beyond simple prediction.
--- 
