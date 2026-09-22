# RAID Log — RiskLens

## Risks
| ID | Risk | Likelihood | Impact | Mitigation | Owner | Status |
|---|---|---|---|---|---|---|
| R1 | Model shows scoring disparity across demographic groups (e.g., under-flags dual-eligible members) | Medium | High | Baseline + mid-pilot + final fairness audits by independent statistician; documented remediation threshold before go-live continues | External Statistician | Open |
| R2 | Care manager adoption is low (recommendations ignored, reverting to old workflow) | Medium | Medium | Champions model, weekly feedback sessions, recommendation-relevance tuning in Weeks 6-7 | Care Manager Champions | Open |
| R3 | Data feed latency (claims lag) undermines "near-real-time" value proposition | Medium | Medium | Set realistic latency expectations (claims lag ~7-10 days is inherent); supplement with CM notes for recency | Data/Analytics Lead | Open |
| R4 | Control pod contaminated (care managers informally share pilot recommendations across pods) | Low | Medium | Explicit instruction in training; control pod supervisor briefed on importance of isolation | Priya Nandakumar | Open |

## Assumptions
| ID | Assumption | Validation Plan | Status |
|---|---|---|---|
| A1 | Existing data warehouse feeds are sufficient without new EDI build | IT integration scoping in Week 1-2 | Confirmed |
| A2 | 40 care managers across 2 pods can complete training without caseload disruption | Scheduling confirmed with pod supervisors | Confirmed |
| A3 | Matched control pod is statistically comparable in acuity/demographic mix | Analytics team comparability check, Week 2 | Confirmed |

## Issues
| ID | Issue | Raised | Impact | Resolution | Owner | Status |
|---|---|---|---|---|---|---|
| I1 | Pharmacy feed had a schema mismatch causing incomplete medication history for ~8% of members | Week 2 | Delayed baseline model run by 3 days | Vendor patched mapping; re-ran affected records | IT Integration Engineer | Resolved |
| I2 | Baseline fairness review flagged mild under-scoring for members 75+ | Week 3 | Required model recalibration before go-live | Vendor adjusted age-related feature weighting; re-validated | External Statistician | Resolved |

## Dependencies
| ID | Dependency | Depends On | Needed By | Status |
|---|---|---|---|---|
| D1 | Model baseline run | Data feed connectivity | Week 3 | Met |
| D2 | Go-live | Passed fairness baseline + completed training | Week 5 | On track |
| D3 | Expansion business case | Confirmed KPI improvement vs. control | Week 11 | Pending |
