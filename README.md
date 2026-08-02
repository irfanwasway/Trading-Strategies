# Trading Strategies
Backtesting and evaluation of systematic trading strategies covering single-asset momentum with volatility targeting and statistical arbitrage via cointegration.

## Overview
This project implements two kinds of strategies from first principles:
1. **Multi-horizon momentum with volatility targeting**: trend-following on **SPY**, improved from an initial naive binary signal to a volatility-scaled blend of multiple lookback horizons.
2. **Statistical arbitrage/pairs trading**: screened asset pairs for cointegration using Engle-Granger two-step methodology, which utilises the Augmented Dickey-Fuller test. Traded via a Z-score mean-reversion rule on the price spread.

Both strategies are backtested with fricion (modelled with 5 basis points) and evaluated on CAGR, annualised volatility, Sharpe ratio, and maximum drawdown to try to assess a strategy's risk-adjusted efficiency rather than raw cumulative return alone.

## Tech Stack
Python; pandas; NumPy; statsmodels(ADF,OLS); matplotlib; yfinance
