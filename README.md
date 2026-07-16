# German Electricity Load Forecasting using Time Series and Machine Learning

## Project Overview

This project was completed as part of a Time Series Modelling coursework. The objective is to forecast German electricity demand using statistical time-series methods, machine learning, and deep learning techniques.

The project compares multiple forecasting approaches including:

- Seasonal Naïve Forecast
- SARIMA
- SARIMAX (using Berlin temperature as an exogenous variable)
- Random Forest Regression
- Long Short-Term Memory (LSTM) Neural Network

Model performance is evaluated using standard forecasting metrics and visual comparison of predictions against actual electricity demand.

---

## Repository Structure

```
time_series_modelling_case_study/
│
├── data/
│   └── berlin_temperature_daily.csv
│
├── figures/
│   ├── seasonal_naive_forecast.png
│   ├── sarima_forecast.png
│   ├── sarimax_forecast.png
│   ├── random_forest_forecast.png
│   └── lstm_forecast.png
│
├── notebook/
│   └── time_series_modelling_case_study.ipynb
│
├── saved_models/
│   ├── sarimax_model.pkl
│   ├── random_forest_model.joblib
│   └── lstm_model.keras
│
├── README.md
├── LICENSE
├── requirements.txt
└── .gitignore
```

---

## Dataset

### Electricity Load

- German electricity load (hourly resolution)
- Source: Open Power System Data (OPSD)

### Weather Data

- Daily Berlin temperature
- Source: Open-Meteo Historical Weather API

Temperature data is used as an exogenous variable in the SARIMAX model.

**Note:** The original hourly electricity dataset is not included because it exceeds GitHub's upload size limit. Users should download it separately before running the notebook.

---

## Methods Implemented

### 1. Seasonal Naïve Forecast

A simple baseline model using historical seasonal observations.

### 2. SARIMA

Seasonal AutoRegressive Integrated Moving Average model for weekly electricity demand forecasting.

### 3. SARIMAX

SARIMA extended with weekly Berlin temperature as an exogenous predictor.

### 4. Random Forest

Feature-based regression model trained on weekly electricity demand and explanatory variables.

### 5. LSTM

Deep learning model trained using hourly electricity demand sequences to forecast the final two years of the dataset.

---

## Evaluation Metrics

The models were evaluated using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score (LSTM)

Forecasts were also visually compared with actual observations.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Scikit-learn
- TensorFlow
- Keras

---

## Saved Models

The repository includes trained models:

- SARIMAX
- Random Forest
- LSTM

These can be loaded without retraining.

---

## How to Run

1. Clone this repository.

```
git clone <repository-url>
```

2. Install dependencies.

```
pip install -r requirements.txt
```

3. Download the hourly electricity load dataset.

4. Place the datasets inside the `data/` directory.

5. Open and execute:

```
notebook/time_series_modelling_case_study.ipynb
```

---

## Results

The project demonstrates the application of:

- Classical statistical forecasting
- Machine learning
- Deep learning

for German electricity demand forecasting and compares their predictive performance using common evaluation metrics.

---

## Author

**Harshitha Maruri**

MSc Data Science

University of Hertfordshire

2026

---

## License

This project is provided for academic purposes only.
