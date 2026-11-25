# Task 4 — Executive Analytics Capstone

## Executive summary
This capstone combines the customer churn data-quality review, exploratory analysis, KPI dashboard definitions and transparent rule-based customer risk segmentation into a concise business story.

## What the sample shows
- Dataset size: 15 customers and 11 fields.
- Churned customers: 7 (46.67%); retained customers: 8 (53.33%).
- Monthly revenue exposure: 409.93 in source charge units, calculated as the sum of MonthlyCharges for the 7 churned customers.
- Average tenure: 18.8 months.
- Month-to-month customers in this sample all churned; customers on one-year and two-year contracts were retained.
- Average support tickets were higher among churned customers (4.29) than retained customers (1.14).
- All 15 TotalCharges values equal TenureMonths × MonthlyCharges.

## Recommended business actions
1. **Prioritize early contract check-ins.** Offer a voluntary plan/value review to month-to-month customers, especially during the first 12 months.
2. **Close the support loop.** Proactively contact customers with repeated support tickets; confirm resolution and track repeat issues.
3. **Use tenure-aware engagement.** Provide onboarding and adoption guidance for early-tenure customers, value reviews for mid-tenure customers, and renewal/loyalty touchpoints for long-tenure customers.
4. **Track results with consistent KPIs.** Review churn rate, retention rate, monthly charges associated with churned customers, and average tenure each reporting period.

## Transparent risk-score approach
A simple, interpretable rule-based score was created for prioritization:
- Month-to-month contract: +3 points.
- Tenure of 6 months or less: +2; 7–12 months: +1.
- 4 or more support tickets: +2; 2–3 tickets: +1.
- Risk bands: High = 5 or more; Medium = 3–4; Low = 0–2.

This sample produced 6 High, 1 Medium and 8 Low risk customers. The score is a prioritization heuristic, not a trained or validated predictive model.

## Expected impact and measurement
No financial uplift is claimed because the sample has no intervention history, experiment, baseline trend or verified unit currency. The expected direction is reduced avoidable churn and better retention through earlier outreach and support resolution. Measure impact by comparing churn rate, retained customer count, monthly charges associated with churn, repeat support tickets and plan conversion before and after a controlled pilot.

## Limitations
- Only 15 sample records; rates and segment patterns are highly unstable.
- The data is synthetic/sample data and may not represent a real customer base.
- Observed associations do not prove causation.
- The source does not specify currency for charge fields.
- Rule weights and risk thresholds are illustrative and require validation on a larger historical dataset with time-based train/test evaluation before operational use.

## Portfolio links
- [Task 1 — Data Quality & EDA](../Task-01-Data-Quality-EDA/)
- [Task 2 — Business KPI Dashboard source](../docs/index.html)
- [Task 3 — Segmentation & Recommendation](../Task-03-Segmentation-Recommendation/)
- [Interactive executive presentation](../docs/executive-capstone.html)
