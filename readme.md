# Market Memory in Financial Returns
### Autocorrelation and Volatility Clustering Analysis

## 📌 Project Overview
This project empirically investigates whether financial markets exhibit memory by analyzing the autocorrelation structure of asset returns and squared returns. While classical financial theory suggests that returns should be serially uncorrelated, empirical evidence often shows persistent dependence in volatility. This study aims to contrast these two behaviors using time-series methods.

---

## ❓ Research Questions
- Do financial returns exhibit statistically significant autocorrelation?
- Does volatility (proxied by squared returns) display persistent memory?
- What does the difference between return and volatility autocorrelation imply about market efficiency?

---

## 📊 Data
- Asset: Equity index ETF (e.g., SPY)
- Frequency: Daily
- Source: Yahoo Finance
- Time span: Multiple years of historical data

Prices are adjusted for corporate actions, and log returns are used for analysis.

---

## 🧠 Methodology

### 1. Return Construction
- Log returns are computed from adjusted closing prices to ensure time additivity and scale consistency.

### 2. Autocorrelation Analysis
- Sample autocorrelation functions (ACF) are computed for:
  - Raw returns
  - Squared returns (volatility proxy)
- Statistical significance is assessed using asymptotic confidence bands under the null hypothesis of no serial correlation.

### 3. Interpretation Framework
- Autocorrelation in returns is interpreted in the context of weak-form market efficiency.
- Persistent autocorrelation in squared returns is analyzed as evidence of volatility clustering and time-varying risk.

---

## 📈 Key Findings

- Raw returns exhibit little to no statistically significant autocorrelation beyond very short lags.
- Squared returns show strong and persistent autocorrelation across multiple lags.
- This contrast suggests that while markets may be efficient in terms of expected returns, volatility exhibits long memory.

---

## 🛠 Tools & Libraries
- Python
- NumPy
- Pandas
- Matplotlib
- Statsmodels

---

## 📌 Current Status
This repository currently focuses on autocorrelation analysis of returns and volatility. Future extensions may include:
- Rolling-window analysis
- Long-memory estimation (Hurst exponent)
- Information shock and volatility decay analysis
- Null-model comparisons

---

## 📚 References
- Cont, R. (2001). Empirical properties of asset returns.
- Tsay, R. S. *Analysis of Financial Time Series*.
- Stat 110 – Harvard University (Joe Blitzstein)

---

## 👤 Author
Independent quantitative research project by [Your Name].
