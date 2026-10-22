# Catalyst IQ Labs – AMS Margin Calculator

A pricing and margin calculator for Catalyst IQ Labs' managed Workday support (AMS) subscriptions.

**Live site:** published with GitHub Pages from `index.html` on the `main` branch.

## What's in here

| File | What it is |
|---|---|
| `index.html` | The whole web calculator: Calculator, Tier comparison and Client portfolio tabs. One file, no setup needed. |
| `Catalyst_IQ_Labs_AMS_Margin_Calculator_Weekly_-_V2.xlsx` | The Excel version with the same math. |

## How the math works

- Monthly revenue = client rate × weekly contracted hours × (billable weeks ÷ 12)
- Rate comes from the tier table (Small 5–20 hrs $189, Mid 21–29 hrs $179, Large 30–40 hrs $169), editable in the page
- Delivery cost = 1099 cost × hours actually delivered
- Contribution margin = (revenue − 1099 cost − overhead) ÷ revenue
- Floor rate = (1099 cost + overhead) × % delivered ÷ (1 − target margin)

## Notes

- Edits made on the page (inputs, tiers, clients) are saved in each person's own browser only.
- This repository is public, so anyone can see the default rates and costs in the code.
