# 📊 Walmart Retail Sales Analysis and Forecasting using SARIMAX

## 📌 Project Overview
Retail businesses rely on accurate demand forecasting to optimize inventory levels, reduce stock shortages, and minimize excess inventory costs. This project builds an end-to-end time series forecasting pipeline using the Walmart Store Sales dataset to analyze historical sales patterns and predict future weekly sales.

The project combines data preparation, exploratory data analysis, statistical diagnostics, feature engineering, and SARIMAX forecasting to generate a 12-week sales forecast that supports inventory planning and business decision-making.

**Business Problem:** Walmart stores experience varying customer demand throughout the year, especially during holiday seasons. Accurate sales forecasting helps support inventory planning and improve operational decision-making.  
**Objective:** Analyze historical sales patterns, evaluate external factors, and build a SARIMAX forecasting model to predict future weekly sales and support inventory planning.  
**Tech Stack:** Python, Pandas, NumPy, Statsmodels (SARIMAX), Scikit-Learn (Metrics), Matplotlib, Seaborn.  

--- 

## 🎯 Project Architecture

* **Data Preparation:** Loaded, cleaned, and validated Walmart sales data.
* **Exploratory Data Analysis (EDA):** Analyzed sales trends, seasonality, and external factors such as unemployment and CPI using statistical analysis and visualizations.
* **Feature Engineering & Preprocessing:**  Applied a log transformation to stabilize sales variance and prepared the data for time series forecasting.
* **Forecasting Model:** Built a SARIMAX time series forecasting model and evaluated its performance using MAE, RMSE, and MAPE.
* **Business Insights:** Forecasted 12 weeks of future sales and translated results into inventory planning recommendations.

---

## 📈 Key Insights
* Weekly sales show strong annual seasonality, with demand peaking during major holiday periods.
* Holiday weeks consistently generate the highest sales throughout the year.
* Unemployment has a stronger relationship with sales than other external variables for several stores.
* Applying a log transformation stabilizes sales variance and improves forecasting performance.
* The SARIMAX model effectively captures both trend and seasonal patterns for short-term forecasting.

## 📊 Forecast Output

The final model provides:

* 12-week weekly sales forecasts
* 95% confidence intervals
* Forecast visualizations alongside historical sales
* Business-ready forecast tables for planning and analysis

## 💼 Business Value

This forecasting solution can help retailers:

* Improve inventory planning
* Reduce stock shortages during peak demand
* Minimize excess inventory costs
* Support data-driven purchasing decisions
* Enhance operational planning during seasonal demand

## 📂 Repository Structure
```text
├── walmart-dataset.csv                       # Multi-store transactional dataset
├── walmart-retails-sales-forecasting.ipynb   # Core execution analytical pipeline
└── README.md                                 # Technical project brief and insights manual
```
---

### 👤 Author
Subhankar Mondal
Data Analytics | Python | SQL | Power BI | Excel

Feel free to connect with me on LinkedIn or explore my other analytics projects.
