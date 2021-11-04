# Augmented Factor Investing with Reinforcement Learning

### Introduction

Portfolio optimization has been a main concern in financial industry for a long time and nowadays, there are many popular theories can be applied to perform portfolio optimization. In this project, our team combined the augmented fundamentals factors such as momentum with both the Markowitz framework and reinforcement learning to perform portfolio optimization on selected stocks. We also compared the performance of these methods by backtesting in year 2019 based on different measures, such as, annualized Sharpe ratio, maximum drawdown etc.

### Data and training period

Our team selected the following 20 large capitalization stocks from the Standard & Poor 500 index with respect to their market capitalization and obtained their stock price information from Yahoo! Finance [linked here](https://finance.yahoo.com/).

| Ticker |	Company Name |	Ticker |	Company Name |
| ------- | --------- | ------- | ------------------ |
| AAPL |	Apple Inc. |	CMCSA |	Comcast Corporation Class A |
| MSFT |	Microsoft Corporation |	XOM |	Exxon Mobil Corporation |
| AMZN |	Amazon.com Inc. |	ADBE |	Adobe Inc. |
| GOOG |	Alphabet Inc. Class C |	VZ |	Verizon Communications Inc. |
| JNJ |	Johnson & Johnson |	INTC |	Intel Corporation |
| UNH |	UnitedHealth Group Incorporated |	PFE |	Pizer Inc. |
| V |	Visa Inc. Class A |	CSCO |	Cisco Systems Inc. |
| NVDA |	NVIDIA Corporation |	NFLX |	Netix Inc. |
| PG |	Procter & Gamble Company |	KO |	Coca-Cola Company |
| MA |	Mastercard Incorporated Class A |	T |	AT&T Inc. |

The portfolio optimization was performed from 2011 to 2019 to avoid the pandemic influence in 2020.

The company's quarter fundamental data can be acquired from SimFin [linked here](https://simfin.com/data/bulk).

### Conclusion

The result is quite clear that the optimal portfolio selected by reinforcement learning outperforms that from the traditional Markowitz framework. Backtested the optimized portfolio in year 2019 with weights adjusted quarterly and record the daily return. Obtained the annualized return approximately as 28.22% and annualized Sharpe ratio as 1.94; the annualized volatility approximately as 13.28%.

For future work, this project can be extended to select optimal portfolios of the mid and small capitalization stocks. We also noticed that the optimization setup might be out-of-control during the pandemic in 2020, so the model sensitivity is another direction for improvement.

- Here, the Python code accounts for porfolio optimization with factor model and Markowitz optimization part (collabroated with Cornell student Rui Dai (rd576@cornell.edu)).
