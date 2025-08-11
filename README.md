# Euronext Factor Screener

**Goal:** Build momentum/volatility factors for Euronext stocks and run a **monthly top-N** backtest versus buy-and-hold.  
**Status:** Scaffold — code will be added incrementally (ingestion → factors → backtest → dashboard).

## Tech stack (planned)
Python (pandas, numpy, yfinance, matplotlib) · YAML config

## Structure (planned)
data/ (tickers.csv, prices/ cache) · notebooks/ · screener/ · backtest/ · scripts/ · img/

## Getting started (as code lands)
1) `pip install -r requirements.txt`  
2) Put symbols in `data/tickers.csv` (e.g., `AIR.PA`, `OR.PA`)  
3) Run scripts in `scripts/` (to be added)

## Roadmap
- [ ] Data ingestion + cache
- [ ] Factor table (mom 1/3/12m, vol)
- [ ] Strategy: monthly top-N (equal-weight)
- [ ] Metrics: CAGR, MaxDD, Sharpe + equity curve CSV
- [ ] Benchmark & basic transaction cost
- [ ] (Optional) Streamlit mini-dashboard

## License
MIT
