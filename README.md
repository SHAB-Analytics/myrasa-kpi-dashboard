# MyRasa SmartMart KPI Dashboard (interactive demo)

**Live dashboard:** https://shab-analytics.github.io/myrasa-kpi-dashboard/

## The question

MyRasa SmartMart, a Malaysian neighbourhood grocer, has invested in five smart-store pilots: self-checkout kiosks, a shopping app, click-and-collect, trained SmartStore Hosts and opt-in personalisation. At the month-9 review, management has to decide: **scale the strategy to more outlets, keep testing, or pause?**

This dashboard shows how that decision would be made using a KPI framework of **six KPIs, four guardrails and agreed green / amber / red rules**, comparing the 5 pilot outlets with matched comparison outlets.

## What you can explore

- **Hover** over any chart to see the pilot and comparison values for that week or month.
- **Compare periods:** the shaded area on each chart is the 12-week baseline before the pilot started.

## Dashboard views

- **Decision gate:** the overall status (Green / Amber / Red) and the three tests behind it.
- **Six KPI cards:** smart task completion, checkout time (slowest 10%), customer effort, service recovery, 90-day repeat purchase, and contribution per outlet. Each card shows its result, target and status.
- **Pilot vs comparison trends:** six charts over the baseline and the 36-week pilot.
- **Guardrail table:** system availability, price accuracy, privacy complaints and staffed-lane cover, with weeks held and breaches.

## Key findings (demo scenario)

- **The gate is Green.** 5 of 6 KPIs meet target, contribution is **+RM 1.9k per outlet per month** above comparison stores, and all four guardrails have held for 8+ weeks.
- **One miss is allowed.** Customer effort improved by +3.9 points against a +5 target, so the decision rules still permit scaling, while flagging an area to fix.
- **Early losses are expected.** Contribution dips in months 1–2 (set-up and training costs) before overtaking comparison stores, which is why the decision waits until month 9.
- **Guardrails can veto growth.** An outage (week 6) and a privacy-complaint spike (week 8) were fixed. Had either still been breached, the gate would be Red regardless of sales.

## Method

- **Difference-in-differences:** each KPI's effect = (pilot change) − (comparison change), so promotions and festive seasons that affect all stores are not credited to the strategy.
- **Baseline:** 12 weeks before the pilot. "Now" = the last 12 weeks (months 7–9). Repeat purchase uses months 4–6, the latest cohorts whose 90-day window has closed.
- **Targets are illustrative:** in practice they would be set only after the baseline is collected.

> ⚠️ **All figures are hypothetical.** They were invented to show how management would use the framework. They are not findings from the case and not forecasts.

## Technology

A single self-contained HTML page built with **D3.js**, with all data embedded. View it at the live link above, or download `index.html` and open it in any browser. It works offline.

## Source

Based on *"Transforming the Malaysian Retail Experience through Smart Retailing: A Strategic Marketing Challenge for MyRasa SmartMart"*. The case itself is not included; this repository contains only the author's analysis.

Prepared by **Shabnam Mohammed Sameer**.
