# Stock Market Predictor

This project explores the use of **Long Short-Term Memory (LSTM)** neural networks for forecasting stock prices from historical market data. The model is trained on closing prices retrieved through the Yahoo Finance API and demonstrates how recurrent neural networks can identify temporal patterns in financial time series.

## Features

- Retrieves historical stock market data using Yahoo Finance
- Normalizes and preprocesses time-series data
- Trains an LSTM model using TensorFlow/Keras
- Predicts stock prices on unseen data
- Visualizes actual and predicted prices for comparison
- Forecasts future trading-day closing prices

## Technologies

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- yfinance

## Installation

Clone the repository:

```bash
git clone https://github.com/Vrukshav-Viswanath/Stock-Market-Predictor.git
cd Stock-Market-Predictor
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `stock_market_predictor.ipynb` and run the notebook.

## Methodology

The workflow follows a typical deep learning pipeline for time-series forecasting:

1. Download historical stock data.
2. Normalize closing prices using MinMaxScaler.
3. Convert the data into sequential training windows.
4. Train an LSTM neural network on historical price sequences.
5. Generate predictions on unseen data.
6. Compare predictions with actual market prices through visualization.
7. Forecast future closing prices.

## Results

The trained model captures general price trends and demonstrates the effectiveness of LSTM networks for sequential data. Although the predictions follow market behavior reasonably well, stock prices are influenced by countless external factors that cannot be inferred solely from historical prices. Consequently, the model should be viewed as a demonstration of deep learning techniques rather than a reliable financial forecasting system.

## Future Improvements

Potential enhancements include:

- Incorporating technical indicators (RSI, MACD, Bollinger Bands)
- Hyperparameter optimization
- Multi-feature input (volume, highs, lows, moving averages)
- Support for forecasting multiple stocks
- Comparison with Transformer and GRU architectures

## Disclaimer

This project was developed for educational purposes to explore deep learning and time-series forecasting. It should not be used as financial or investment advice.
