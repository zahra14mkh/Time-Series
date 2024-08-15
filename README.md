# Time Series Analysis for Energy Production Forecasting

## Overview
This project applies time series analysis techniques to forecast energy production using various ARIMA and SARIMA models. It involves data visualization, stationarity checks, model selection, residual analysis, and performance evaluation. The models used in this project include manually configured ARIMA, automatically optimized ARIMA (based on AIC and BIC), and a seasonal SARIMA model.

## Requirements
The project is implemented in Python. The following libraries are required:
- `pandas`
- `numpy`
- `matplotlib`
- `pmdarima`
- `statsmodels`
- `scipy`
- `sklearn`

To install the necessary packages, run:
```bash
pip install pandas numpy matplotlib pmdarima statsmodels scipy scikit-learn
```

## Dataset
The dataset used in this project is time series data for energy production. The data should be in CSV format, with dates as the index and energy production values as the column.

## Key Steps in the Project:
1. **Data Import and Visualization:**
   - The dataset is imported and visualized to understand the trend and seasonality.

2. **Stationarity Check and Transformation:**
   - The Augmented Dickey-Fuller (ADF) test is used to check for stationarity.
   - Differencing is applied to achieve stationarity if necessary.

3. **Model Selection:**
   - ARIMA models are configured manually and optimized using AIC and BIC criteria.
   - A seasonal SARIMA model is also created to account for any seasonal patterns in the data.

4. **Model Fitting and Forecasting:**
   - The models are fitted to the training data and forecasts are made for the test data.
   - Forecasts are visualized and compared.

5. **Residual Analysis and Evaluation:**
   - Residuals from the models are checked for normality using the Shapiro-Wilk test.
   - Models are evaluated using the R²-score, Mean Absolute Error (MAE), and Mean Squared Error (MSE).

6. **SARIMA Model:**
   - A SARIMA model is used to capture seasonality and is compared with ARIMA models.

## Usage
1. Place the dataset (CSV format) in the project directory.
2. Modify the file path to the dataset in the `pd.read_csv()` function.
3. Run the notebook to perform data analysis, model selection, and forecasting.
4. Check the model performance metrics in the output.

## Output
- Forecast plots for the ARIMA and SARIMA models.
- Performance comparison of the models using error metrics and R² scores.

## Conclusion
This project provides insights into selecting and evaluating time series forecasting models. It compares various ARIMA models and a seasonal SARIMA model, helping to identify the best model for forecasting energy production.
