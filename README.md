# TFT-QuantileRegression-WindEnergy-Prediction48h

# Thesis – 48h Wind Power Forecasting Using Deep Learning Models

**Temporal Fusion Transformer (TFT) & LSTM for Smart Energy Planning**
Mälardalen University, 2025 | Electrification Hub Collaboration

---

## Project Overview

As the world transitions away from fossil fuels, accurate forecasting of renewable energy—particularly wind power—remains a major challenge. Reliable forecasts are critical for:

* Smart energy management
* Proactive planning and integration of storage
* Demand-side flexibility
* Enabling a sustainable, fossil-free energy future

This project demonstrates how deep learning with uncertainty awareness can support the green transition.

---

## Methods

**Modeling Approach:**

* Temporal Fusion Transformer (TFT) with quantile regression loss
* Baseline: LSTM

**Feature Engineering:**

* Wind direction and speed decomposed into vector components (u, v)
* Weather data and calendar features (hour, day, week, month) encoded using cyclical functions

**Data Sources:**

* Historical wind production (SE1 & SE3 regions, Sweden)
* Weather forecasts

---

## Results (MAPE – Mean Absolute Percentage Error)

* 1h: 7.66% error → 94.34% accuracy
* 12h: 10.15% error → 89.85% accuracy
* 24h: 12.54% error → 87.46% accuracy
* 36h: 17.50% error → 82.50% accuracy

The TFT model provided uncertainty-aware forecasts, enabling better risk-aware decision making compared to deterministic models.

---

## Impact and Applications

This project highlights how AI-powered forecasting can:

* Optimize energy storage and demand-side flexibility
* Enable cost-efficient, risk-aware decisions in energy markets
* Support smart grids and EV charging planning
* Reduce reliance on non-renewable energy sources

Since wind power has near-zero marginal cost, high wind output often correlates with lower spot prices, making accurate forecasts crucial for the energy sector.

---

## Collaboration

This thesis was conducted by Rickars Sörlin and Fredrik Karlsson as part of an interdisciplinary Electrification Hub initiative with students in:

* Applied AI
* Civil Engineering in Energy
* Finance
* Applied Mathematics

---

## Repository Structure

* `notebooks/` – model training and evaluation
* `data/` – processed datasets (not public, linked via SMHI API)
* `src/` – helper functions (data preprocessing, feature engineering, model utilities)
* `results/` – plots, metrics, visualizations

---

## Visuals

(Here you should add screenshots/plots, e.g. predicted vs. actual wind power curve, TFT attention weights, quantile ranges, etc.)


