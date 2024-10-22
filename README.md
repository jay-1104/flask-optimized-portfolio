# Flask Optimized Portfolio API

This repository contains a Flask-based API that optimizes stock portfolios using K-Means clustering and Efficient Frontier optimization techniques. It allows users to retrieve an optimized stock portfolio for a given month and year by analyzing historical data.

## Features
- **K-Means Clustering**: Groups stocks based on features such as RSI to select high-momentum stocks.
- **Efficient Frontier Optimization**: Maximizes the Sharpe ratio by optimizing stock weights using historical data.
- **Factor Betas**: Incorporates rolling factor betas (e.g., Fama-French) to estimate stock exposures.
- **Diversification Constraints**: Imposes weight limits on individual stocks to ensure diversification.

## Technologies
- **Flask**: For building the API.
- **Pandas**: For data manipulation.
- **PyPortfolioOpt**: For financial portfolio optimization.
- **Scikit-learn**: For K-Means clustering.

