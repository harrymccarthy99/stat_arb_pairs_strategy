#### Statistical Arbitrage Pairs Trading Strategy

This notebook explores how to exploit **forecasted pricing inefficiencies** between two stocks

The stocks included in this study are Ford and General Motors - two american automotive manufacturing companies. Given this similarity, it seems reasonable to expect a **stationary** relationship between the two stocks may exist.

I investigate this in the notebook and find that the **log returns** of the two stocks are indeed cointegrated

To this end, I find a **stationary spread** between the two stocks and implement a mean reverting trading strategy.

Trade entry here is determined by the daily returns of the spread exceeding **two standard deviations** based on training data

The strategy is backtested on the data from 02/01/2023 - 01/06/2024. **Cumulative returns**, **Sharpe ratio**, **max drawdown** and **number of trades** are all returned.
