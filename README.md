# 📊 Black–Litterman + Multi-Benchmark Tracking Error (MBTE) Portfolio Optimizer

**Live App:** https://assetpricing.kctradings.com/  
**Author:** Karan Chavan (MSc Quantitative Finance, SMU)  
📧 **Contact:** [Karan80121@gmail.com](mailto:Karan80121@gmail.com)

---

## Overview

This project delivers an end-to-end **portfolio optimization framework** that combines:

- **Black–Litterman (BL)**: equilibrium market returns + investor views  
- **Multi-Benchmark Tracking Error (MBTE)**: alignment to multiple indices (SPY, RSP, IVE, IVW, QQQ, TLT, GLD, HYG, LQD)  
- **Sharpe & Higher-Moments**: max-Sharpe optimization and skew/kurtosis-aware variants

Data is pulled from **Yahoo Finance (`yfinance`)** for S&P 500 tickers, sector/style factors, and benchmarks. The script runs three analyses:
1) Mean-Variance (BL / MBTE / Hybrid)  
2) Maximum Sharpe (with TE constraints)  
3) Higher-Moment-aware (penalizing negative skew and excess kurtosis)

---

## Key Features

| Component | Description |
|:--|:--|
| **Data Loader** | Fetches S&P tickers, sector/style ETFs, and benchmarks; risk-free from `^IRX` (13-week T-Bill). |
| **Black–Litterman** | Posterior expected returns using `P`, `Q`, `Ω` (views). |
| **MBTE** | Minimizes **multi-benchmark tracking error** across several ETFs. |
| **Max Sharpe** | Highest risk-adjusted return, with optional TE constraints. |
| **Higher-Moments** | Penalizes negative skew / excess kurtosis for stability. |
| **Visualizations** | Risk–return, Sharpe, TE, allocations, and higher-moment charts. |

---


