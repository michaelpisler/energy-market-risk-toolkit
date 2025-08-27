# Energy Market Risk Toolkit (MySQL + Python)
Full package with SQL, data, scripts, and CVs.
# Energy Market Risk Toolkit

This repository contains a **practical risk analytics demo** for energy/commodity trading portfolios.  
It demonstrates **SQL + Python** skills for a Market Risk Analyst role.

## Features
- Load and manage trade, market curve, and FX data.
- Store data in **SQLite** (default) so the notebook runs anywhere.  
  - Optional: switch to **MySQL** by changing one line in `MySQL_Risk_Demo.ipynb`.
- Compute:
  - Open positions (as-of date snapshot)
  - Portfolio P&L attribution
  - Historical & parametric Value-at-Risk (VaR)
  - Daily price P&L
- Visualize P&L time series and distributions.

## How to Run
1. Clone this repo:
   ```bash
   git clone https://github.com/michaelpisler/energy-market-risk-toolkit.git
   cd energy-market-risk-toolkit
# Energy Market Risk Toolkit

This repository contains a **practical risk analytics demo** for energy/commodity trading portfolios.  
It demonstrates **SQL + Python** skills for a Market Risk Analyst role.

## Features
- Load and manage trade, market curve, and FX data.
- Store data in **SQLite** (default) so the notebook runs anywhere.  
  - Optional: switch to **MySQL** by changing one line in `MySQL_Risk_Demo.ipynb`.
- Compute:
  - Open positions (as-of date snapshot)
  - Portfolio P&L attribution
  - Historical & parametric Value-at-Risk (VaR)
  - Daily price P&L
- Visualize P&L time series and distributions.

## How to Run
1. Clone this repo:
   ```bash
   git clone https://github.com/michaelpisler/energy-market-risk-toolkit.git
   cd energy-market-risk-toolkit
Install requirements (Python 3.9+ recommended):
Install requirements (Python 3.9+ recommended):

pip install -r requirements.txt


Launch Jupyter:

jupyter lab


Open and run MySQL_Risk_Demo.ipynb.

Database Setup

By default the notebook uses SQLite (energy_risk.sqlite) so it works out of the box.

To use MySQL instead (requires local DB setup):

from sqlalchemy import create_engine
eng = create_engine("mysql+pymysql://root:root@localhost:3306/energy_risk", future=True)


Schema and seed data are in the sql/
 folder.

Data

data/trades.csv → trade details

data/curve_prices.csv → forward curves

data/fx_rates.csv → FX rates

Example Output

Positions snapshot

P&L time series

Historical & parametric VaR

Daily price P&L


This project demonstrates practical SQL + Python risk analytics for energy/commodity portfolios.