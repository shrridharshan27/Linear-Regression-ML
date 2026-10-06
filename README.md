# ML Lab 01: Simple & Multiple Linear Regression

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)

---

## Academic Details
- **Student Name:** Shrri Dharshan D R
- **Register Number:** 23BPS1090
- **Course Code:** BCSE209P
- **Course Title:** Machine Learning Laboratory
- **Faculty:** Dr. S. Shridevi
- **Institution:** School of Computer Science and Engineering (SCOPE), VIT Chennai

---

## Overview
This repository contains laboratory implementations and empirical comparative studies of **Simple Linear Regression (SLR)** and **Multiple Linear Regression (MLR)** across three benchmark regression datasets.

The objective is to understand how single vs. multi-variable ordinary least squares (OLS) models perform, evaluate model goodness-of-fit, analyze residual behaviors, and identify key regression metrics.

---

## Experiments & Datasets

### 1. Gas Turbine Electrical Energy Prediction (Lab-1/)
- **Dataset:** Micro Gas Turbine Electrical Energy Prediction Dataset ([UCI ID: 994](https://archive.ics.uci.edu/dataset/994))
- **Objective:** Predict gas turbine net hourly electrical energy output using ambient operating parameters (temperature, pressure, humidity, exhaust vacuum).
- **Notebook:** [Lab-1/23BPS1090_ShrriDharshan_ML_Lab_1.ipynb](./Lab-1/23BPS1090_ShrriDharshan_ML_Lab_1.ipynb)
- **Algorithms:** Simple Linear Regression (Ambient Temperature as predictor) vs. Multiple Linear Regression (all thermodynamic features).

### 2. Morocco Smart Meter High-Resolution Load Analysis (Lab-2/)
- **Dataset:** High-Resolution Load Dataset from Smart Meters Across Various Cities in Morocco
- **Objective:** Model electricity consumption and load profiles against time-series demand attributes.
- **Notebook:** [Lab-2/23BPS1090_ShrriDharshan_ML_Lab2.ipynb](./Lab-2/23BPS1090_ShrriDharshan_ML_Lab2.ipynb)
- **Algorithms:** SLR vs. MLR on smart meter power consumption.

### 3. Paddy Cultivation & Crop Yield Prediction (Lab-3/)
- **Dataset:** Paddy Dataset ([UCI ID: 1186](https://archive.ics.uci.edu/dataset/1186))
- **Objective:** Predict crop yield/output from agricultural cultivation factors (cultivation area, seed rate, manure application, soil profile, variety).
- **Notebook:** [Lab-3/23BPS1090_ShrriDharshan_ML_Lab3.ipynb](./Lab-3/23BPS1090_ShrriDharshan_ML_Lab3.ipynb)
- **Algorithms:** SLR and MLR modeling agricultural yield determinants.

---

## Evaluation Metrics
Models were assessed using standard continuous evaluation criteria:
- **Mean Absolute Error (MAE):** Average magnitude of errors without direction.
- **Mean Squared Error (MSE):** Penalizes larger deviations quadratically.
- **Root Mean Squared Error (RMSE):** Error in original unit scale.
- **Coefficient of Determination (^2$ Score):** Proportion of variance explained by model features.
- **Residual Distribution:** Validating normality and homoscedasticity assumptions.

---

## Repository Structure
`	ext
ML-Lab-01-Linear-Regression/
├── Lab-1/
│   ├── 23BPS1090_ShrriDharshan_ML_Lab_1.ipynb
│   └── gas_turbine_data/
├── Lab-2/
│   ├── 23BPS1090_ShrriDharshan_ML_Lab2.ipynb
│   └── morocco_load_data/
├── Lab-3/
│   ├── 23BPS1090_ShrriDharshan_ML_Lab3.ipynb
│   └── paddy_data/
├── .gitignore
└── README.md
`

---

## How to Run
1. **Clone the repository:**
   `ash
   git clone https://github.com/shrridharshan27/ML-Lab-01-Linear-Regression.git
   cd ML-Lab-01-Linear-Regression
   `
2. **Install dependencies:**
   `ash
   pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo jupyter
   `
3. **Launch Jupyter Notebook:**
   `ash
   jupyter notebook
   `
