### Problem Statement

Financial market is variable and full of uncertain factors, which investors always wish to find a right approach either decreasing risk or increasing return. However, the core problem of optimal investment is that how investors can reasonably allocate their existing investable assets to impletment the best return under a certain risk. This is a portfolio optimization that impletment a balance between return rate and risk rate. In this case I want to combine some stocks as a long-term investment, and I need to find a balance point between return and risk, which achieve a maxmum return and a minimum risk.

Skills: Covariance/ Normalization / Correlation Matrix / Data Visualization / Markov Chain Monte Carlo Simulation / Sharpe Ratio
The purpose of this project is to gain an optimal weight distribution with the lowest risk and the highest return by analyzing a stock portfolio.
  - The optimal weights in 10,000 simulations: Apple/0.3638, Amazon/0.3377, Facebook/0.0309, Google/0.0063, Tesla/0.2613.


### Data:
  Data is from Yahoo finance (stocks symbols: AAPL, AMZN, FB, GOOGL, TSLA)
  
  
### Methodology:
  - Stocks price-weighted portfolio
    - The weight bases on the percentage of the price of a stock in the total price of five stocks.
  - Stocks equal-weighted Portfolio
    - The weight for each stock is equal.
  - Stocks value-weighted Portfolio
    - The weight bases on market value of a stock.
  - Optimal Portfolio of Stocks
    - Markov Chain Monte Carlo (MCMC) Simulations
    - Minimum risk portfolio
    - Maxmum return portfolio
    - Optimize portfolio (Max Sharpe Ratio Portfolio)
    - Find a maxmum sharpe ratio portfolio


### EDA:
  - Calculated stocks daily return and year return
  - Calculated stocks daily risk and year risk
  - Stocks correlation analysis
    - Correlation Matrix of Portfolio
    - Covariance Matrix of Portfolio
    - Standard Deviation / Mean of Portfolio


### Data Preprocessing
   Data normalization
   
  
### Conclusions:
  In 10000 weights combination of simulations by MCMC, I find out the best weights of the optimal portfolio is that:
  - AAPL: 0.3638
  - AMZN: 0.3377
  - FB: 0.0309
  - GOOGL: 0.0063
  - TSLA: 0.2613
