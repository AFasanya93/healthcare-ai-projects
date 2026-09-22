# Project Charter — RiskLens: AI-Driven Risk Stratification & Care Gap Closure

**Organization:** Alden Health Partners, an Accountable Care Organization (fictional)
**Sponsor:** Renee Ostrowski, Chief Care Management Officer
**Project Manager:** Priya Nandakumar
**Date:** 2026-09-22 | **Duration:** 90 days (Pilot phase, 2 care management pods)

## Background
Alden Health Partners manages ~62,000 attributed lives under value-based contracts. Care managers currently rely on monthly claims-based risk lists that lag real-world status by 4-6 weeks, and outreach is largely undifferentiated. Alden wants to pilot an AI risk-stratification and care-gap-prioritization tool that ingests near-real-time claims, pharmacy, and care-management notes to rank patients daily and recommend next-best-outreach actions, aiming to reduce avoidable ED visits and close preventive care gaps faster.

## Objectives
1. Deploy AI risk stratification + next-best-action recommendations for 2 pilot care management pods (~40 care managers, ~9,000 attributed lives).
2. Reduce average time-to-outreach for newly high-risk patients from 18 days to ≤5 days by Day 90.
3. Increase closure rate of top-3 priority care gaps (A1c testing, post-discharge follow-up, medication reconciliation) by 15 percentage points in pilot cohort vs. control pods.
4. Establish a repeatable model-monitoring process (drift, fairness/bias checks across demographic groups) before any org-wide expansion decision.

## Scope
**In scope:** 2 of Alden's 8 care management pods, AI risk score + gap recommendations surfaced inside existing care management platform (via vendor integration), care manager training, weekly model performance monitoring.
**Out of scope:** Automated patient-facing outreach (all outreach remains human-initiated this phase), integration with EHR clinical notes (claims/pharmacy/CM notes only), full 8-pod rollout (contingent on Day 90 results).

## Success Criteria
- Tool live and generating daily risk scores for both pilot pods by Day 45.
- Time-to-outreach and care-gap-closure KPIs measured weekly against a matched control pod.
- Documented fairness review showing no significant disparity in risk scoring or recommendation rates across race/ethnicity, age, or dual-eligible status.
- Expansion recommendation delivered to Alden's Value-Based Care Steering Committee by Day 90.

## Assumptions
- Vendor tool can ingest Alden's existing claims/pharmacy feeds via current data warehouse without new EDI build.
- Care managers in pilot pods can complete a half-day training without disrupting current caseload coverage.
- Compliance/Legal pre-approves the vendor's BAA and model documentation within 3 weeks of contract signature.

## Constraints
- No change to care management staffing levels during pilot — this tests prioritization, not capacity increase.
- Health plan data-sharing agreements limit which claims fields can leave Alden's environment (must stay within existing data-processing agreement scope).
- Pilot budget capped at $150,000 for the 90-day period.

## High-Level Budget
| Category | Estimate |
|---|---|
| Vendor pilot license + integration | $95,000 |
| Care manager training & change management | $20,000 |
| Fairness/bias audit (external statistician review) | $25,000 |
| Internal labor (PM, analytics, IT) | ~0.5 FTE-quarter, dept. OpEx |
| **Total incremental cash spend** | **$140,000** |

## Governance
- Steering Committee: Chief Care Management Officer (sponsor), VP Analytics, Compliance Officer, 2 Pod Supervisors — biweekly.
- Working team: PM, Data/Analytics Lead, Care Manager Champions (2), Vendor Implementation Lead, IT Integration Engineer.

## Sign-off
| Role | Name | Approved |
|---|---|---|
| Executive Sponsor | Renee Ostrowski | ☐ |
| Compliance Officer | Hector Delgado | ☐ |
| Project Manager | Priya Nandakumar | ☐ |
