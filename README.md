# Stock Market Analysis — FTSE 100 & S&P 500

Python financial time-series analysis of the FTSE 100 and S&P 500 indices: risk modelling, co-integration testing, and GARCH volatility forecasting.

## Key Findings

> Replace bracketed values with your actual results.

- **Stationarity:** price levels [non-stationary] (ADF p = [value]); log returns stationary (ADF p = [value]).
- **Co-integration:** Engle–Granger test [did/did not] find a long-run relationship (p = [value]).
- **Systematic risk:** beta = [value]; Jensen's alpha = [value].
- **Volatility:** GARCH(1,1) persistence α + β = [value], confirming volatility clustering.
- **Distribution:** returns non-normal (Jarque–Bera p = [value]), with fat tails.

## Methods

- Data cleaning and daily log-return computation
- Descriptive statistics and Jarque–Bera normality test
- Beta and Jensen's alpha via CAPM (OLS regression)
- ACF/PACF plots and Augmented Dickey–Fuller tests
- Engle–Granger co-integration test
- ARCH(1) and GARCH(1,1) volatility models

## Structure

```
proiect_python.py   Main analysis script
FTSE100_data.csv    FTSE 100 historical prices
SP500_data.csv      S&P 500 historical prices
```

## Setup

```sh
pip install pandas numpy matplotlib statsmodels arch scipy
git clone https://github.com/aariton/FTSE100_SP500_project.git
cd FTSE100_SP500_project
python proiect_python.py
```

**Author:** Alexandru Ariton
