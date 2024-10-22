# Stock Portfolio Optimization with K-Means and Efficient Frontier

This repository implements a stock portfolio optimization model that leverages **K-Means Clustering** and the **Efficient Frontier** approach. The aim is to optimize stock portfolios by grouping assets based on their features and then optimizing portfolio weights to maximize the Sharpe ratio.

## Key Features
- **K-Means Clustering**: Group stocks based on various features (e.g., RSI) to capture momentum patterns and select stocks with high potential for the next period.
- **Efficient Frontier Optimization**: Use PyPortfolioOpt to optimize the portfolio weights, maximizing returns for a given level of risk by maximizing the Sharpe ratio.
- **Rolling Factor Betas**: Incorporate Fama-French factor models (e.g., market risk, size, value) to estimate stock exposure to key risk factors over time.
- **Diversification Constraints**: Set weight limits on individual stocks to ensure that portfolios are diversified and not overly concentrated in a few assets.

## Clustering and Portfolio Strategy
1. **K-Means Clustering**: 
    - Each month, stocks are grouped into clusters based on their RSI (Relative Strength Index) and other key financial metrics.
    - The model initializes predefined centroids for clustering to target high-momentum stocks (e.g., those clustered around RSI 70).
  
2. **Portfolio Construction**:
    - After clustering, stocks from the most desirable cluster (e.g., high momentum) are selected to form the portfolio for the next month.
    - The Efficient Frontier method is applied to calculate the optimal weights for each stock, balancing risk and return.

3. **Sharpe Ratio Maximization**:
    - The portfolio weights are optimized to maximize the Sharpe ratio, ensuring the highest possible return for the least amount of risk.
