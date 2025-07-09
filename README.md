# Quantitative Metrics
Portfolio analysis on Quantitative Metrics (Sharpe, Alpha, Beta) for 1Y, 2Y, 3Y and quarterly performance with 29 stocks.

## Files
**Sharpe Ratios:**
- `sharpe_ratio_calculator.py` - quarterly sharpe + market bottom performance for entire portfolio

**Alpha Analysis:**
- `portfolio_alpha_analysis.py` - comprehensive alpha analysis vs S&P 500 for individual stocks and portfolio

**Beta Analysis:**  
- `beta_calculator.py` - 2Y volatility vs market

## Results Summary

### Sharpe Ratios
- **Q1-Q2 2025:** -0.12 (underperformed risk-free rate)
- **Market Bottom (Apr-Jul):** 2.82 (recovered)
- **SP500 Q1-Q2:** 0.11 (Outperformed Portfolio in 1H)

### Portfolio Performance
- **YTD 2025:** 5.92%
- **Q1 2025:** -4.77%
- **Q2 2025:** 10.99%  
- **Market (S&P 500) YTD:** 6.38%
- **Risk-Free Rate:** 4.42% (3 Month Treasury Bill)

### Alpha Analysis

#### Portfolio Alpha Summary
- **YTD Portfolio Alpha:** -0.46%
- **Latest Quarter (Q2 2025) Alpha:** 0.83%
- **Trailing 4-Quarter Average Alpha:** -0.35%
- **Trailing 2-Quarter Average Alpha:** 0.22%

#### Individual Stock Alpha (1Y)
**Best performers:**
- IDCC: 77.16%
- GILD: 59.76%
- WFC: 28.03%
- META: 27.14%
- NOK: 23.47%

**Worst performers:**
- NVO: -61.53%
- REGN: -59.95%
- UNH: -49.78%
- AMD: -33.87%
- AMAT: -33.64%

#### Individual Stock Alpha (2Y)
**Best performers:**
- IDCC: 127.09%
- DELL: 95.54%
- KLAC: 58.65%
- META: 109.67%
- WFC: 62.34%

### 2-Year Beta (Pulled from YFinance)
Highest volatility:
- AMD: 3.49 
- GNRC: 2.60
- UIS: 2.58

Negative beta (moves opposite):
- BP: -1.11
- UNH: -0.87
- GILD: -0.77

Market-like:
- WFC: 1.02
- TXN: 1.04

## CSV Files Generated

**Alpha Analysis:**
- `alpha_comprehensive_analysis.csv` - all data for all periods
- `alpha_sorted_by_1y.csv` - stocks ranked by 1Y alpha
- `alpha_sorted_by_2y.csv` - stocks ranked by 2Y alpha
- `alpha_sorted_by_3y.csv` - stocks ranked by 3Y alpha
- `portfolio_original_order_alpha.csv` - complete data in original portfolio order with company names
- `alpha_summary_original_order.csv` - simplified alpha summary in original order
- `quarterly_portfolio_alpha.csv` - quarterly portfolio performance
- `portfolio_summary.csv` - key portfolio metrics summary

**Beta:**
- `beta_2year_sorted_by_value.csv`
- `beta_2year_original_order.csv`


## Usage
To run the analysis:
```python
python portfolio_alpha_analysis.py
