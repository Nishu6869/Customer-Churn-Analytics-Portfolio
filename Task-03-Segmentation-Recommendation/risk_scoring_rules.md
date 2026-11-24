# Rule-Based Risk Scoring Rubric

| Input signal | Rule | Points |
|---|---|---:|
| ContractType | Month-to-Month | +3 |
| TenureMonths | 0–6 months | +2 |
| TenureMonths | 7–12 months | +1 |
| SupportTickets | 4 or more | +2 |
| SupportTickets | 2–3 | +1 |
| Other values | No listed risk signal | 0 |

## Risk bands
- High: 5–7 points
- Medium: 3–4 points
- Low: 0–2 points

## Segmentation
- Early-tenure: 0–12 months
- Mid-tenure: 13–24 months
- Long-tenure: 25+ months

## Human-readable recommendations
- Early-tenure: onboarding and product-adoption check-in.
- Mid-tenure: value review and unmet-needs discussion.
- Long-tenure: loyalty or renewal engagement.
- Month-to-month: offer a clear annual-plan comparison without pressure.
- 4+ support tickets: proactive support follow-up and repeat-issue review.
- 2–3 support tickets: check resolution of open support issues.

## Guardrails
The score is an uncalibrated heuristic for prioritizing review. It is not a churn probability, causal model, or validated predictor. Do not automate adverse decisions based on it. Test and recalibrate with a substantially larger dataset and held-out validation before operational use.
