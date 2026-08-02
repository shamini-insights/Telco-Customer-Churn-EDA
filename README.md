# Telco Customer Churn — Exploratory Data Analysis

An end-to-end exploratory data analysis (EDA) project in Python examining customer churn behavior for a telecommunications provider, using IBM's publicly released Telco Customer Churn dataset.

## 📋 Project Objective

To analyze customer churn behavior using historical customer account data — comparing churn rates across contract types, service types, and demographic groups — and to generate data-driven insights and recommendations through Python-based data visualization and analytics.

## 📊 Dataset

- **Source:** IBM Sample Data Sets — Telco Customer Churn
- **Size:** 7,043 customers, 33 attributes
- **Domain:** Telecommunications / Customer Retention
- **File:** `Telco_Customer_Churn_Dataset.csv`

The dataset includes customer demographics, account details (tenure, contract type), subscribed services (internet, streaming, security add-ons), billing information, and churn outcome.

## 🎯 Business Problem

Customer churn is one of the most significant challenges facing telecom companies, directly impacting revenue and long-term growth. This project analyzes which customer segments — by contract type, tenure, service bundle, payment method, and demographics — are most likely to churn, to support proactive, targeted retention strategies.

## 🛠️ Tools & Libraries

- **Python** (pandas, numpy)
- **Visualization:** matplotlib, seaborn, plotly
- **Environment:** Google Colab / Jupyter Notebook

## 📁 Repository Contents

| File | Description |
|---|---|
| `Telco_Customer_Churn_EDA.ipynb` | Full analysis notebook — cleaning, EDA, visualizations, insights |
| `Telco_Customer_Churn_Dataset.csv` | Raw dataset as obtained from source |
| `README.md` | Project documentation (this file) |

## 🚀 How to Run

1. Clone or download this repository
2. Open `Telco_Customer_Churn_EDA.ipynb` in [Google Colab](https://colab.research.google.com) or Jupyter
3. If using Colab, upload `Telco_Customer_Churn_Dataset.csv` to the Colab file browser (left sidebar → Files → Upload)
4. Run **Runtime → Run all** to execute the notebook top to bottom

## 🔍 Notebook Structure

1. **Data Loading and Initial Overview** — shape, dtypes, `head()`, `info()`, `describe()`
2. **Data Pre-processing** — missing values, duplicates, dtype corrections, derived columns (Tenure Group, Services Subscribed, Avg Monthly Spend, CLTV Segment)
3. **Exploratory Data Analysis** — univariate, bivariate, and multivariate analysis using groupby, pivot tables, and correlation analysis
4. **Visualizations** — 10 charts (pie, bar, histogram, box plot, scatter, heatmap, line chart, horizontal bar, multi-panel subplots, interactive Plotly scatter)
5. **Insight Generation** — key findings and business recommendations

## 💡 Key Findings

- **Overall churn rate: ~26.5%** — roughly 1 in 4 customers left
- **Contract type is the strongest churn driver** — month-to-month customers churn at ~43% vs. ~2.8% for two-year contracts
- **Fiber optic customers churn more than DSL customers**, despite being the premium service
- **First-year customers are the highest-risk segment** — churn risk drops sharply with tenure
- **Electronic check users churn more** than customers on automatic payment methods
- **Fewer add-on services correlates with higher churn** — customers with more subscribed services show greater loyalty
- **Top self-reported churn reasons** center on competitor offers and service/support dissatisfaction

## 📈 Recommendations

- Prioritize retention offers for month-to-month, fiber-optic customers within their first 12 months
- Investigate fiber optic service quality and pricing specifically
- Promote add-on service bundles to increase customer "stickiness"
- Encourage enrollment in automatic payment methods
- Use `Churn Score` and `CLTV Segment` to build a prioritized outreach list for high-value, at-risk customers

## ⚠️ Limitations

This is a cross-sectional dataset (not time-series), so findings reflect correlation rather than proven causation. `Churn Reason` is self-reported and may not capture the complete underlying cause of churn.

---

*This analysis was independently built as a final project for a Data Analysis (Python) course.*
