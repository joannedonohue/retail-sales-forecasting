# Retail Sales Forecasting

Predictive models for retail demand planning using Walmart sales data — achieving R² = 0.96 with Random Forest and Gradient Boosting on weekly sales forecasting.

---

## Overview

This project builds machine learning models to forecast weekly retail sales across Walmart store types, with a secondary analysis applying classification to cardiovascular disease risk data. The primary forecasting pipeline identifies store type and temperature as the strongest demand signals, and flags holiday markdown periods as significant sales drivers.

---

## Key Results

| Task | Model | Metric | Score |
|---|---|---|---|
| Weekly sales forecasting | Random Forest / Gradient Boosting | R² | **0.96** |
| Disease risk classification | Classification model | Accuracy | **71%** |

---

## Dataset

- **Primary:** Walmart historical weekly sales data across multiple store types
- **Features:** Store type, temperature, fuel price, CPI, unemployment rate, holiday indicators
- **Secondary:** Bureau of Labor Statistics supplementary employment data

---

## Top Predictors (Feature Importance)

1. **Store type** — accounts for largest variance in weekly sales volume
2. **Temperature** — seasonal demand signal with strong predictive weight
3. **Holiday markdown periods** — significant uplift events requiring separate modeling consideration

---

## Models

- **Random Forest** — primary ensemble model; handles non-linear interactions between store, region, and economic variables
- **Gradient Boosting** — secondary ensemble; captures sequential patterns in time-ordered data
- **Linear Regression** — baseline comparison

---

## Methodology

1. Load Walmart historical sales and supplementary BLS data
2. Engineer features: holiday flags, store type encoding, economic indicator normalization
3. Train and evaluate Random Forest, Gradient Boosting, and Linear Regression
4. Analyze feature importance to identify primary demand drivers
5. Separately apply classification models to cardiovascular disease risk dataset

---

## Tech Stack

| Component | Tool |
|---|---|
| Machine learning | scikit-learn |
| Data manipulation | pandas |
| Visualization | Matplotlib, Seaborn |
| Language | Python |

---

## Repository Structure

```
retail-sales-forecasting/
├── retail_sales_forecasting.ipynb          # Main forecasting notebook
├── Untitled1.ipynb                         # Exploratory analysis
├── walmart_holiday_predict_app.py          # Holiday prediction application
├── walmart_holiday_predict_v2.py           # Iterated holiday model
├── walmart_weekly_sales_v1.py              # Weekly sales model v1
├── walmart_weekly_sales_v2.py              # Weekly sales model v2
├── AI Bootcamp Project 2 - Group 3 Walmart.pdf   # Presentation slides
├── Resources/                              # Input datasets
└── README.md
```

---

## Outcomes

- Achieved **R² = 0.96** on Walmart weekly sales forecasting — the model explains 96% of sales variance
- Identified store type and temperature as primary demand signals, providing actionable guidance for inventory and staffing planning
- Discovered holiday markdown periods as significant non-linear demand events requiring special-case handling
- Produced a deployable holiday prediction application alongside the core forecasting pipeline

---

## Getting Started

```bash
pip install scikit-learn pandas matplotlib seaborn
jupyter notebook retail_sales_forecasting.ipynb
```
