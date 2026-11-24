# Task 2 — Business KPI Dashboard

Interactive dashboard: `../docs/index.html` (enable GitHub Pages from branch `main`, folder `/docs`).

Filters: contract type, tenure band (0–12, 13–24, 25+ months), payment method.

KPI definitions:
- Churn rate = churned customers / all filtered customers × 100.
- Retention rate = retained customers / all filtered customers × 100.
- Monthly revenue at risk = sum of MonthlyCharges for customers marked Churn = Yes.
- Average tenure = mean TenureMonths.

Baseline (all 15 records): churn 46.67%; retention 53.33%; monthly revenue at risk 409.93 (currency unspecified); average tenure 18.8 months.

Charts: churn vs retained counts, churn rate by contract, monthly revenue at risk by payment method, average tenure by churn status.

Limitations: sample size is only 15; patterns are descriptive, not causal or statistically conclusive. Revenue at risk is a simple exposure metric, not a forecast.