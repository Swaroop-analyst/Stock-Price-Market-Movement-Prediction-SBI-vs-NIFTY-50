# Stock-Price-Market-Movement-Prediction-SBI-vs-NIFTY-50
End-to-end time series forecasting and market-relative investment analysis for SBI, benchmarked against NIFTY 50 using ARIMA, SARIMA, Prophet, and machine learning models. The project delivers actionable Buy/Hold/Sell insights based on trend, volatility regimes, and excess return evaluation.

# 📈 Stock Price & Market Movement Prediction — SBI vs NIFTY 50
### Time Series Forecasting & Market-Relative Modeling

---

## 🧭 Business Objective
To build a robust forecasting system for **State Bank of India (SBI)** that:

- Predicts future stock price trend and direction  
- Evaluates whether SBI is outperforming or underperforming the market (**NIFTY 50**)  
- Provides actionable investment insights using **statistical, machine learning, and market-relative modeling**

---

## 📊 Why SBI & Why NIFTY

**Why SBI**
- Highly liquid large-cap Indian stock  
- Sensitive to macroeconomic & interest rate cycles  
- Strong but non-perfect correlation with the overall market → ideal for benchmark modeling  

**Why NIFTY 50**
- Represents Indian equity market performance  
- Enables calculation of **excess returns, beta, and market-adjusted signals**

---

## 🧪 CRISP-DM Framework

### 1️⃣ Business Understanding
**Problem Statement:**  
Can we forecast SBI’s price movement and determine whether it offers better investment opportunity than simply tracking NIFTY 50?

**Success Criteria**
- Accurate price & direction forecasts  
- Clear assessment of market outperformance  
- Practical **Buy / Hold / Sell** recommendations  

---

### 2️⃣ Data Understanding
**Data Sources**
- Historical SBI prices & volume  
- NIFTY 50 index prices  
- Period: Multi-year daily time series  

**Exploration**
- Price trends, volatility regimes  
- Return distributions  
- Correlation & rolling beta vs NIFTY  
- Detection of structural regime shifts  

---

### 3️⃣ Data Preparation
- Missing value treatment  
- Log returns computation  
- Lag features & rolling statistics  

**Benchmark features**
- NIFTY returns  
- Excess return (SBI − NIFTY)  
- Rolling correlation  
- Rolling beta  

**Targets**
- Regression: Next-day price  
- Classification: Up / Down movement  

---

### 4️⃣ Modeling
**Classical Time-Series**
- ARIMA  
- SARIMA  
- Prophet  

**Machine Learning**
- Random Forest  
- XGBoost  

**Benchmark-Aware Decision Models**
- Return-based prediction  
- Direction classification using market features  

These models align SBI’s signals with NIFTY to assess true market outperformance. 
Time-series methods capture structural trends, while machine learning adapts to complex, non-linear market behaviors.
---

### 5️⃣ Evaluation

**Price Forecasting Accuracy (MAE in ₹)**

| Model         | MAE   | Rank |
|---------------|-------|------|
| **Prophet**   | 149.14 | 🥇 Best |
| **SARIMA**    | 188.09 | 🥈 |
| **Random Forest** | 199.78 | 🥉 |
| XGBoost       | 213.23 |      |
| ARIMA         | 226.48 |      |

**Key Insights**
- Prophet best captures long-term trend & regime changes  
- SARIMA strongest classical model  
- Random Forest best ML model for market-relative signals  
- All models face challenges due to market non-stationarity  

**Takeaway:** 
Prophet is the most accurate for forecasting, while Random Forest provides the most reliable market-relative decision signals. Together, they form a complementary system — one structural model for trend, one ML model for benchmark-aware decisions.

👉 In simple terms: **Prophet is best at predicting SBI’s future price**, and **Random Forest is best at telling whether SBI will move upward along with NIFTY**.
---

### 6️⃣ Business Interpretation & Decision Analysis

**Market Position of SBI**
- Rolling beta > 1 → SBI more volatile than NIFTY  
- Positive excess returns → Outperforming the market  
- Prophet & ML direction models → Bullish regime  

**Valuation View**
- Current price trades at a **momentum-driven premium**  
- Premium supported by strong trend & market leadership  
- Not fundamentally overvalued  

**Investment Recommendation**

| Horizon      | Decision |
|--------------|----------|
| Short-term   | 🟢 BUY / HOLD |
| Medium-term  | 🟡 HOLD with risk management |

**Price Outlook**
- Conservative 6–9 month range: **₹1020 – ₹1100**  
- Strong momentum scenario: **₹1150+**  

---

### 7️⃣ Limitations & Risk
- Financial markets are non-stationary  
- Regime shifts & macro shocks reduce forecast stability  
- High beta → higher drawdown risk during corrections  

---

### 8️⃣ Next Steps
- Integrate **news sentiment analysis**  
- Add **macro-economic indicators**  
- Implement **regime-switching models**  
- Extend to **multi-stock portfolio testing**

---

## 🧾 Final Conclusion
This project demonstrates that combining **structural time-series models (Prophet)** with **machine learning and benchmark-aware features** produces reliable, market-relevant investment insights.  

SBI currently exhibits **strong momentum and consistent outperformance over NIFTY**, supporting a **positive investment outlook under disciplined risk management**.
