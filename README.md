#  Multi-Currency Crypto Price Forecasting  
**Forecasting BTC, ETH, and SOL prices using ARIMA & SARIMAX Time Series Models**

---

##  Overview

This project forecasts the monthly closing prices of three major cryptocurrencies — **Bitcoin (BTC)**, **Ethereum (ETH)**, and **Solana (SOL)** — using classical time series models: **ARIMA** and **SARIMAX**. The models are evaluated using RMSE and MAE metrics, with forecasts projected 6 months into the future.

---

##  Features

-  Fetches historical price data directly from the **Binance API**
-  Applies **Box-Cox transformation** for variance stabilization
-  Builds ARIMA and SARIMAX models for each currency
-  Evaluates models using **RMSE** and **MAE**
-  Forecasts future prices for the next **6 months**
-  Visualizes actual vs predicted prices with clean plots

---

##  Tech Stack

- Python 3.x  
- `pandas`, `numpy`, `matplotlib`  
- `statsmodels`, `scikit-learn`, `scipy`  
- `python-binance` (for live crypto data)

---

##  Project Structure

```
crypto-forecast/
│
├── data/
│   ├── btc_binance_ohlcv.csv
│   ├── eth_binance_ohlcv.csv
│   └── sol_binance_ohlcv.csv
│
├── models/
│   └── (optional saved models)
│
├── notebooks/
│   └── crypto_forecast.ipynb
│
├── requirements.txt
└── README.md
```

---

##  Setup Instructions

1. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```


2. **Or use the Jupyter notebook** for interactive modeling.

---

##  Results Summary

| Asset    | Model   | RMSE       | MAE        |
|----------|---------|------------|------------|
| BTC      | SARIMAX | (value)    | (value)    |
| ETH      | SARIMAX | (value)    | (value)    |
| SOL      | SARIMAX | (value)    | (value)    |

> SARIMAX consistently outperformed ARIMA, especially in capturing seasonal price trends across all three currencies.

---

##  Future Work

- Add support for more cryptocurrencies (ADA, XRP, etc.)
- Integrate external features (on-chain data, news sentiment)
- Deploy as a real-time **Streamlit dashboard**
- Explore **LSTM/Transformer-based** forecasting

---

##  References

- [Box-Cox Transformation](https://en.wikipedia.org/wiki/Power_transform#Box%E2%80%93Cox_tansformation)  
- [ARIMA vs SARIMA](https://www.statsmodels.org/stable/tsa.html)  
- [Binance API Docs](https://github.com/sammchardy/python-binance)

---

##  Contact

**Author:** Aarush Garg  
**Email:** aarush.garg2305@gmail.com
**GitHub:** [https://github.com/aarush23g]