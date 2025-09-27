# Factor Portfolio Analysis

A quantitative finance project demonstrating **bottom-up portfolio construction** and **performance evaluation** using classical factor investing signals.  
This project mimics the construction of **Fama-French style factors** (Size, Value, Momentum) and evaluates their long-short portfolio returns.

---

## 🚀 Project Workflow

1. **Data Collection**  
   - Download historical stock prices & fundamentals (market cap, P/E) via `yfinance`.  
   - Stocks: AAPL, MSFT, AMZN, META, GOOGL, NVDA, JPM, JNJ, XOM, PG, UNH, TSLA.  

2. **Factor Signal Construction**  
   - **Size:** `log(market cap)`  
   - **Value:** `1 / P/E`  
   - **Momentum:** 12-month return – 1-month return  

3. **Portfolio Construction**  
   - Long **top 30%** of stocks by signal  
   - Short **bottom 30%**  
   - Daily factor return = Long – Short  

4. **Performance Evaluation**  
   - Annualized Return, Volatility, Sharpe Ratio, Cumulative Return  
   - Visualization of cumulative growth of $1 across factors  
   - Factor return correlations (heatmap)  

---

## 📊 Results (2020–2024)

| Factor    | Ann. Return | Ann. Vol | Sharpe | Cumulative |
|-----------|-------------|----------|--------|------------|
| **Size**  | +29.5%      | 30.9%    | 0.95   | +168%      |
| **Value** | -39.9%      | 40.7%    | -0.98  | -85%       |
| **Momentum** | +20.8%  | 38.0%    | 0.55   | +72%       |

---

## 🛠️ Tech Stack

- **Python**: pandas, numpy, matplotlib, seaborn  
- **Finance Libraries**: yfinance  
- **Quant Concepts**: Factor Investing, Long-Short Portfolios, Performance Metrics  

---

## 🔑 Key Takeaways

- Factor-based investing can be **systematically modeled**.  
- Different factors behave differently across market regimes.  
- Performance metrics (Sharpe, Cumulative return) quantify *risk-adjusted profitability*.  

---

## 📌 Future Extensions

- Expand factor set (Profitability, Low Vol, Quality)  
- Apply rolling rebalancing & out-of-sample testing  
- Integrate risk model (e.g., PCA, correlation-based diversification)  

---

## 👤 Author

Developed by **[Your Name]** — aspiring Quantitative Analyst.  
Passionate about **quant research, portfolio construction, and risk modeling**.  


