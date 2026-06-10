# 📊 Walmart Retail Sales Analysis & Forecasting Pipeline

**Author:** Subhankar Mondal  
* **Business Problem:** A major national retail brand with multiple outlets faces significant supply chain and inventory management mismatches. Outlets frequently struggle to align supply with localized customer demand, leading to costly stockouts of high-demand items and steep holding fees for overstocked merchandise.
**Objective:** Build an end-to-end data analytics and predictive pipeline to resolve retail inventory management mismatches by analyzing historical economic drivers and forecasting multi-week store-level sales trajectories.  
**Tech Stack:** Python, Pandas, Numpy, Statsmodels (SARIMAX), Scikit-Learn (Metrics), Matplotlib, Seaborn

---

## 🎯 Project Architecture

This repository contains a production-grade time-series engineering framework designed to model seasonal demand patterns, account for macroeconomic covariates, and generate mathematically stable forward-looking revenue forecasts.

1. **Environment & Data Ingestion:** Streamlined data pipeline to ingest multi-variable store transaction matrices with systematic validation checks.
2. **Data Quality & Anomaly Detection:** Programmatic anomaly and extreme-outlier filtering utilizing a robust Interquartile Range ($IQR$) filtering threshold.
3. **Statistical Exploratory Data Analysis (EDA):** Granular correlation tracking against external macroeconomic indicators (Unemployment, CPI inflation, Temperature) alongside classical additive/multiplicative time-series decomposition.
4. **Stationarity & Variance Stabilization:** Automated variance dampening via log transformation and stationarity validation using the Augmented Dickey-Fuller (ADF) test framework.
5. **Predictive Modeling Engine:** Rigorous hyperparameter tuning and optimization for a Seasonal Autoregressive Integrated Moving Average with Exogenous Regressors (**SARIMAX**) pipeline.
6. **Evaluation & Horizon Deployment:** Out-of-sample backtesting via mean metrics ($MAE$, $RMSE$, $MAPE$) mapped back to the raw financial currency scale, culminating in a 12-week operational forecasting dashboard.

---

## 📂 Repository Structure
```text
├── walmart-dataset.csv               # Multi-store transactional log dataset
├── walmart-retails-sales-forecasting.ipynb   # Core execution analytical pipeline 
└── README.md                         # Technical project brief and insights manual
```

## 📌 Operational Insights & Actionable Business Takeaways
### 📈 Executive Analytical Summary
Transitioning retrospective sales tracking into an active statistical prediction engine converts historic data into proactive operational indicators. The framework maps future scale targets surrounded safely by a 95% demand uncertainty horizon.

## 🔍 Key Operational Insights & Business Use-Cases
### 🚀 1. Macro-Demand Velocity (Supply Chain & Inventory Buffer Strategy)
* **The Insight:** The forecasting engine projects distinct seasonal surge velocity patterns, highlighting high-volume sales intervals weeks before they happen.
* **Business Application:** Inventory replenishment managers can utilize these automated target volumes to proactively establish localized buffer stocks, mitigating out-of-stock risks on fast-moving consumer goods and streamlining warehouse inbound cargo flows.
### 📅 2. Holiday Cycle Trajectories (Workforce & Capacity Optimization)
* **The Insight:** By tracking annual seasonality fluctuations, the pipeline maps explicit revenue spikes followed by sharp operational slowdowns.
* **Business Application:** Store operational directors can leverage these cyclical trend points to dynamically scale seasonal associate hiring, optimization checkout lane availability, and schedule routine maintenance operations during low-velocity intervals.
### 🛡️ 3. Risk Mitigation via Certainty Envelopes (Financial Stress Testing)
* **The Insight:** The integration of shaded upper and lower confidence boundaries establishes a rigorous margin-of-error matrix.
* **Business Application:** Executive leadership can avoid the common mistake of budgeting overhead costs purely against single midpoint forecasts. Instead, labor models and emergency cash reserves should be stress-tested against the Lower Boundary Limit to protect profitability margins under worst-case demand drops.

## 🏃‍♂️ How To Run and Reproduce
- Clone this repository to your local computer:
```git clone "https://github.com/subhankar0296/walmart-sales-forecasting.git"```
- Place the file ```walmart-dataset.csv``` inside the root folder alongside the notebook.
- Install the required dependency frameworks:
```pip install pandas numpy statsmodels matplotlib seaborn scikit-learn```
- Run all cells in ```walmart-retails-sales-forecasting.ipynb``` to regenerate the interactive graphics and performance evaluation metrics.
