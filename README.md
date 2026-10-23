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
- Rate comes from the tier table (Lite Engagement 5–20 hrs $189, Part-Time 21–29 hrs $180, Full-Time 30–40 hrs $174), editable in the page
- Contract term discount (monthly, 6 or 12 months) is applied to the hourly rate
- 1099 cost can be one consultant or a blended team of roles (% of hours × $/hr)
- Delivery cost = 1099 cost × hours actually delivered
- Contribution margin = (revenue − 1099 cost − overhead) ÷ revenue
- Floor rate = (1099 cost + overhead) × % delivered ÷ (1 − target margin)

## Notes

- Edits made on the page (inputs, tiers, clients, market data) are saved in each person's own browser only. Use **Backup & restore** to move them between devices.
- This repository is public, so anyone can see the default rates and costs in the code.
