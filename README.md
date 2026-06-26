# Portfolio Optimisation and Bollinger Bands Backtest

This project builds and evaluates a 10-stock equity portfolio using historical Yahoo Finance data from 2020 to 2025. It backtests a Bollinger Bands Mean Reversion strategy, compares the strategy against buy-and-hold returns, and optimises the portfolio using both a Sharpe Ratio optimiser and an AI-generated downside-aware optimiser.

## Project Description

The notebook approaches the task from the perspective of a portfolio manager setting up a new equity portfolio. It selects ten actively traded US stocks, retrieves six years of historical data with `yfinance`, cleans and validates the dataset, explores price behaviour, tests a rules-based mean reversion strategy, and compares portfolio allocations on a like-for-like return basis.

The final recommendation is based on risk-adjusted performance, drawdown behaviour, concentration risk, and whether the Bollinger strategy adds value for each stock.

## Contents

- `Assessment2.ipynb` - main executed Jupyter Notebook with code, charts, analysis, and final report.
- `outputs/Assessment2.ipynb` - copy of the final notebook for sharing.
- `outputs/Assessment2.html` - HTML export for submission or easy viewing.
- `work/` - helper scripts and intermediate files used to generate and verify the notebook.

## Methods Used

- Yahoo Finance data retrieval with `yfinance`
- Data cleaning and missing-value checks with `pandas`
- Closing-price exploration and visualisation
- Bollinger Bands Mean Reversion backtest
- Equal-weight portfolio construction
- Correlation analysis of simple daily returns
- Sharpe Ratio portfolio optimisation with `scipy.optimize.minimize`
- AI-generated downside-aware portfolio optimisation
- Final investment recommendation with in-text citations and reference list

## Stocks Analysed

The portfolio uses ten large-cap US equities:

`AAPL`, `MSFT`, `AMZN`, `GOOGL`, `META`, `NVDA`, `JPM`, `XOM`, `UNH`, `COST`

## How to View

For GitHub, open:

```text
Assessment2.ipynb
```

For a rendered submission-style version, open:

```text
outputs/Assessment2.html
```

## Requirements

The main Python packages are:

```text
pandas
numpy
matplotlib
seaborn
scipy
yfinance
ipython
```

If running locally, install the requirements with:

```bash
pip install pandas numpy matplotlib seaborn scipy yfinance ipython
```

## Note

This project is for educational analysis only. It is not financial advice, and historical backtest results should not be interpreted as a guarantee of future investment performance.
