# Traffic Density Analysis

This repository contains the code and analysis notebooks for the **DSPG Project** on assessing the impact of scheduled road maintenance on traffic density in Istanbul.

## Team
- [Niyazi Ülke](https://github.com/niyaziulke)
- Esra ŞEKERCİ

## Objective
To estimate how planned road maintenance activities affect average traffic speeds using machine learning, enabling authorities to schedule maintenance during low-traffic periods to minimize disruption.

## Dataset Overview
- **Traffic Speed Data**: 30-minute intervals for selected roads (Jan–Jun 2019)
- **Maintenance Logs**: Time, coordinates, type, and day/night info
- **Weather Data**: Daily rainfall levels in Istanbul
- **Holiday Info**: Dates of official public holidays in 2019

## Methods & Tools
- GIS & Mapping: `osmnx` for spatial matching of maintenance coordinates to road segments
- Feature Engineering: Time, weather, road characteristics, maintenance presence/type
- Models Tested:
  - Decision Tree Regressor
  - Random Forest Regressor
  - Linear & Ridge Regression

## Modeling Strategy
Three modeling approaches were evaluated:
1. Separate model per **road** (high risk of overfitting)
2. Single model for **all roads** (too many categorical features)
3. **Separate model per district** (best balance – selected strategy)|

