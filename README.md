# Customer Churn Analytics Portfolio

End-to-end customer churn analytics portfolio using Python and Power BI.

## Project roadmap
- **Task 1 — Data Quality & Exploratory Analysis:** completed analysis artifacts are in `Task-01-Data-Quality-EDA/`.
- **Task 2 — Business KPI Dashboard:** upcoming.
- **Task 3 — Segmentation & Recommendation Model:** upcoming.
- **Task 4 — Executive Analytics Capstone:** upcoming.

## Task 1 contents
- `01_Customer_Churn_EDA.ipynb` — reproducible data audit, cleaning, validation and EDA.
- `customer_churn_sample.csv` — supplied synthetic source dataset.
- `cleaned_customer_churn.csv` — cleaned analysis-ready dataset.
- `data_dictionary.csv` — field definitions.
- `data_quality_summary.md` — cleaning decisions, findings and limitations.

## Run the notebook
1. Open the Task 1 folder in Jupyter Notebook or JupyterLab.
2. Install dependencies: `pip install pandas numpy matplotlib`.
3. Open and run `01_Customer_Churn_EDA.ipynb` from top to bottom.

## Initial sample findings
- 15 records and 11 columns.
- No missing values, exact duplicate rows or duplicate customer IDs.
- Sample churn: 7 of 15 customers (46.67%); retention: 8 of 15 (53.33%).
- No numeric outliers flagged by the 1.5×IQR screening rule.
- TotalCharges equals TenureMonths × MonthlyCharges in all 15 rows.

## Important limitation
This is a very small synthetic dataset. Findings are descriptive, not causal or statistically conclusive. The source does not specify a currency for charge fields. No customer-level sensitive information is included in this portfolio sample.
