# Predicting Bitcoin Prices Using Machine Learning Models

## Overview
This project explores the performance of three machine learning models—Linear Regression, Random Forest Regressor, and LSTM (Long Short-Term Memory)—in predicting the price of Bitcoin. The goal is to understand how these models handle the volatility and complex patterns in Bitcoin’s price using historical data collected from Yahoo Finance.

### Research Question
How do different machine learning models perform in predicting the price of Bitcoin, and what factors contribute to their varying performance?

## Abstract
This study compares the performance of three machine learning models—Linear Regression, Random Forest, and Long Short-Term Memory (LSTM) networks—in predicting Bitcoin prices. Linear Regression served as a baseline model, delivering strong results with a Mean Absolute Error (MAE) of 1181.13, Root Mean Squared Error (RMSE) of 1754.55, and R-squared (R²) value of 0.9931. Random Forest, although successful in identifying feature importance, such as the 5-day moving average, showed lower overall accuracy, with MAE of 3888.63, RMSE of 8717.58, and R² of 0.8286. LSTM networks, designed for time-series forecasting, excelled in capturing Bitcoin’s volatility and temporal dynamics, with an MAE of 1456.71, RMSE of 2087.55, and R² of 0.9903. The study also included 30-day future price predictions, where Linear Regression provided smooth, trend-aligned forecasts, Random Forest showed more variability, and LSTM balanced trend consistency with capturing fluctuations. These findings highlight that while Linear Regression is computationally efficient, LSTM is the most effective for dynamic, volatile financial markets.


## Results
### Model Performance Metrics
| Model               | MAE     | RMSE    | R²       |
|---------------------|---------|---------|-----------|
| Linear Regression   | 1181.13 | 1754.55 | 0.9931    |
| Random Forest       | 3888.63 | 8717.58 | 0.8286    |
| LSTM                | 1456.71 | 2087.55 | 0.9903    |

### 30-Day Future Predictions
- **Linear Regression**: Produced smooth and trend-aligned forecasts, suitable for identifying general price movements.
- **Random Forest**: Exhibited variability in predictions, reflecting its sensitivity to feature interactions and noise.
- **LSTM**: Balanced trend consistency with an ability to capture market fluctuations, making it well-suited for volatile conditions.

---

## Aims
This project aims to:
- Compare the effectiveness of Linear Regression, Random Forest Regressor, and LSTM models in predicting Bitcoin prices.
- Analyze model performance through metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² score.

## Objectives
1. **Data Collection**: Gather historical Bitcoin price data and generate additional features such as moving averages, volatility, and daily returns.
2. **Model Training**: Train and test Linear Regression, Random Forest Regressor, and LSTM models on the dataset.
3. **Model Evaluation**: Evaluate the models using MAE, RMSE, and R² score.
4. **Analysis**: Analyze the strengths and weaknesses of each model in capturing trends, volatility, and patterns in Bitcoin prices.

---

## Background
Bitcoin, the most prominent cryptocurrency, has experienced massive price fluctuations influenced by macroeconomic conditions, regulatory news, and market speculation. Predicting Bitcoin prices is challenging due to its inherent volatility, but machine learning models provide promising tools for financial forecasting.

### Why These Models?
- **Linear Regression**: A simple, interpretable model for establishing a baseline prediction based on linear relationships between features.
- **Random Forest Regressor**: An ensemble method ideal for handling nonlinearities and feature interactions in noisy financial data.
- **LSTM**: A recurrent neural network well-suited for time series data, capable of learning from temporal dependencies.

---

## Data Collection
### Data Source
The dataset is sourced using the `yfinance` Python API and includes:
- Historical Bitcoin price data (daily open, close, high, low, and volume).
- Additional features:
  - Moving averages (e.g., 5-day, 10-day, 50-day).
  - Daily returns (percentage change in closing price).
  - Volatility (calculated using rolling standard deviation of returns).

---

## Usage
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the scripts to:
   - Prepare the dataset.
   - Train the machine learning models.
   - Evaluate their performance.
4. Analyze the results and insights provided in the final report.

Feel free to open issues or contribute to the repository!
