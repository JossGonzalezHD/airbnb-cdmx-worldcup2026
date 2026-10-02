# Airbnb CDMX: Pricing Intelligence for the 2026 World Cup
### A Comparative Machine Learning Study: Random Forest vs Neural Network

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JossGonzalezHD/airbnb-cdmx-worldcup2026/blob/main/airbnb_cdmx_worldcup2026_v2_comparative.ipynb)

---

## Overview

This project builds and compares two supervised Machine Learning models to predict nightly rental prices on Airbnb in Mexico City, with a focus on the business opportunity created by the **2026 FIFA World Cup**.

Context: an illustrative analysis built around the operating zones of a furnished-rental company in **Miguel Hidalgo (Polanco)** and **Cuauhtémoc (Condesa, Roma)**, two of the most premium zones in the CDMX Airbnb market. This is an academic project built with public data; it was not implemented in production.

---

## Key Findings

- **Random Forest** outperformed the Neural Network across all three metrics (R², MAE, RMSE)
- **Distance to Estadio Azteca** (constructed via Haversine formula) ranked as the **2nd most important feature** for price prediction, above number of bedrooms

---

## Illustrative Revenue Scenario (assumption-based, not a validated forecast)

Assuming a +35% price increase, 98% occupancy and 215 units over 30 peak nights, revenue would move from about MXN 10.3M to about MXN 15.2M. The +35% increase, the 98% occupancy and the 215-unit count are my assumptions. The model only supports the relative importance of distance to Estadio Azteca; it does not validate this revenue figure.

---

## Models Compared

| Metric | Random Forest | Neural Network (MLP) |
|--------|--------------|----------------------|
| R² | **0.5468** | 0.5106 |
| MAE | **$292 MXN** | $314 MXN |
| RMSE | **$413 MXN** | $429 MXN |
| Negative predictions | **None** | Yes |

---

## Dataset

- **Source:** [Inside Airbnb — Mexico City](http://insideairbnb.com/get-the-data)
- **Snapshot:** September 27, 2025
- **Original records:** 27,052 properties
- **After cleaning:** 19,249 properties × 22 features

---

## Tech Stack

- Python 3 / Google Colab
- Scikit-learn (RandomForestRegressor, MLPRegressor)
- Pandas, NumPy, Matplotlib, Seaborn
- Geopy (Haversine distance calculation)

---

## Author

**Joseph Gonzalez**  
Field Operations Staff (Operations Hub), Mexico City  
M.S. in IT Management, Data Science specialty, Universidad Tecmilenio
