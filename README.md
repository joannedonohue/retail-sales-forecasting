# Retail Sales Forecasting with Machine Learning

Predictive models for retail demand planning using real-world Walmart sales data, with a secondary analysis on cardiovascular disease classification.

## Overview

This project builds and evaluates machine learning models to forecast weekly sales across Walmart store departments. Accurate demand forecasting is critical in retail operations — reducing overstock, preventing stockouts, and informing promotional strategy.

## Key Results

- **R² = 0.96** on Walmart weekly sales forecasting
- Top predictors: **store type** and **temperature** (seasonal demand signals)
- Holiday markdown periods identified as significant sales drivers
- Secondary model: **71% accuracy** on cardiovascular disease risk classification

## Dataset

- Walmart historical weekly sales across multiple store types and departments
- Features include temperature, fuel price, CPI, unemployment rate, and holiday flags
- Bureau of Labor Statistics supplementary data

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat-square)

- **Models**: Random Forest, Gradient Boosting, Linear Regression
- **Evaluation**: R², RMSE, feature importance analysis
- **Visualization**: Matplotlib, Seaborn

## Project Structure

```
├── FInal_Walmart_Sales_Predict.ipynb   # Main forecasting notebook
├── walmart_weekly_sales_v1.py          # Sales model script v1
├── walmart_weekly_sales_v2.py          # Sales model script v2
├── walmart_holiday_predict_app.py      # Holiday prediction app
├── Resources/                          # Source datasets
└── README.md
```

## Business Context

Demand forecasting directly impacts supply chain efficiency, inventory investment, and promotional ROI — core levers in consumer goods and retail strategy. This analysis demonstrates the ability to translate raw transactional data into actionable forecasting insights at scale.
