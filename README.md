# Inflation Risk Analysis (WIP)

🚧 Work In Progress 🚧  
This flagship portfolio project focuses on analyzing inflation risk across multiple countries.  
The goal is to build a data pipeline, perform exploratory analysis, create risk scoring features, and finally deliver insights through a Power BI dashboard.

> ⚠️ **Disclaimer**:
> The following exploratory analysis of this project is descriptive in nature. We focus on patterns directly observable in the data, without attempting deeper economic interpretation (as this project is aimed at data workflow demonstration rather than economic research).

---

## Tools & Stack 🛠️
- **Python**: pandas, numpy, matplotlib, seaborn
- **Power BI**: interactive dashboard *(WIP)*

---

## Folder Structure 📂
- `notebooks/`
  - [`01_data_cleaning.ipynb`](https://github.com/namora-fernando/inflation-risk-analysis/blob/main/notebooks/01_data_cleaning.ipynb) → preprocessing & cleaning steps
  - [`02_exploratory_analysis.ipynb`](https://github.com/namora-fernando/inflation-risk-analysis/blob/main/notebooks/02_exploratory_analysis.ipynb) → exploratory data analysis (EDA)
  - [`03_feature_engineering_risk_index.ipynb`](https://github.com/namora-fernando/inflation-risk-analysis/blob/main/notebooks/03_feature_engineering_risk_index.ipynb) → feature engineering for risk index
  - [`04_modeling.ipynb`](https://github.com/namora-fernando/inflation-risk-analysis/blob/main/notebooks/04_modeling.ipynb) → preparation for Power BI friendly
- `data/`
  - [`raw_data/`](https://github.com/namora-fernando/inflation-risk-analysis/tree/main/data/raw_data) → raw datasets
  - [`processed/`](https://github.com/namora-fernando/inflation-risk-analysis/tree/main/data/processed) → intermediate outputs
- `reports/`
  - `dashboard/` *(WIP)* → Power BI dashboard & screenshots
- `requirements.txt` → Python dependencies
- `README.md` → project documentation

---

## Objectives
- Clean and preprocess macroeconomic & inflation-related data  
- Explore country-level inflation patterns  
- Engineer features to quantify inflation risk exposure  
- Visualize findings through Power BI dashboard  → *(WIP)*

---

## Next Steps 📌
- Complete the modeling stage (Notebook 04)  
- Build and publish Power BI dashboard  
- Add final report & insights summary  
