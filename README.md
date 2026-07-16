\# German Electricity Load Forecasting



\## Project Overview



This project investigates electricity load forecasting for Germany using multiple forecasting approaches. The study compares statistical, machine learning and deep learning models on historical electricity demand data.



The project was completed as part of an MSc Data Science forecasting assignment.



\---



\## Objectives



\- Forecast German electricity load

\- Compare multiple forecasting approaches

\- Evaluate forecast accuracy using standard metrics

\- Analyse the effect of weather (temperature) as an exogenous variable



\---



\## Dataset

The hourly electricity dataset (time_series_60min_singleindex.csv) exceeds GitHub's web upload limit (25 MB) and is therefore not included in this repository.

It can be downloaded from the Open Power System Data project:
https://open-power-system-data.org/

Electricity Load:

\- ENTSOE Transparency Platform

\- Hourly German electricity demand (2015–2020)



Temperature:

\- Open-Meteo Archive API

\- Daily Berlin temperature



\---



\## Models Implemented



\### Part 1

Seasonal Naive Benchmark



\### Part 2

SARIMA



\### Part 3

SARIMAX (Temperature as Exogenous Variable)



\### Part 4

Random Forest Regressor



\### Part 5

LSTM Neural Network



\---



\## Evaluation Metrics



\- RMSE

\- MAE

\- R² Score



\---



\## Repository Structure



```

german-load-forecasting/

│

├── data/

├── figures/

├── notebook/

├── report/

├── saved\_models/

│

├── README.md

├── requirements.txt

├── .gitignore

└── LICENSE

```



\---



\## Technologies Used



\- Python

\- Pandas

\- NumPy

\- Matplotlib

\- Scikit-learn

\- Statsmodels

\- TensorFlow

\- Keras



\---



\## Results



| Model | RMSE |

|--------|------|

| SARIMAX | 3816.99 |

| Random Forest | 2951.93 |

| LSTM | 1791.27 |



The LSTM model achieved the best forecasting performance among the evaluated models.



\---



\## Author



Harshitha Maruri



MSc Data Science



University of Hertfordshire

