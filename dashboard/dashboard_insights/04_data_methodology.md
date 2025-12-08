# Data Quality and Risk Index Methodology

This page documents how the inflation risk index is constructed and how missing values are treated before visualization in Power BI. It provides transparency on the reliability, transformations, and assumptions behind the final Risk Score.

---

## Dashboard Preview
![Data Methodology](../dashboard_pages/data_methodology.png "Data Methodology")

---

## 1. Missing Data Overview

The bar chart **"Missing % by Indicator"** summarizes how much of each core indicator contains missing values across the dataset:

- **Money Supply (% Change YoY)** shows the highest missing share (above 20%).
- **CPI Inflation** has a moderate level of missing values.
- **Exchange Rate (% Change YoY)** contains only a small fraction of missing observations.
- **GDP Growth** has the lowest missing share.

This pattern indicates that liquidity-related indicators are more fragmented across countries, while price- and output-related data are generally more complete.

---

## 2. Imputed Share by Country

The table **"Imputed Share by Country"** shows the proportion of values that were filled through imputation for each country and indicator:

- Countries highlighted in darker colors rely more heavily on imputed data.
- Some economies depend primarily on imputation for **Money Supply** and **CPI**.
- A number of countries still retain mostly original observations with very low imputation shares.

This table allows users to directly assess **how much each country’s Risk Score depends on reconstructed values rather than original observations**.

---

## 3. Risk Index Construction

### Inputs

The composite inflation risk index is constructed from four core indicators:

- CPI annual inflation (%)
- Exchange rate change vs USD (% YoY)
- Money supply as % of GDP and its YoY change
- Real GDP growth (%)

### Transformations and Outliers

- CPI, exchange rate change, and money supply growth are **log(1 + x) transformed** to reduce skewness.
- These transformed variables are then **winsorized annually at the 1st–99th percentiles** to limit extreme outliers.
- GDP growth is only winsorized (without log transformation), as its distribution is more symmetric.

### Standardization and Weighting

- After transformation, all indicators are converted into **z-scores**.
- Weights are assigned as follows:
  - CPI: 0.40  
  - Exchange Rate: 0.25  
  - Money Supply: 0.20  
  - GDP (inverted): 0.15  

- The composite Risk Index is calculated as a weighted sum of these standardized components.

---

## 4. Scaling and Risk Categorization

- The composite index is **min-max scaled to a 0–100 Risk Score within each year**.
- Risk categories are defined using cross-sectional percentiles:
  - **Low Risk:** below the 33rd percentile  
  - **Medium Risk:** between the 33rd and 66th percentiles  
  - **High Risk:** above the 66th percentile  

This ensures that risk is measured **relatively across countries each year**, rather than against fixed absolute thresholds.

---

## 5. Missing Data Imputation Policy

- Short gaps (up to 2 years) are interpolated linearly.
- Longer gaps use a forward–backward fill strategy.
- Remaining missing values are intentionally left as blanks.

The **“filled” flag from the engineering stage** and the imputation visualizations on this page indicate **how much the final index depends on estimated values**.

---

## 6. Notes on Interactivity

Although this page currently shows results with **Region = All** and **Year = All**, users may optionally:

- Select a specific **region** to inspect localized data quality patterns.
- Select a specific **year** to observe how missingness and imputation evolve over time.

All visuals on this page update dynamically based on these slicer selections.

---

*This methodology page ensures that the Risk Score used throughout the dashboard is reproducible, transparent, and auditable.*
