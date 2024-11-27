# Dominos Ingredient Forecasting System:

  This project optimizes Dominos' ingredient ordering process by predicting weekly pizza sales and calculating ingredient requirements using historical data. The ARIMA   model is used for accurate forecasting to minimize waste and prevent stockouts, while insights into sales trends and ingredient usage are also provided.

# Prerequisites:

-> Python 3.x: Required to run the project.
-> Python Libraries: Install the dependencies via pip.

# Libraries Used:

    *pandas: Data manipulation and analysis.
    *numpy: Numerical operations.
    *scikit-learn:
    -> train_test_split: Splitting datasets into training and testing sets.
    -> mean_absolute_percentage_error: Model evaluation metric.
    *matplotlib: Plotting graphs.
    *seaborn: Visualizing trends and insights.
    *statsmodels:
    -> ARIMA: Time series forecasting model.
    -> SARIMAX: Seasonal time series model.
    -> Prophet: Capturing seasonality for forecasting.
    -> XGBoost: Gradient boosting regression model.

# Project Steps: For this steps refer the dominosfinal.py file

1. Data Preprocessing:

    ->Parsed and standardized dates, handled missing values, and removed outliers.
    ->Cleaned and standardized ingredient names for consistency.

2. Feature Engineering:

    ->Aggregated daily sales into weekly data.
    ->Added temporal features like moving averages, lag values, and day indicators.

3. Exploratory Data Analysis:

    ->Visualized sales and revenue trends.
    ->Identified key ingredients and seasonal patterns for production planning.

4. Model Development:

    ->Trained and evaluated four models (Prophet, ARIMA, SARIMA, XGBoost).
    ->Selected ARIMA as the best-performing model (MAPE: 0.8999).

5. Weekly Forecasting:

    ->Predicted weekly pizza sales and calculated ingredient requirements.
    ->Merged forecasts with ingredient data for purchase order generation.

6. Output:

    ->Saved results in an Excel file: Total_Weekly_Ingredients_Quantity.xlsx.

# Output:

The final output is an Excel file containing:

    ->Weekly predicted sales for each pizza type.
    ->Corresponding ingredient requirements for production.
