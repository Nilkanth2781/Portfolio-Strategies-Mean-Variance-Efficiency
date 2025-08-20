---

# 📊 Project 3 – Portfolio Strategies & Mean-Variance Efficiency

## Overview

This project, completed as part of **FINA 6333 – Spring 2024**, evaluates the **risk-return tradeoffs** and **mean-variance efficiency** of several well-known portfolio strategies. Using long-term historical data (1927–2023), we compare traditional and modern portfolio designs to assess their performance, resilience, and suitability for different investor profiles.

## 🔑 Portfolios Analyzed

* **All-Equity Portfolio** – 100% S\&P 500 exposure
* **Traditional 60/40 Portfolio** – 60% equities, 40% bonds
* **Harry Browne’s Permanent Portfolio** – 25% stocks, 25% bonds, 25% cash, 25% gold
* **Ray Dalio’s All Weather Portfolio** – diversified mix of stocks, bonds, commodities, and gold
* **Custom Optimized Portfolio** – constructed via **maximum Sharpe ratio optimization**

## 📂 Project Structure

```
.
├── Project_3_Team_36.ipynb    # Jupyter notebook with full analysis
├── Project3_Team36.docx       # Written report
├── histretSP.csv              # Historical returns dataset
└── README.md                  # Documentation
```

## ⚙️ Methodology

### Data

* Source: **Ibbotson historical returns (S\&P 500, T-Bonds, T-Bills, Gold, Commodities, Real Estate, Baa Bonds)**
* Period: **1927 – 2023**
* Frequency: Annual returns

### Techniques

1. **Portfolio Construction**

   * Implemented fixed-weight portfolios (Equity-only, 60/40, Browne, Dalio).
   * Built optimized portfolio using Monte Carlo simulation and mean-variance optimization.

2. **Risk & Performance Metrics**

   * Mean return, volatility, Sharpe ratio
   * Kurtosis & skewness (tail risk)
   * Efficient frontier plots
   * Cumulative return comparisons

3. **Optimization**

   * Simulated 100,000 random portfolios.
   * Identified **Max Sharpe Ratio portfolio** and **Min Volatility portfolio**.
   * Compared traditional allocations against optimal frontier.

## 📊 Results (Summary)

### Risk-Return Tradeoff

| Portfolio                 | Mean Return | Volatility | Sharpe Ratio | Skewness | Kurtosis |  
| ------------------------- | ----------- | ---------- | ------------ | -------- | -------- |
| All Equity                | 11.7%       | 19.6%      | 0.43         | -0.44    | 0.05     | 
| Traditional 60/40         | 8.9%        | 12.2%      | 0.46         | -0.41    | 0.08     |  
| Harry Browne Permanent    | 6.6%        | 7.3%       | 0.45         | +0.61    | 3.51     |  
| Ray Dalio All Weather     | 7.2%        | 7.8%       | 0.49         | -0.13    | 1.03     | 
| Custom Optimized (Sharpe) | 8.8%        | 10.4%      | 0.53         | -0.70    | 0.94     |  

### Key Insights

* **All Equity** has the highest returns but extreme volatility – inefficient under MPT.
* **60/40** remains balanced but underperforms in today’s low-interest-rate environment.
* **Harry Browne’s portfolio** provides stability across regimes but limits growth.
* **Ray Dalio’s All Weather** shows strong Sharpe ratio and resilience across cycles.
* **Optimized portfolio** achieves the best risk-adjusted returns, validating Modern Portfolio Theory.

### Efficient Frontier Findings

* Traditional 60/40 is **not on the efficient frontier** → inefficient.
* Browne and Dalio portfolios are **closer to efficient** due to diversification.
* Optimized portfolio **lies on the efficient frontier**, maximizing Sharpe ratio.

