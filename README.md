# ApexRisk
Dynamic Portfolio Optimization &amp; Key Portfolio Metrics Analysis

Dynamic Portfolio Optimization vs. Fixed Allocation

A Retrospective Analysis (2014-2024)

Overview
This project presents a retrospective analysis comparing a dynamic, rules-based portfolio optimization strategy to a traditional fixed 60/40 stocks/bonds allocation and the SPY benchmark over the period 2014–2024. Using historical market data and key risk metrics, the goal is to explore how active, monthly rebalancing might enhance risk-adjusted returns compared to a static allocation. It is important to note that this analysis is observational and should not be interpreted as a predictive model or guarantee of future performance.

Key Features
Dynamic Rebalancing:
The model rebalances the portfolio monthly based on asset performance and changing market conditions.

Risk Metrics Calculation:
Implements various measures such as:

Rolling Sharpe Ratio: Evaluates risk-adjusted returns ("bang for your buck").

Rolling Beta: Assesses portfolio sensitivity to market movements.

Drawdown Metrics: Tracks peak-to-trough and maximum drawdowns to gauge portfolio resilience.

Rolling R²: Measures the proportion of return variability explained by the market.

Comparative Analysis:
The project compares the dynamic portfolio's performance with a static 60/40 allocation and the SPY benchmark, highlighting differences during bull markets, bear markets, interest rate hike cycles, and the COVID-19 crash.

Educational Insights:
Derived from key courses at Rutgers Business School such as Financial Econometrics (regression analysis, beta, alpha, Sharpe ratio, and R²) and Fixed Income (yield curves, bond pricing, interest rate dynamics).

Methodology
Data Acquisition:
Historical price data for the specified stocks, bond ETFs, and SPY are downloaded via the yfinance library.

Data Preprocessing:
The data is cleaned (using forward and backward filling) and resampled from daily to monthly returns using pandas.

Dynamic Portfolio Optimization:
The core of the project uses a monthly rebalancing algorithm that optimizes portfolio weights using risk-adjusted return metrics. This dynamic strategy is then compared with a traditional 60/40 portfolio.

Risk Analysis:
A suite of risk measures is computed using libraries like numpy, statsmodels, and scipy. The analysis includes rolling metrics (Sharpe, Beta, R²) and drawdown calculations, with visualizations produced via matplotlib.

Files and Notebooks
DynamicPortfolio_Optimization.ipynb
The main Google Colab Notebook that contains the full project code, from data download and preprocessing, through dynamic portfolio optimization, to risk measure calculations and visualizations.

Additional Files:

Optional Excel export of portfolio weights and metrics.

Supplementary data files (if any).

Dependencies
Python 3.x

numpy

pandas

yfinance

scipy

statsmodels

matplotlib

tqdm

These can be installed via pip:

bash
Copy
pip install numpy pandas yfinance scipy statsmodels matplotlib tqdm
How to Run the Project
Open the Notebook:
Upload or open the DynamicPortfolio_Optimization.ipynb notebook in Google Colab.

Install Dependencies:
Ensure that the required libraries are installed. You can run the installation commands in a Colab cell if needed.

Run All Cells:
Execute the notebook cells sequentially to download the data, perform portfolio optimization, compute risk metrics, and generate the visualizations.

Explore the Results:
The notebook produces charts that compare the dynamic portfolio with the traditional 60/40 portfolio and the SPY benchmark under various market regimes.

Disclaimer
This project is a retrospective observational study based on historical data and simulated scenarios. The results are meant to provide insights into risk management strategies and do not predict future performance.

Contact & Collaboration
If you have any questions, feedback, or would like to collaborate, please feel free to contact me via LinkedIn @ https://www.linkedin.com/in/darienramirez/ or email at dvr26@scarletmail.rutgers.edu.
