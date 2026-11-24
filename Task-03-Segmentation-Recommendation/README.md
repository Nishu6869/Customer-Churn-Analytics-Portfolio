# Task 3 — Customer Segmentation & Recommendation Model

## Deliverables
- `03_Customer_Segmentation_Risk_Model.ipynb` — reproducible notebook.
- `customer_segments_risk_recommendations.csv` — customer-level segments, scores, explanations and suggested actions.
- `risk_scoring_rules.md` — transparent scoring rubric and caveats.

## Tenure segments
- Early-tenure: 0–12 months
- Mid-tenure: 13–24 months
- Long-tenure: 25+ months

## Rule-based churn-risk score
- Month-to-month contract: +3
- Tenure 0–6 months: +2
- Tenure 7–12 months: +1
- 4+ support tickets: +2
- 2–3 support tickets: +1

Risk bands: High 5–7; Medium 3–4; Low 0–2.

## Sample results
- Segments: 6 early-tenure, 5 mid-tenure, 4 long-tenure.
- Risk levels: 6 high, 1 medium, 8 low.
- In this 15-row sample, the 6 high-risk and 1 medium-risk customers are marked churned; all 8 low-risk customers are marked retained.

## Recommendations
Early-tenure customers receive onboarding/adoption follow-up; mid-tenure customers receive value reviews; long-tenure customers receive loyalty/renewal engagement. Month-to-month customers may be offered a clear annual-plan comparison. Customers with 4+ support tickets receive proactive support review.

## Important limitations
This is a transparent heuristic, not a trained machine-learning model or calibrated probability. The rules are not validated on held-out data. The dataset contains only 15 sample records, so the apparent in-sample alignment must not be presented as predictive accuracy. Human review is required before customer actions.
