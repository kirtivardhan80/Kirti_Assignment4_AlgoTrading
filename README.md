# Algo-Trading Prototype with Logistic Regression

An end-to-end algorithmic trading system that combines rule-based
technical analysis with machine learning to generate buy/sell
signals for NIFTY 50 stocks, with automated logging and alerts.

## Overview
- **Strategy**: RSI(14) + SMA(20/50) Crossover
- **ML Model**: Logistic Regression for next-day price prediction
- **Stocks**: YESBANK, IRCTC, ETERNAL
- **Automation**: Google Sheets logging + Telegram alerts

## Project Structure
| File/Folder | Description |
|--------------|-------------|
| `AlgoTrading.ipynb` | Full Jupyter notebook with all code |
| `outputs/` | Charts, dashboards, and visualizations |
| `data/` | CSV datasets and trade logs |
| `report/` | Final PDF report |

## Features
- Fetches 2 years of historical data via yfinance
- RSI + SMA crossover trading strategy with 6-month backtest
- Logistic Regression model (Accuracy, Precision, Recall, F1)
- Real-time Google Sheets trade logging
- Telegram bot notifications for buy/sell signals
- Interactive visualization dashboards

## Results Summary
| Stock | Trades | Win Rate | ML Accuracy |
|-------|--------|----------|--------------|
| YESBANK | 2 | 50% | 53% |
| IRCTC | 1 | 0% | 56% |
| ETERNAL | 1 | 0% | 41% |

## Tech Stack
Python, Pandas, NumPy, Scikit-learn, yfinance, gspread,
Matplotlib, Telegram Bot API

## Setup
1. Install dependencies: `pip install yfinance pandas numpy scikit-learn gspread matplotlib requests`
2. Add your own `credentials.json` for Google Sheets API
3. Update `BOT_TOKEN`, `CHAT_ID`, `SHEET_ID` in the notebook
4. Run `run_algo_trading(tickers=tickers)`

## Author
Kirti vardhan singh
