# Internship_Task_02

# Stock Price Prediction using Random Forest Regression

## Objective
This project aims to predict Apple Inc.'s (AAPL) next-day closing stock prices using historical market data. The goal is to build a machine learning model that can analyze patterns in stock market behavior to forecast future prices.

## Dataset
- **Source**: Yahoo Finance (via yfinance API)
- **Ticker**: AAPL (Apple Inc.)
- **Time Period**: January 1, 2010 to January 1, 2023
- **Features Used**:
  - Open price
  - High price
  - Low price
  - Volume
  - Closing price
- **Target Variable**: Next day's closing price

## Data Characteristics
- **Rows**: 3,279 trading days
- **Columns**: 6 features + target variable
- **No missing values** found in the dataset

## Methodology
1. **Data Preparation**:
   - Created target variable by shifting closing prices forward by 1 day
   - Removed the last row with NaN target value
   - Split data into 80% training and 20% testing sets

2. **Model Applied**:
   - **Random Forest Regressor** with 100 estimators
   - Default hyperparameters with random_state=42 for reproducibility

3. **Evaluation Metrics**:
   - Mean Squared Error (MSE)
   - R-squared (R²) score

## Key Results
- **Mean Squared Error**: [Your MSE value from output]
- **R-squared Score**: [Your R² value from output]
  
The model achieved [good/moderate/poor] performance in predicting next-day closing prices, as evidenced by the R² score of [value]. The actual vs predicted plot shows [describe the visual alignment between lines].

## Visualization
The project includes a comparative plot showing:
- Blue line: Actual closing prices
- Red line: Predicted closing prices

![Actual vs Predicted Prices](actual_vs_predicted.png)

## How to Run
1. Install required packages:
   ```bash
   pip install yfinance pandas numpy scikit-learn matplotlib
