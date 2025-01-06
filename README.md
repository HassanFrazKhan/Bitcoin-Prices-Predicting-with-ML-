# Predicting Bitcoin Prices Using Machine Learning Models

## Overview
This project explores the performance of three machine learning models—Linear Regression, Random Forest Regressor, and LSTM (Long Short-Term Memory)—in predicting the price of Bitcoin. The goal is to understand how these models handle the volatility and complex patterns in Bitcoin’s price using historical data collected from Yahoo Finance.

### Research Question
How do different machine learning models perform in predicting the price of Bitcoin, and what factors contribute to their varying performance?

## Abstract
This study investigates the application of machine learning models for predicting Bitcoin prices, aiming to address the challenges posed by the high volatility and complexity of cryptocurrency markets. The research evaluates the performance of three distinct models—Linear Regression, Random Forest, and Long Short-Term Memory (LSTM) networks—to provide a comprehensive understanding of their strengths and limitations in financial forecasting. By leveraging historical Bitcoin price data and feature engineering techniques, the study highlights the predictive capabilities of these models while offering valuable insights into their practical implications.

Linear Regression served as a baseline model, demonstrating strong predictive performance with a fine-tuned Mean Absolute Error (MAE) of 1181.13, Root Mean Squared Error (RMSE) of 1754.55, and R-squared (R²) value of 0.9931. Random Forest, an ensemble learning method, excelled in identifying feature importance, with the 5-day moving average emerging as the most significant predictor. Despite its strengths in handling non-linear relationships, the model’s overall accuracy was comparatively lower, with an MAE of 3888.63, RMSE of 8717.58, and R² value of 0.8286. LSTM networks, designed specifically for time-series forecasting, demonstrated superior performance by effectively capturing temporal dynamics and volatility. With an MAE of 1456.71, RMSE of 2087.55, and R² value of 0.9903, LSTM emerged as the most suitable model for predicting Bitcoin prices.

The study also included 30-day future price predictions, providing a practical demonstration of the models’ applicability. Linear Regression produced smooth, trend-aligned forecasts, while Random Forest exhibited greater variability in its predictions. LSTM balanced trend consistency with the ability to capture fluctuations, showcasing its adaptability to volatile market conditions.

The findings of this research underscore the importance of selecting models that align with the specific objectives and characteristics of the dataset. While Linear Regression provides a computationally efficient baseline, LSTM offers the nuanced understanding required for dynamic financial markets. Random Forest, despite its lower accuracy, contributes to feature interpretability and enriches the overall analysis.

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
