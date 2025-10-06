# 📊 Black–Litterman + Multi-Benchmark Tracking Error (MBTE) Portfolio Optimizer

**Live App:** 🌐 https://assetpricing.kctradings.com/  
**Author:** Karan Chavan (MSc Quantitative Finance, SMU)  
📧 **Contact:** [Karan80121@gmail.com](mailto:Karan80121@gmail.com)

---

## 🧭 Overview

This project delivers an end-to-end **portfolio optimization framework** that combines:

- **Black–Litterman (BL)**: equilibrium returns + investor views  
- **Multi-Benchmark Tracking Error (MBTE)**: alignment to multiple indices (SPY, RSP, IVE, IVW, QQQ, TLT, GLD, HYG, LQD)  
- **Sharpe & Higher-Moments**: max-Sharpe and skew/kurtosis-aware variants

It uses **Yahoo Finance (`yfinance`)** to fetch data for S&P 500 tickers, sector/style factors, and benchmarks, then runs three analyses:
1) Mean-Variance (BL / MBTE / Hybrid)  
2) Maximum Sharpe (with TE constraints)  
3) Higher-Moment-aware (penalizing negative skew and excess kurtosis)

---

## 🚀 Quick Start

### 1) Clone
```bash
git clone https://github.com/<your-username>/portfolio-bl-mbte-yf.git
cd portfolio-bl-mbte-yf
