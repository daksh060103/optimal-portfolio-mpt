This project builds a Python-based script to generate an optimal stock portfolio using Modern Portfolio Theory (MPT) and mean-variance optimization.
Pulls live stock data from NSE using yfinance.

Calculates daily returns and covariance matrix.

Optimizes portfolio weights to maximize Sharpe Ratio.

Applies constraints:

Total weights sum to 1.

Individual stock weight between 0% and 60%.

**Outputs:**

Optimalweights.
Expected portfolio return (annualized).
Portfolio volatility (annualized).
Maximum Sharpe Ratio.

**Technologies Used:**
Python 3
pandas
NumPy
SciPy
yfinance

**How It Works:**

Select Stocks → List of NSE stock tickers.
Download Data → Fetch historical prices from Yahoo Finance.\
Calculate Returns & Covariance → Based on daily price movements.
Optimize Portfolio → Using scipy.optimize.minimize with constraints.
Display Results → Best weights, expected return, risk, Sharpe ratio.

Future inprovements:
Can add an efficent frontier to visalise the portfolio with CML or indifference curve .
Create a stock optimizer that can select stocks according to various stats we provide like low correlation, sharpe ratio for ranking.



