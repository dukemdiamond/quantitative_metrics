# Quantitative Metrics

Portfolio analysis on Quantitative Metrics (Sharpe, Alpha, Beta) for Q1-Q2 2025 with 29 stocks.

## Files

**Sharpe Ratios:**
- `sharpe_ratio_calculator.py` - quarterly sharpe + market bottom performance for entire portfolio

**Alpha Analysis:**
- `alpha_calculator.py` - vs SP500

**Beta Analysis:**  
- `beta_calculator.py` - 2Y volatility vs market

## Results Summary

### Sharpe Ratios
- **Q1-Q2 2025:** -0.12 (underperformed risk-free rate)
- **Market Bottom (Apr-Jul):** 2.82 (recovered)
- **SP500 Q1-Q2:** 0.11 (Outperformed Portfolio in 1H)

### Portfolio Performance
- **Q1 2025:** -7.08%
- **Q2 2025:** 6.84%  
- **Since Market Bottom:** 28.91%
- **Risk-Free Rate:** 4.42% 3 Month Treasury Bill

### Alpha Analysis (Q1-Q2 avg vs SP500)
Best performers:
- GRAL: 37.85%
- KLAC: 13.55%
- META: 8.05%

Worst performers:
- UNH: -33.80%
- ILMN: -27.90%
- UIS: -21.65%

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

## CSV Files 

**Alpha:**
- `alpha_sorted_by_performance.csv`
- `alpha_original_order.csv`
- `alpha_market_bottom_sorted.csv`
- `alpha_market_bottom_original.csv`

**Beta:**
- `beta_2year_sorted_by_value.csv`
- `beta_2year_original_order.csv`

## Key Insights

1. **Recovery was strong** - portfolio sharpe went from -0.12 to 2.82 since market bottom
2. **High beta portfolio** - lots of volatile tech stocks
3. **Some defensive positions** - negative beta stocks like healthcare/energy

## Usage

To run, run each file independently:
```python
python sharpe_ratio_calculator.py
python alpha_calculator.py  
python beta_calculator.py
```

All generate dataframes and save CSV files automatically.

## Portfolio Holdings (29 stocks)
META, REGN, FI, GILD, MITK, FIS, IDCC, COUR, AMAT, KLAC, NICE, WFC, AMD, LLY, NVO, DELL, BP, NOK, RMBS, EL, UIS, ILMN, GOOG, SNPS, GRAL, UNH, GNRC, TXN, ROK

Total portfolio weight: concentrated in top holdings with META at 13.94%
