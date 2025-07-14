# 📈 Statistical Arbitrage Strategy using Pairs Trading

## 🧠 Project Overview

This project implements a **Statistical Arbitrage Strategy using Pairs Trading**, a market-neutral approach that profits from the **mean-reverting behavior** between two historically related financial instruments.

We will:

1. **Download historical price data** for two selected stocks.
2. **Visualize their price movements** to assess co-movement behavior.
3. **Perform cointegration analysis** using OLS regression and the Augmented Dickey-Fuller (ADF) test to verify a long-term equilibrium relationship.
4. **Construct and normalize the spread** between the two assets using z-scores.
5. [In next stage] **Generate trading signals** and **backtest** the strategy based on entry/exit thresholds.

This strategy is based on the premise that while individual asset prices may drift apart in the short term, their relative pricing (the spread) tends to revert to a historical mean if they are cointegrated.

📍 **Objective**:  
To explore whether a statistically significant and mean-reverting relationship exists between two assets, and to lay the groundwork for a rule-based trading system using real market data and quantitative finance techniques.

---
