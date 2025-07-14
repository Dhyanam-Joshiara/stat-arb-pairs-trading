
---

## 🔧 Key Sections in the Code

### 1. 📦 Imports and Setup
- Python libraries: `pandas`, `numpy`, `statsmodels`, `seaborn`, `matplotlib`, `yfinance`
- Configuration for plotting and date range

### 2. 🏛️ Universe Selection
- Indian IT stocks (large, mid, and small cap)
- Download historical data (using Yahoo Finance)
- Clean and preprocess price data

### 3. 📊 Correlation Analysis
- Compute and visualize correlation matrix
- Filter highly correlated pairs (e.g., correlation > 0.8)

### 4. 🔁 Helper Functions
- `calculate_hedge_ratio()`: OLS regression for hedge ratio (beta)
- `calculate_spread()`: Computes spread between two stocks
- `adf_test()`: Augmented Dickey-Fuller test for stationarity
- `calculate_half_life()`: Measures speed of mean reversion

### 5. 🔎 Pairs Testing Loop
- Evaluate all pair combinations using:
  - Cointegration (ADF test)
  - Correlation
  - Spread characteristics
  - Half-life of mean reversion
- Store results in a structured DataFrame

### 6. ✅ Result Filtering
- Filter valid pairs (ADF p-value < 0.05)
- Sort by strongest cointegration (lowest ADF stat)
- Optional: Filter by half-life < 30 days

### 7. 🧪 Backtesting Framework
- Generate entry/exit signals based on z-score
- Simulate pair-wise strategy returns
- Calculate performance metrics:
  - Total return
  - Annualized return & volatility
  - Sharpe Ratio
  - Maximum drawdown

### 8. 🚀 Backtest Top Pairs
- Backtest top cointegrated pairs (based on ADF or Sharpe Ratio)
- Export results for review

### 9. 📈 Visualization
- Plot for best pair:
  - Price series
  - Spread with ±1 std dev bands
  - Z-score and trade signals
  - Cumulative strategy returns

### 10. 📊 Portfolio Simulation (Optional)
- Construct equal-weight portfolio of top 3 pairs
- Compute portfolio-level returns and performance
- Compare portfolio Sharpe with individual best pair

### 11. 💰 Investment Simulation (Optional)
- Track actual investment capital over time
- Estimate ROI, final portfolio value, and net profit

---

## 📈 Sample Output (Console)
