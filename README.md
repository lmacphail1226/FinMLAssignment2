# FinMLAssignment2

## Description
Assignment 2 is a Monte Carlo Simulation of a portfolio of stocks over a 5 year period with the mean and standard deviation of the portfolio returns. 
1000 simulations were used with random weights assigned to each stock denoting if we were long or short on the stock. 
The results show a comparison of a portfolio allowing for shorts and longs vs. just longs 
DraftKings (DKNG), FanDuel (FLUT), and MGM Sports (MGM) stocks were used as the stocks for this simulation

## How to Use
The following modules were used in the Jupyter Notebook and will be required to be able to run the notebook.
* numpy: 1.26.4
* pyarrow: 17.0.0
* polars: 1.31.0
* seaborn: 0.13.2
* yfinance: 0.2.64

The Notebook will execute 4 different models (Logistic, SVM, XGBoost, and Light GBM) starting with a baseline model and then using a randomized search to find the optimal hyperparameters. The notebook is set up with the correct hyperparameters given the random state selected (2025), but hyperparameters may need to be updated if the random state is updated
The Notebook will download the selected stocks in the specific date range specified in the beginning portion and then run the simulation. The notebook is seeded to replicate the results

Final output is a scatter plot of the mean returns vs. standard deviation of the returns for a portfolio with longs and shorts vs. just shorts.
