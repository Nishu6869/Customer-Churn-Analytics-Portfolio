# Task 1 — Data Quality Summary

## Scope
Synthetic customer churn sample: 15 rows, 11 columns.

## Audit results
- Missing values: 0
- Exact duplicate rows: 0
- Duplicate CustomerIDs: 0
- IQR-flagged numeric outliers: 0
- Invalid/non-positive age values: 0
- Negative tenure, charge or support-ticket values: 0
- Churn labels outside Yes/No: 0
- TotalCharges arithmetic mismatches against TenureMonths × MonthlyCharges: 0

## Cleaning decisions
1. Trim leading/trailing whitespace from text fields.
2. No imputation was performed because no values were missing.
3. No records were removed because no exact duplicates or duplicate customer IDs were found.
4. No numeric values were capped or removed because the IQR screen did not flag outliers.
5. Preserve original valid categories and fields.
6. Keep CustomerID as an identifier, not an analytical measure.

## Initial patterns
- Churn: 7/15 = 46.67%.
- Retained: 8/15 = 53.33%.
- In this sample, all month-to-month customers churned; all one-year and two-year customers remained.
- Average support-ticket count is higher among churned customers.

## Limitations
The sample is very small (n=15), so group percentages are unstable. These observations are descriptive and do not demonstrate causation or predictive performance. The source does not specify the currency of charge fields.
