# E-Commerce-User-Behavior-Analytics-A-B-Testing-Engine

## 1. Project Overview

This project investigates how users interact with an e-commerce website, from browsing products to completing a purchase.

The goal is to identify customer journey drop-offs, understand user behavior, measure retention, analyze purchasing patterns, and evaluate whether a proposed product change improves conversion.

The project combines SQL, Python, statistical analysis, and Power BI into a reproducible analytics workflow.

## 2. Business Problem

An e-commerce business needs to understand:

- Where do users drop off during the purchase journey?
- How do browsing, cart additions, checkout, and purchasing relate?
- Which user segments have different engagement or conversion patterns?
- How many users return after their first observed activity?
- Does a proposed website change improve purchase conversion?
- What actions should the business investigate or test next?

## 3. Dataset

**Source:** Google Analytics 4 sample e-commerce dataset

Dataset:
`bigquery-public-data.ga4_obfuscated_sample_ecommerce`

Official documentation:
https://developers.google.com/analytics/bigquery/web-ecommerce-demo-dataset

The dataset contains event-level web analytics data, including product views, cart additions, checkout events, purchases, and other website interactions.

### Initial data profile

| Metric | Initial result |
|---|---:|
| Total event records | 4,295,584 |
| Distinct user identifiers | 270,154 |
| Observed event dates | 92 |
| Events without user identifiers | 0 in the initial event-type summary |

These are initial query results, not final business KPIs. Further validation and metric definitions are required.

The source dataset is obfuscated, and its values may have limitations. Findings will be interpreted accordingly.

## 4. Analytical Workflow

1. **Data exploration:** Inspect event types, schema, identifiers, timestamps, and relevant event parameters.
2. **Data quality:** Check missing values, duplicate records, timestamp consistency, and purchase-related fields.
3. **SQL analytics:** Build user-level and session-level metrics, funnel analysis, cohort retention, and segment comparisons.
4. **Python analysis:** Validate query results, perform exploratory analysis, and calculate statistical measures.
5. **A/B testing:** Analyze a separately documented experiment dataset with explicit treatment assignment and conversion outcomes.
6. **Power BI:** Present key metrics, conversion funnels, retention patterns, and experiment results.
7. **Business recommendations:** Translate supported findings into actionable next steps, limitations, and proposed follow-up tests.

## 5. Technology Stack

- SQL and Google BigQuery
- Python
- pandas and NumPy
- Statistical analysis
- Power BI
- Git and GitHub

Additional libraries and tools will be documented as they are used.

## 6. Planned Deliverables

- Reproducible SQL queries
- Python notebooks and validation checks
- Defined KPI formulas and data dictionary
- Interactive Power BI dashboard
- A/B testing analysis with uncertainty estimates
- Findings and recommendations report
- Documentation of limitations and assumptions

## 7. Validation and Integrity

Metrics will use explicit definitions and denominators. SQL and Python outputs will be compared where applicable.

The historical e-commerce dataset will not be treated as a randomized experiment. Any simulated experiment data will be labelled clearly, and simulated results will not be presented as real company outcomes.

## 8. Current Progress

- [x] Connected to the public dataset and ran a baseline query.
- [x] Summarized event volumes and distinct users by event type.
- [ ] Validate event sequences and session boundaries.
- [ ] Build and validate the conversion funnel.
- [ ] Analyze retention and customer segments.
- [ ] Inspect purchase and revenue fields.
- [ ] Perform A/B testing on a documented experiment dataset.
- [ ] Build the Power BI report.
- [ ] Complete findings, screenshots, and reproducibility documentation.

## 9. Expected Outcome

The completed project will demonstrate how raw behavioral data can be transformed into validated analytical metrics, visual reports, statistical evidence, and business recommendations.

All conclusions will be based on the actual analysis, with assumptions and limitations documented.
