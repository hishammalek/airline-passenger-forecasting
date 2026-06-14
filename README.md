# **Airline Passenger Demand Forecasting: ARIMA vs SARIMA Analysis**
**Python & Power BI | Time Series Forecasting & Business Insights**

[![Python](https://img.shields.io/badge/Python-3.14-blue)](https://www.python.org/)
[![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-green)](https://powerbi.microsoft.com/)

---

## **Project Overview**
Analyzed the **Airline Passenger dataset (1949-1960)** to understand passenger demand trends and seasonal patterns

The goal is to build a forecasting model that can predict future passenger demand and to support airline planning in all aspects
ARIMA and SARIMA models were used to compare forecasting performance
The final model helps identify seasonal peaks and long-term proportional growth in air travel demand

---

## **Problem Statement**
Airlines need accurate forecasts for passenger demand to optimize capacity, staffing, scheduling and marketing

This project explores whether ARIMA or SARIMA provides better forecasting performance for this dataset of airline passenger demand

---

## **Dataset**
- Source: https://www.kaggle.com/datasets/chirag19/air-passengers
- Time period: 1949-1960
- Key variables: Passengers (monthly time series)

---

## **Tools Used**
Python:
- pandas
- numpy
- matplotlib
- statsmodels
- sklearn
   
Power BI:
- Interactive dashboard
- KPI visuals
- Forecast visualization

---

## **Methodology**
- Data cleaning and preprocessing
- Exploratory time series analysis
- Feature engineering (trend & seasonality)
- ARIMA baseline modeling
- SARIMA seasonal modeling
- Model evaluation using Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE)
- Forecast visualizations and comparison

---

## **Key Insights**

1. Passenger demand shows a **strong long-term upward trend**
2. Clear **seasonal fluctuations** with peak travel mid-year and lowest on Nov - Feb
3. SARIMA was selected as the **final model due to significantly lower error and its ability to capture seasonal demand patterns**
4. Forecasts show **continued proportional growth** in air travel demand throughout the years

---

## **Model Performance**
- **ARIMA: (1,1,0)** baseline model with no seasonality and AIC score of 1401.85
- **SARIMA: Final model (1,1,0)(1,1,0,12)** improved performance with seasonal componennt and AIC score of 1020.393
- Evaluation metrics:
  - **RMSE: 20.81 (3.35%)**
  - **MAE: 15.99 (2.57%)** 

---

## **Business Impact**

- Helps airlines **plan capacity** during peak travel seasons
- Optimize **staffing, scheduling decisions and resource allocation**
- Improves demand forecasting for **revenue planning**
- Prepare for **seasonal fluctuations in advance**
- Reduce risk of **over or under** capacity
  
---

## **Project Structure**

data_raw/

data_clean/

notebooks/

powerbi/

assets/

Organized project into modular folders for reproducibility and Power BI integration

---

## **Future Improvements**

- Include **external variables** to perform ARIMAX, such as GDP, festive seasons, promotions, fuel prices or travel demand factors
- Try other forecasting like **Prophet or LSTM (Long Short-Term Memory)**
- Perform **hyperparameter tuning** for SARIMA
- Expand dataset with more **recent** airline data

**Overall, the SARIMA model provides a reliable baseline forecasting approach for airline passenger demand and demonstrates the importance of incorporating seasonality in time series analysis**

---


## **Visuals**

### Executive Overview
![airline-passenger-forecasting](assets/images/01_executive_overview.png)

### Trend & Seasonality
![airline-passenger-forecasting](assets/images/02_trend_seasonality.png)

### Forecast vs Actual
![airline-passenger-forecasting](assets/images/03_forecast_actual.png)

### Business Insights
![airline-passenger-forecasting](assets/images/04_business_insights.png)

Click on the Power BI file in the `powerbi/` folder to explore the interactive dashboard.



