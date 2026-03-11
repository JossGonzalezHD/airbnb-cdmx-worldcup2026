# Airbnb CDMX: Pricing Intelligence for the 2026 World Cup
### A Comparative Machine Learning Study: Random Forest vs Neural Network

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JossGonzalezHD/airbnb-cdmx-worldcup2026/blob/main/airbnb_cdmx_worldcup2026_v2_comparative.ipynb)

---

## Overview

This project builds and compares two supervised Machine Learning models to predict nightly rental prices on Airbnb in Mexico City, with a focus on the business opportunity created by the **2026 FIFA World Cup**.

The analysis is grounded in real operations: the author manages 215+ short-term rental units across **Miguel Hidalgo (Polanco)** and **Cuauhtémoc (Condesa, Roma)** — two of the most premium zones in the CDMX Airbnb market.

---

## Key Findings

- **Random Forest** outperformed the Neural Network across all three metrics (R², MAE, RMSE)
- **Distance to Estadio Azteca** (constructed via Haversine formula) ranked as the **2nd most important feature** for price prediction — above number of bedrooms
- NIDO's operating zones command a **44–54% price premium** over the city average
- Projected additional revenue opportunity during World Cup peak nights: **+$4.9M MXN (~USD 286K)** across 215 units

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
Sr. Field Operations Staff — NIDO / RentinBA, Mexico City  
Master's in IT Management (Cloud Computing & Data Science) — Universidad Tecmilenio
