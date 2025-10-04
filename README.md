# 🌍 Short-Term Forecast of Gaseous Air Pollutants (O₃ and NO₂) using Satellite and Reanalysis Data

## 🧠 Overview
This repository presents a **prototype system** designed to predict short-term ground-level concentrations of **Ozone (O₃)** and **Nitrogen Dioxide (NO₂)** in urban areas such as **Delhi**, using a combination of **satellite-derived** and **meteorological reanalysis** data.

Air pollution in megacities poses a major health challenge, with O₃ and NO₂ often exceeding safe air quality limits. The proposed approach integrates multiple data sources to enable **data-driven air quality forecasting** and support **early warning systems**.

---

## 🚀 Project Objective
To build a **machine learning–based forecasting pipeline** that predicts **O₃ and NO₂ concentrations** for the next **24 to 48 hours** using satellite and reanalysis datasets.

> ⚠️ **Note:**  
> This project is currently a **prototype**. Predictions are generated using **typical machine learning algorithms** (e.g., Linear Regression, Random Forest, XGBoost) rather than deep learning or time series models like LSTM or Transformer.  
> Future work will focus on developing advanced **spatio-temporal models** for improved accuracy.

---

## 🧩 Methodology

### 1. Data Sources
- **Satellite Data:** Sentinel-5P (TROPOMI) datasets for tropospheric NO₂, CO, HCHO, and O₃.
- **Reanalysis Data:** ERA5 meteorological parameters (temperature, wind speed, boundary layer height, humidity, etc.).
- **Ground Data:** Central Pollution Control Board (CPCB) monitoring stations in Delhi for ground-truth validation.

### 2. Data Preprocessing
- Spatial alignment and temporal synchronization of datasets  
- Feature engineering:
  - Lagged pollutant values  
  - Meteorological variables  
  - Diurnal and seasonal indicators  
- Handling missing values and normalization

### 3. Model Development
- Implemented and compared baseline ML algorithms:
  - Linear Regression  
  - Decision Tree Regressor  
  - Random Forest Regressor  
  - XGBoost Regressor  
- Evaluation Metrics:
  - Root Mean Square Error (RMSE)  
  - Mean Absolute Error (MAE)  
  - Bias  

### 4. Forecasting
- Short-term (24–48 hour) pollutant concentration forecasts  
- Visualization of results for interpretability and comparison  

---

## 📊 Results
- The prototype demonstrates the feasibility of forecasting O₃ and NO₂ using hybrid data sources.  
- Preliminary results show reasonable performance from traditional ML models, confirming the validity of the proposed data fusion approach.

---

## 🧠 Future Work
- Integrate **deep learning (LSTM, CNN-LSTM, Transformer)** models for improved temporal forecasting  
- Expand to other pollutants (PM
