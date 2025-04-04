## Financial Analysis Tools

This package provides a comprehensive set of tools for financial analysis and portfolio management. It includes various metrics, ratios, and models commonly used in quantitative finance.

### Features

- **Performance Metrics**
  - Adjusted Sharpe Ratio
  - Annual Return
  - Average Return
  - Calmar Ratio
  - Double Sharpe Ratio
  - Modified Sharpe Ratio
  - Sharpe Ratio
  - Sortino Ratio
  - Treynor Ratio

- **Risk Measures**
  - Conditional Value at Risk (CVaR)
  - Value at Risk (VaR)
  - Portfolio Volatility

- **Market Models**
  - Capital Asset Pricing Model (CAPM)
  - Fama-French Three-Factor Model

- **Technical Indicators**
  - Relative Strength Index (RSI)
  - Momentum

- **Portfolio Analysis**
  - Benchmarking
  - Correlation with Index
  - Intraweek Variances
  - Market Alpha
  - Market Beta

- **Backtesting**
  - SeffyBacktest: A custom backtesting framework

### Usage

Every file in /modules is an indicator that can be used alone except for:

benchmarking.py -> A program that allows you to compare your portfolio to various different indexes at the same time. It is currently configured to 5 indexes to chose from and 4 indicators as standard. This is not used in seffybacktest.py

get_portfolio_returns.py -> This allows you to pass in the tickers, weights, start_date and end_date of your portfolio, if you do not have a csv file already prepared. The output of this can be direclty passed in to the seffybacktest from seffybacktest.py to perform whatever analysis you desire.

seffybacktest.py ->The `seffybacktest.py` script is a comprehensive portfolio analysis tool that offers a user-friendly interface for evaluating investment strategies. It integrates various financial indicators and metrics, including Sharpe ratio, CAPM, Fama-French factors, and momentum analysis, allowing users to select specific indicators for their portfolio evaluation. The script utilizes popular Python libraries such as yfinance for data retrieval, matplotlib for visualization, and tkinter for creating an interactive GUI. It provides flexibility in input parameters, such as risk-free rates and market indices, and offers options for annualizing volatility and plotting momentum and RSI graphs. The tool calculates selected indicators, displays results in a clear tabular format, and generates visual representations when applicable. With its modular design and extensive range of financial metrics, `seffybacktest.py` serves as a valuable resource for investors and financial analysts seeking to conduct thorough portfolio performance assessments.

### Dependencies

python = "^3.12"
numpy = "^2.0.0"
pandas = "^2.2.2"
scipy = "^1.14.0"
yfinance = "^0.2.40"
DateTime = "^5.5"
sklearn = "^0.0.post12"
matplotlib = "^3.9.1"

### License

MIT Lisence

### Disclaimer

These tools are for educational and research purposes only. Always consult with a qualified financial advisor before making investment decisions. 