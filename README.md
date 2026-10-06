# Linear Regression: Multi-Dataset Predictive Modeling

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Author
- **Shrri Dharshan D R** — [@shrridharshan27](https://github.com/shrridharshan27)

---

## Overview
This repository implements and benchmarks **Simple Linear Regression (SLR)** and **Multiple Linear Regression (MLR)** algorithms across three real-world domain datasets: gas turbine thermodynamic power generation, smart meter electrical load demand, and agricultural paddy crop yields.

The project evaluates ordinary least squares (OLS) regression equations, compares single-variable vs. multi-variable predictors, analyzes residual homoscedasticity and normality, and benchmarks continuous predictive accuracy.

---

## Project Modules & Datasets

### 1. Gas Turbine Electrical Energy Prediction (`gas-turbine-energy/`)
- **Dataset:** Micro Gas Turbine Electrical Energy Prediction Dataset ([UCI ID: 994](https://archive.ics.uci.edu/dataset/994))
- **Objective:** Predict gas turbine net hourly electrical power output using thermodynamic ambient parameters (ambient temperature, ambient pressure, relative humidity, exhaust vacuum).
- **Notebook:** [`gas-turbine-energy/23BPS1090_ShrriDharshan_ML_Lab_1.ipynb`](./gas-turbine-energy/23BPS1090_ShrriDharshan_ML_Lab_1.ipynb)
- **Methodology:** Simple Linear Regression (Ambient Temperature as primary predictor) compared against full Multiple Linear Regression across all ambient features.

### 2. Morocco Smart Meter High-Resolution Load Modeling (`morocco-load-demand/`)
- **Dataset:** High-Resolution Load Dataset from Smart Meters Across Moroccan Cities
- **Objective:** Model electricity consumption profiles and demand characteristics from time-series load attributes.
- **Notebook:** [`morocco-load-demand/23BPS1090_ShrriDharshan_ML_Lab2.ipynb`](./morocco-load-demand/23BPS1090_ShrriDharshan_ML_Lab2.ipynb)
- **Methodology:** SLR vs. MLR modeling consumption dynamics against temporal and atmospheric load covariates.

### 3. Paddy Cultivation & Agricultural Crop Yield Prediction (`paddy-crop-yield/`)
- **Dataset:** Paddy Dataset ([UCI ID: 1186](https://archive.ics.uci.edu/dataset/1186))
- **Objective:** Forecast crop yield from agricultural cultivation factors (land area, seed rate, organic manure, fertilizers, soil profile, variety).
- **Notebook:** [`paddy-crop-yield/23BPS1090_ShrriDharshan_ML_Lab3.ipynb`](./paddy-crop-yield/23BPS1090_ShrriDharshan_ML_Lab3.ipynb)
- **Methodology:** OLS parameter estimation, multi-collinearity checks, and comparative residual diagnostics.

---

## Evaluation Metrics
Model performance is benchmarked using standard continuous regression metrics:
- **Mean Absolute Error (MAE):** Linear average magnitude of residuals.
- **Mean Squared Error (MSE):** Quadratic penalty on large prediction discrepancies.
- **Root Mean Squared Error (RMSE):** Error interpretable in the original target measurement units.
- **Coefficient of Determination ($R^2$):** Proportion of variance explained by model covariates.
- **Residual Distribution Plots:** Assessing OLS normality and homoscedasticity assumptions.

---

## Project Structure
```text
Linear-Regression-ML/
├── gas-turbine-energy/
│   ├── 23BPS1090_ShrriDharshan_ML_Lab_1.ipynb
│   └── gas_turbine_data/
├── morocco-load-demand/
│   ├── 23BPS1090_ShrriDharshan_ML_Lab2.ipynb
│   └── morocco_load_data/
├── paddy-crop-yield/
│   ├── 23BPS1090_ShrriDharshan_ML_Lab3.ipynb
│   └── paddy_data/
├── .gitignore
└── README.md
```

---

## Quickstart & Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/shrridharshan27/Linear-Regression-ML.git
   cd Linear-Regression-ML
   ```
2. **Install requirements:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo jupyter
   ```
3. **Run the notebooks:**
   ```bash
   jupyter notebook
   ```

---

## License
Distributed under the [MIT License](https://opensource.org/licenses/MIT).
