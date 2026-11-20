# Johannesburg Air Quality & Smog Early-Warning System

## Problem Statement
During winter, cold air inversions, traffic, and industrial emissions cause severe air pollution spikes in Johannesburg. Vulnerable residents—including children, older adults, and people with asthma—need advance warning before air quality reaches unhealthy levels.

## Dataset & Cleaning
- **Source:** Historical Daily Air Quality Data for Johannesburg (`air_quality_historical.csv`)
- **Size:** 1,294 clean daily records after removing 4 incomplete rows
- **Key Features:** `pm2_5`, `pm10`, `ozone`, `sulphur_dioxide`, `nitrogen_dioxide`, `carbon_monoxide`, `us_aqi`, and `month`

## Key Findings
- **Winter Smog Spike:** Average monthly air quality crosses above the unhealthy threshold (`US AQI > 100`) during **May, June, and July**, peaking in June.
- **Summer Relief:** Summer rainfall and wind keep average AQI lower (`75–85`) from September through April.

## Predictive Model
- Trained a **Random Forest Regressor** using chronological train/test splitting (80% past days, 20% recent days) to forecast **next-day US AQI** and flag unhealthy air days early.

## Files in This Repository
- `project_2.ipynb` — Full data cleaning, visualization, and Random Forest modeling notebook
- `monthly_aqi_chart.png` — Average monthly US AQI across Johannesburg
- `aqi_prediction_chart.png` — Actual vs. predicted next-day US AQI over the test period
-# Johannesburg-air-quality
