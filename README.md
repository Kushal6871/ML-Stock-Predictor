# NVDA Stock Return Predictor

A machine learning project exploring whether an LSTM neural network can predict NVIDIA (NVDA) stock returns over the next five trading days.

## About the Project

I built this project to learn how LSTM neural networks can be used for stock market time-series forecasting. I used historical NVIDIA stock data and technical indicators to predict its cumulative return over the next five trading days.

## Methodology

- **Model:** LSTM neural network built with PyTorch
- **Input window:** Previous 60 trading days
- **Features:** Seven technical and historical features
- **Target:** Cumulative return over the next five trading days
- **Data splitting:** Chronological training, validation, and test sets
- **Scaling:** StandardScaler fitted on training data
- **Baseline:** Predicting a zero return

## Results

| Model | Test L1 Loss |
|:--|--:|
| Zero-return baseline | 0.6032 |
| LSTM | 0.5737 |

The LSTM achieved approximately **4.9% lower test loss** than the zero-return baseline in this experiment.

This is a modest improvement and does not establish that the model can reliably predict stock returns or generate profitable trades.

## What I Learned

Through this project, I gained experience with time-series data, feature engineering, data scaling, LSTM neural networks, and evaluating a model against a baseline.

I also learned that training a model successfully is different from demonstrating that it makes useful predictions.

## Limitations

- Stock returns are noisy and difficult to forecast.
- Results may vary across different time periods and market conditions.
- Further tuning is needed to determine whether the predictions are accurate.
- The profitability of a trading strategy has not been established.
