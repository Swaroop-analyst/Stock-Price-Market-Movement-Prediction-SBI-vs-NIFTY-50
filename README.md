# Stock-Price-Market-Movement-Prediction-SBI-vs-NIFTY-50
End-to-end time series forecasting and market-relative investment analysis for SBI, benchmarked against NIFTY 50 using ARIMA, SARIMA, Prophet, and machine learning models. The project delivers actionable Buy/Hold/Sell insights based on trend, volatility regimes, and excess return evaluation.

## Business Objective
Build a forecasting system for SBI to predict price & direction and assess performance relative to NIFTY 50.

## Why SBI & NIFTY
SBI: Highly liquid, macro-sensitive, market leader.
NIFTY: Market benchmark enabling excess return & beta analysis.

## CRISP-DM Summary

### Business Understanding
Goal: Forecast SBI and generate Buy/Hold/Sell insights vs market.

### Data Understanding
Multi-year daily prices for SBI & NIFTY, EDA on trends, volatility, beta, correlation.

### Data Preparation
Returns, lag features, rolling stats, excess returns, rolling beta & correlation.

### Modeling
ARIMA, SARIMA, Prophet, Random Forest, XGBoost.

### Evaluation (MAE ₹)
Prophet: 149.14 (Best)
SARIMA: 188.09
Random Forest: 199.78
XGBoost: 213.23
ARIMA: 226.48

### Business Interpretation
SBI is in bullish regime, outperforming NIFTY. Momentum-driven premium, not overvalued.

### Recommendation
Short-term: BUY / HOLD
Medium-term: HOLD with risk management
Expected 6–9 month price range: ₹1020–₹1100, high momentum scenario ₹1150+.

### Limitations
Non-stationary markets, regime shifts, macro risk.

### Final Conclusion
This project demonstrates that combining structural time-series models (Prophet) with machine learning and benchmark-aware features produces reliable, market-relevant investment insights.
SBI currently exhibits strong momentum and consistent outperformance over NIFTY, supporting a positive investment outlook under disciplined risk management.

### Next Steps
Add news sentiment, macro variables, regime switching, portfolio extension.
