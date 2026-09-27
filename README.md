# Microsoft Stock Price Prediction

A small machine learning project that uses a Decision Tree Regressor to predict
Microsoft (MSFT) stock closing prices from the day's Open, High, and Low prices.

## What it does

1. Loads historical MSFT price data (`MSFT.csv`, Dec 2021 – Dec 2022).
2. Plots the closing price over time.
3. Shows a correlation heatmap between Open, High, Low, Close, Adj Close, and Volume.
4. Trains a `DecisionTreeRegressor` on Open/High/Low to predict Close.
5. Builds a small comparison table of predicted vs. real prices with an accuracy %.

## Data

`MSFT.csv` — daily MSFT OHLCV data from Yahoo Finance, covering
2021-12-27 through 2022-12-19.

## Requirements

```
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Usage

```
python Microsoft_Stock_Price_Prediction.py
```

The script will display three plots in sequence (close the window to continue
to the next one): the price chart, the correlation heatmap, and the
prediction comparison table.

## Notes

- The "real values" table near the end is illustrative: it pairs the first
  five predictions from the (shuffled) test set with five real closing
  prices looked up separately, rather than being a strict row-by-row match.
- Built as a learning project exploring basic regression on financial time
  series data.
