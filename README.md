# FIFA World Cup 2026: Measuring Food & Accommodation Spending Surges in US Host Cities

### Using SARIMA time series forecasting to establish pre-tournament consumer spending baselines across 9 US cities, then quantifying the World Cup spending premium as live data becomes available.

## Project Overview
This project trains SARIMA models on 4+ years of historical restaurant and hotel consumer spending data to forecast what spending would look like in a normal summer without the World Cup. By comparing these baselines against actual June/July 2026 spending data, we quantify the tournament's economic impact on local businesses across US host and control cities.


## Research Questions
1. How much does spending increase vs a normal summer baseline?
2. Which week peaks — opening weekend, match days, or the final?
3. Do non-host cities see spillover effects?
4. Which host city sees the biggest impact?


## Cities Analyzed
**Host Cities:** Dallas, Los Angeles, Atlanta, Boston, Kansas City  
**Control Cities:** Chicago, Austin, Denver, Charlotte


## Methodology
1. **EDA** — Explored historical spending patterns (2022–2026) across all 9 cities
2. **SARIMA Modeling** — Built individual SARIMA models per city using auto_arima parameter selection
3. **Model Evaluation** — Walk-forward cross-validation to validate forecast accuracy
4. **World Cup Analysis** — Baseline forecasts compared against live 2026 tournament data as it becomes available to quantify world cup affect on food and accommodation consumer spending

## Stack
Python · Pandas · Statsmodels · pmdarima · Matplotlib · Seaborn · Scikit-learn

## Status
**In Progress** — SARIMA baseline models built and validated. World Cup spending comparison pending Opportunity Insights June/July 2026 data release (expected July/August 2026).


## Key Finding (Preliminary)
Non-host cities historically outperform host cities in restaurant and hotel spending, largely driven by Los Angeles persistently underperforming other metros. Any divergence above SARIMA-forecasted baselines during World Cup weeks will be attributed to the tournament effect.


## Data Source
[Opportunity Insights Economic Tracker](https://economictracker.org)  
Chetty, Friedman, Stepner, and the Opportunity Insights Team (QJE 2023)