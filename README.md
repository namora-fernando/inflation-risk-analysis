# Inflation Risk Analysis (WIP)

🚧 Work In Progress 🚧  
This project focuses on analyzing inflation risk across multiple countries. <br>
The goal is to build a data pipeline, perform exploratory analysis, create risk scoring features, and finally deliver insights through a Power BI dashboard.

> ⚠️ **Disclaimer**: <br>
> The following exploratory analysis of this project is descriptive in nature. We focus on patterns directly observable in the data, without attempting deeper economic interpretation (as this project is aimed at data workflow demonstration rather than economic research).

---

## Tools & Stack 🛠️
- **Python**: pandas, numpy, matplotlib, seaborn
- **Power BI**: interactive dashboard

---

## Folder Structure 📂
- `notebooks/`
  - [`01_data_cleaning.ipynb`](./notebooks/01_data_cleaning.ipynb) → preprocessing & cleaning steps
  - [`02_exploratory_analysis.ipynb`](./notebooks/02_exploratory_analysis.ipynb) → exploratory data analysis (EDA)
  - [`03_feature_engineering_risk_index.ipynb`](./notebooks/03_feature_engineering_risk_index.ipynb) → feature engineering for risk index
  - [`04_modeling.ipynb`](./notebooks/04_modeling.ipynb) → preparation for Power BI friendly
- `data/`
  - [`raw_data/`](./data/raw_data) → raw datasets
  - [`processed/`](./data/processed) → intermediate outputs
- `dashboard/` → Power BI dashboard & screenshots
  - [`inflation_risk_analysis_dashboard.pbix`](./dashboard/inflation_risk_analysis_dashboard.pbix)
  - [`inflation_risk_analysis_dashboard.pdf`](./dashboard/inflation_risk_analysis_dashboard.pdf) → pdf export of pbix
  - dashboard_insights/ → insights of dashboards
  - [`dashboard_pages`](./dashboard/dashboard_pages)/ → screenshots of dashboards
- `requirements.txt` → Python dependencies
- `README.md` → project documentation

---

## Objectives
- Clean and preprocess macroeconomic & inflation-related data  
- Explore country-level inflation patterns  
- Engineer features to quantify inflation risk exposure  
- Visualize findings through Power BI dashboard

---

## Screenshots of Dashboard Pages
- 1️⃣ **Global Overview**
  ![global_overview.png](./dashboard/dashboard_pages/global_overview.png "Global Overview")
- 2️⃣ **Country-Deep-Dive**
  ![country-deep-dive.png](./dashboard/dashboard_pages/country-deep-dive.png "Country-Deep-Dive")
- 3️⃣ **Regional Comparison**
  ![regional_comparison.png](./dashboard/dashboard_pages/regional_comparison.png "Regional Comparison")
- 4️⃣ **Data Methodology**
  ![data_methodology.png](./dashboard/dashboard_pages/data_methodology.png "Data Methodology")

---

## Next Steps 📌
- Complete the modeling stage (Notebook 04)  
- Build and publish Power BI dashboard  
- Add final report & insights summary  
