# Global Inflation Risk Analysis Dashboard

This project analyzes inflation risk across multiple countries using macroeconomic indicators. <br>
It demonstrates a complete **end-to-end data analytics workflow**, from data cleaning and exploratory analysis to **risk scoring and interactive visualization using Power BI**. <br>
Source of the dataset [World Bank dataset](https://data.worldbank.org/indicator), focus indicators: <br>
- CPI (Inflation, consumer prices (annual %))
- GDP growth (annual %)
- Money Supply (Broad money (% of GDP))
- Exchange Rate (Official exchange rate (LCU per US$, period average))

> ⚠️ **Disclaimer**: <br>
> The following exploratory analysis of this project is **descriptive in nature** and focuses on patterns observable directly in the data. <br>
> This project is **does not aim to provide economic policy recommendations or causal economic interpretation**.  <br>
> The primary objective is to showcase a full **data engineering, analytics, and dashboarding workflow**.

---

## Tools & Stack
- **Python**: pandas, numpy, matplotlib, seaborn
- **Power BI**: interactive dashboard for visualization & reporting

---

## Folder Structure 📂
- `notebooks/`
  - [`01_data_cleaning.ipynb`](./notebooks/01_data_cleaning.ipynb) → preprocessing & cleaning steps
  - [`02_exploratory_analysis.ipynb`](./notebooks/02_exploratory_analysis.ipynb) → exploratory data analysis (EDA)
  - [`03_feature_engineering_risk_index.ipynb`](./notebooks/03_feature_engineering_risk_index.ipynb) → feature engineering for inflation risk index
  - [`04_modeling.ipynb`](./notebooks/04_modeling.ipynb) → final dataset preparation for Power BI
  
- `data/`
  - [`raw_data/`](./data/raw_data) → raw datasets
  - [`processed/`](./data/processed) → intermediate outputs
  - [`final/`](./data/final) → Power BI-ready datasets
  
- `dashboard/`
  - [`inflation_risk_analysis_dashboard.pbix`](./dashboard/inflation_risk_analysis_dashboard.pbix) → interactive Power BI dashboard
  - [`inflation_risk_analysis_dashboard.pdf`](./dashboard/inflation_risk_analysis_dashboard.pdf) → static PDF export
  - [`dashboard_insights`](./dashboard/dashboard_insights) → written analytical insights for each dashboard page 
  - [`dashboard_pages`](./dashboard/dashboard_pages)/ → screenshots of dashboard pages
  
- `requirements.txt` → Python dependencies
- `README.md` → project documentation

---

## Project Objectives
- Clean and preprocess macroeconomic & inflation-related data  
- Explore country-level inflation patterns  
- Engineer a composite **Inflation Risk Score**  
- Compare risk patterns across **countries and regions**  
- Deliver findings through an **interactive Power BI dashboard**

---

## Dashboard Preview

### 1️⃣ **Global Overview**
  ![Global Overview](./dashboard/dashboard_pages/global_overview.png "Global Overview")
  <br>
### 2️⃣ **Country Deep-Dive**
  ![Country Deep-Dive](./dashboard/dashboard_pages/country-deep-dive.png "Country-Deep-Dive")
  <br>
### 3️⃣ **Regional Comparison**
  ![Regional Comparison](./dashboard/dashboard_pages/regional_comparison.png "Regional Comparison")
  <br>
### 4️⃣ **Data Methodology**
  ![Data Methodology](./dashboard/dashboard_pages/data_methodology.png "Data Methodology")

---

## Dashboard Insights (Written Analysis)

Each dashboard page is accompanied by a dedicated written analytical summary:

- [`01_global_overview.md`](./dashboard/dashboard_insights/01_global_overview.md)  
- [`02_country_deep_dive.md`](./dashboard/dashboard_insights/02_country_deep_dive.md)  
- [`03_regional_comparison.md`](./dashboard/dashboard_insights/03_regional_comparison.md)  
- [`04_data_methodology.md`](./dashboard/dashboard_insights/04_data_methodology.md)  

These files explain **what the visuals show, how the Risk Score is constructed, and how to interpret the observed patterns**.

---

## Key Deliverables

- Fully automated data preprocessing pipeline (Python)
- Composite Inflation Risk Index (z-score based, weighted, min–max scaled)
- Interactive multi-page Power BI dashboard
- Written analytical interpretation for each dashboard page
- Transparent treatment of missing data and imputation methods
