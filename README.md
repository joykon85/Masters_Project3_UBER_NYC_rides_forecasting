# NUS-ISS MSc Data Science – Group Project 3
## Specialized Predictive Modelling & Forecasting  
### Uber NYC Ride Demand Forecasting (2023–2024)

## Project Overview

This project was completed as part of the **NUS-ISS Master of Science in Data Science** programme under the module **Specialized Predictive Modelling & Forecasting**.

The objective of the project is to analyze and forecast **Uber ride demand in New York City** using large-scale historical trip data (2023–2024), with a focus on **time-series forecasting for driver allocation and operational planning**.

Ride request data was aggregated to **hourly order counts** by pickup location to support time-series modelling.

---

## My Contributions (Scope of This Repository)

This repository contains **only my individual contributions** to the group project, specifically:

- **Time-series demand forecasting using:**
  - **LSTM (Long Short-Term Memory) neural networks**
  - **ARIMA / SARIMAX models**
- Data preprocessing and feature engineering for hourly demand prediction
- Model training, evaluation, and comparison against benchmark baselines
- Forecasting demand at **next-hour and next-day horizons**

Other components of the group project (e.g. pricing optimisation, survival analysis, Monte Carlo simulation, and linear programming) were implemented by other team members and are **not included** in this repository.

---

## Modelling Approach

### Data Preparation
- Uber ride request data for NYC (2023–2024)
- Aggregated to **order count per hour**
- Focused on **Manhattan pickup locations** to reduce complexity and improve model performance
- Feature engineering included:
  - Hour, day of week, weekend indicators
  - Holiday indicators
  - Normalization and sequencing for time-series models

### Models Implemented
- **SARIMAX**
  - Statistical baseline with seasonal components and exogenous variables
  - Used to evaluate limitations of classical time-series models
- **LSTM**
  - Deep learning approach for multi-location time-series forecasting
  - Trained to predict:
    - Next-hour demand
    - Next-day demand
  - Demonstrated significant improvement over naïve benchmark models

Model performance was evaluated using **MSE and RMSE** metrics.

---

## Environment & Execution Notes

- Analysis and modelling were performed using **Jupyter Notebooks on Google Colab**
- Notebooks may require **minor path or dependency adjustments** to run locally after download

---

## Full Report

The complete project methodology, results, and business insights are documented in the final group report

---

## Notes

- This repository includes **only the code for my assigned modelling components (LSTM and ARIMA/SARIMAX)**.
- Other parts of the project and dashboards referenced in the report are **not included**.
