# Portfolio-Optimization-

## Overview
This project demonstrates portfolio optimization proficiency through Monte Carlo simulation. It identifies optimal asset allocations based on the Sharpe ratio, helping balance expected returns and risk.

## Features of the program

### Data Processing
- Imports and processes stock price data from CSV files
- Calculates percentage daily returns
- Scales prices for comparative analysis
- Generates correlation heatmaps for asset relationships

### Portfolio Construction
- Generates random portfolio weights 
- Allocates investment amounts across multiple assets
- Tracks portfolio value over time
- Calculates portfolio returns and volatility

### Optimization
- Runs Monte Carlo simulations to generate thousands of portfolio configurations
- Calculates key metrics for each portfolio:
  - Expected annual return
  - Portfolio volatility (standard deviation)
  - Sharpe ratio (risk-adjusted return)
  - Final portfolio value
  - Return on investment percentage

### Visualization
- Displays adjusted closing prices over time
- Plots percentage daily returns
- Creates histograms of return distributions
- Generates correlation heatmaps
- Visualizes the efficient frontier
- Highlights optimal portfolio allocations
- Shows portfolio performance over time


### Prerequisites
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- plotly

## Key Functions

### `price_scaling(raw_prices)`
Scales all asset prices relative to their starting value for comparative analysis.

### `generate_weights(n)`
Generates random portfolio weights for n assets that sum to 1.

### `asset_allocation(df, weights, initial_investment)`
Allocates investment across assets according to specified weights and tracks portfolio performance.

### `simulation_engine1(weights, initial_investment)`
Calculates portfolio metrics including expected return, volatility, Sharpe ratio, and final value.

## Future Development
Future versions aim to incorporate machine learning algorithms to provide predictive capabilities, potentially enabling:
- Time series forecasting of asset prices
- Optimization based on predicted future performance
- Risk assessment under various market scenarios
- Anomaly detection for portfolio rebalancing triggers

## Limitations
- The tool currently uses historical data only without predictive capabilities
- Monte Carlo simulations assume normal distribution of returns
- The optimization is based solely on the Sharpe ratio without considering other factors such as the Sortino, Treynor, Jensen's Alpha, and M2
- No transaction costs or taxes are included in the calculations

## Output
The tool generates visualizations of the efficient frontier, highlighting the optimal portfolio based on the Sharpe ratio. It provides detailed metrics for the optimal portfolio including expected annual return, volatility, Sharpe ratio, final value, and return on investment.
