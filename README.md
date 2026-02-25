# oil-returns-volatility-risk
This repository contains a Jupyter notebook that analyzes **Brent crude oil prices from 2017-01-01 to 2025-12-01, focusing on returns, volatility clustering, distributional fit, and risk metrics such as Value at Risk (VaR) and Expected Shortfall (ES)

# Brent Crude Oil Volatility & Risk Modeling (GARCH, VaR, Expected Shortfall)

This repository contains a Jupyter notebook that analyzes **Brent crude
oil prices** (Yahoo Finance ticker **`BZ=F`**) from **2017-01-01 to
2025-12-01**, focusing on **returns, volatility clustering,
distributional fit**, and **risk metrics** such as **Value at Risk
(VaR)** and **Expected Shortfall (ES)**.

Notebook: `project2.ipynb`

------------------------------------------------------------------------

## What's inside

-   **Data acquisition**
    -   Download daily Brent crude prices via `yfinance` (`BZ=F`)
    -   Compute log returns
-   **Exploratory analysis**
    -   Descriptive statistics (skewness, kurtosis, normality tests)
    -   ACF/PACF inspection on returns
-   **Distribution fitting**
    -   Fit and compare **Normal** vs **Student-t** distributions for
        returns
-   **Volatility modeling**
    -   GARCH-family modeling using the `arch` library
    -   Conditional volatility visualization
    -   Residual diagnostics
-   **Risk modeling**
    -   Parametric **Value at Risk (VaR)**
    -   **Expected Shortfall (ES)**
    -   Time-varying (dynamic) risk via volatility forecasts

------------------------------------------------------------------------

## Data

The notebook pulls data directly from Yahoo Finance using:

-   **Ticker:** `BZ=F` (Brent Crude Oil)
-   **Range:** 2017-01-01 to 2025-12-01

No dataset files are committed---running the notebook will fetch the
data online.

------------------------------------------------------------------------

## Getting started

### 1) Create an environment

``` bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -U pip
```

### 2) Install dependencies

``` bash
pip install numpy pandas matplotlib seaborn scipy statsmodels yfinance arch jupyter
```

------------------------------------------------------------------------

## Suggested repository structure

    .
    ├── project2.ipynb
    ├── README.md
    └── .gitignore

------------------------------------------------------------------------

## License

This project is licensed under the **MIT License**.

You are free to: - Use - Modify - Distribute - Commercially use

As long as you include the original copyright and license notice.

A copy of the MIT License should be included in a `LICENSE` file at the
root of the repository.
