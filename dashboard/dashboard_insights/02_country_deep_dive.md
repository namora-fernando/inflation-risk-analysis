# Country Deep Dive Analysis

This page focuses on a single selected country and examines how its inflation risk is formed and how it evolves over time. The example shown in this view is based on **Venezuela (2003)**, but all insights dynamically update with the country and year slicers.

---

## Purpose of This Page

The objective of this page is to:
- Understand how inflation risk behaves over time for a specific country.
- Break down the macroeconomic drivers that contribute most to the country’s inflation risk.
- Connect short-term economic shocks with long-term structural risk patterns.

This page is designed to move from a global perspective into a detailed country-level diagnosis.

---
## Dashboard Preview
![Country Deep-Dive](../dashboard_pages/country-deep-dive.png "Country-Deep-Dive")

---

## Key Economic Snapshot (Selected Country and Year)

For the selected country (Venezuela, 2003), the dashboard displays:

- **Risk Score:** 100.00  
  This is the maximum possible value on our 0–100 scale for that year.  
  A score of 100 means that, in 2003, Venezuela is the **riskiest country in the world** according to our composite risk index (built from CPI, exchange rate change, money-supply change, and inverted GDP growth).

- **CPI Annual Change:** 27.08%  
  Inflation was already elevated, reflecting rapid consumer price increases.

- **Exchange Rate Change (YoY):** 38.42%  
  Strong currency depreciation pressure is visible in this year.

- **Money Supply Growth (YoY):** 30.48%  
  Rapid monetary expansion suggests accommodative or unstable monetary conditions.

- **GDP Annual Growth:** -7.76%  
  In our risk model, GDP growth enters with an inverted sign, so a deep contraction like this increases the composite risk score rather than reducing it.

This snapshot reflects a combination of high inflation, currency instability, aggressive money growth, and economic recession.

---

## Risk Score Trend Over Time

The time series of the **Risk Score across all years** shows that:
- Risk spikes tend to appear around periods of economic instability and macroeconomic shocks.
- The Risk Score over time shows that inflation risk is persistently elevated rather than a one-off spike.
- There are multiple crisis episodes where the score jumps sharply, and even in non-crisis years the country rarely returns to a clearly “low-risk” zone.

This suggests that inflation risk is not a temporary event for the selected country but a recurring structural issue.

> The series stops in the mid-2010s due to missing values in later years, but the final observed period already reflects very elevated risk levels.

---

## Which Indicator Affects Risk the Most?

The standardized indicator trends (z-scores) reveal:
- **CPI volatility** and **money supply growth** exhibit the strongest upward deviations during high-risk periods.
- **Exchange rate volatility** shows frequent sharp swings, often aligning with risk surges.
- **GDP growth (inverted)** contributes through persistent periods of weak or negative growth: when the economy shrinks, the inverted GDP term pushes the risk index higher.

This confirms that inflation risk is typically driven by a combination of:
- Price instability
- Currency pressure
- Monetary expansion
- Weak real economic performance

---

## Contribution of Each Risk Driver

The weighted contribution chart shows the relative importance of each indicator in forming the composite risk score:

- **CPI (Inflation):** The dominant contributor to total risk.
- **Exchange Rate:** The second most influential factor.
- **Money Supply:** A moderate but consistent contributor.
- **GDP (Inverted):** A smaller but still meaningful contributor.

This weighting structure ensures that inflation dynamics remain the primary signal of risk, while macro-financial instability reinforces the final score.

---

## Key Takeaways

- Inflation risk for the selected country is structurally high rather than temporary.
- High CPI growth and exchange rate instability are the main risk amplifiers.
- Monetary expansion consistently reinforces inflationary pressure.
- Economic contraction further exacerbates overall inflation risk.
- The composite risk score effectively captures both price instability and broader macroeconomic fragility.

---

*This page provides the foundation for interpreting country-specific inflation risk before comparing patterns across regions.*
