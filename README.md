
# CX Performance Dashboard & Automation Strategy (Namma Yatri Case Study)

A formula-driven Excel dashboard and written analysis of a year (2025) of contact-centre data for a mobility app. It diagnoses why most callers were not getting through, models the staffing gap, and sizes the opportunity to deflect contacts through self-serve and automation.

Built as a Customer Experience & Strategy case study (data analysis plus automation strategy).

---

## Headline findings (FY 2025)

| Metric | Value |
|--------|-------|
| Calls offered | 1,339,160 |
| Calls answered | 564,643 |
| Answer rate (answered / offered) | 42.2%, falling to 28.8% in December |
| Repeat call share | 61.2% in Dec (54.1% for the year) |
| Contacts per 1,000 rides | 16.0 in April, 37.2 in December |
| Reported FCR / CSAT | 78.2% / 88.8% |
| Average handle time | 192 sec |
| Peak staffing gap | 37.8 FTE at an 85% answer-rate target (scenario) |
| Automation opportunity | about 263,000 contacts a year (scenario estimate) |

**The story in brief**

1. **Capacity ceiling, not an agent problem.** Demand grew 70% from H1 to H2, but answered calls stayed capped at about 50,000 a month.
2. **The queue is consuming itself.** Unanswered contacts come back as repeat calls, which are now over 60% of volume.
3. **One issue drives a quarter of contacts.** "Not getting rides" is 23.1% of all tagged contacts and grew 32% H1 to H2. It is an information gap that an in-app diagnostic could address.
4. **Two metrics contradict each other.** Reported FCR improved in the same months repeat calls rose, so FCR needs re-measuring from contact-level data.
5. **The cause sits upstream of support.** Contacts per 1,000 rides more than doubled while rides declined slightly.

## What is in the workbook

| Tab | Contents |
|-----|----------|
| 01 Read Me | Structure, method, assumptions, and data limitations |
| 02 Dashboard | 12 KPI tiles, six key takeaways, a priority-ranked recommendation table, top 5 contact drivers, and 8 charts |
| 03 Call Trend Analysis | Source metrics plus derived metrics (answer rate, abandon, repeat share, occupancy, contact rate) |
| 04 Capacity Model | Required vs actual headcount, staffing gap, and the cost of closing it by hiring |
| 05 Issue Analysis | Pareto of 119 issue tags, H1 vs H2 movement, queue split, and new H2 tags |
| 06 Automation Opportunity | Deflection sizing per issue with levers, agent hours and cost released, plus a 5-phase roadmap |
| 07 Findings & Actions | 12 findings with evidence, implication, action, owner, metric and priority, plus a 30-60-90 day plan |
| 08 / 09 Data | Source data (Call Trend and Issue Types) exactly as supplied |

**Built with:** Excel formulas (880+ live formulas, no hardcoded results), 8 charts, scenario inputs.

## Method

- Every calculated cell is a live formula that references the data tabs, so replacing the data makes the whole workbook update.
- Colour convention: blue text on yellow = editable assumption, green = link to another sheet, purple = derived metric, black = source value.

## Assumptions (scenarios, not observed results)

- Target answer rate of 85% (analyst-set benchmark).
- 8-hour shift, 70% occupancy, 26 working days a month.
- INR 35,000 fully loaded cost per agent per month.
- Deflection rates of 35% to 90% by lever. Projected savings are a scenario, not booked savings.
- Contacts were mapped to Driver or Customer Support queues from the tag name, since the source has no queue field.

All of these are editable in the workbook.

## Data limitations found

- "SL %" in the source is an answer rate (answered / offered), not a true service level.
- The in-scope SL definition changes in Q1, so Jan to Mar values do not reconcile with later months.
- Issue tags cover answered calls only (560,258 tagged against 1,339,160 offered), so the issue mix is biased toward answered calls.
- The Total row under-counts the sum of its own rows by 16 contacts.
- There is no AHT, CSAT or FCR split by queue or tag, so per-issue cost figures are indicative.
- The tag taxonomy has 119 tags, including duplicates and generic buckets.

## Recommendations (summary)

| Priority | Recommendation |
|----------|----------------|
| P0 | Demand-based workforce planning with a published capacity ceiling |
| P0 | Track repeat calls by original issue and run a weekly root-cause review |
| P0 | Ship an in-app supply diagnostic for the largest contact driver |
| P0 | Separate escalation path for safety and conduct contacts |
| P1 | Rebuild FCR from contact-level data (same user, same issue, 72 hours) |
| P1 | Rebuild the taxonomy as six L1 themes with L2 sub-reasons |
| P1 | Add a Product-CX launch-readiness gate before new features ship |

The full list, with owners and metrics, is in tab 07, along with a 30-60-90 day plan.

## How to use

1. Download `CX_Dashboard_2025.xlsx` and open it in Excel.
2. Start on **02 Dashboard** for the overview.
3. Change the yellow cells in tabs 04 and 06 to test different staffing and deflection scenarios.

## Screenshots

![Dashboard overview](screenshots/overview.png)
![Charts](screenshots/charts.png)

## Author

Ajeet Kumar Singh ([@Ajeetku07](https://github.com/Ajeetku07))
