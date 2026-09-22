# RAID Log — PV-Copilot

## Risks
| ID | Risk | Likelihood | Impact | Mitigation | Owner | Status |
|---|---|---|---|---|---|---|
| R1 | AI model under-codes rare/serious AE terms, causing missed signal | Medium | High | 100% human review during pilot; weekly concordance audit stratified by seriousness | PV Coder SME | Open |
| R2 | Vendor data handling doesn't satisfy Meridian's data privacy/security standards | Low | High | Legal + InfoSec review of DPA before any data transfer; de-identification enforced pre-transfer | CISO Delegate | Closed (Wk 1) |
| R3 | PV physician review capacity insufficient for pilot volume, delaying cycle-time gains | Medium | Medium | Cap pilot volume at 150 cases/week; escalation path to borrow 0.2 FTE from adjacent team | Dana Whitfield | Open |
| R4 | Regulatory Affairs raises late objection to advisory-only framing during Safety Committee review | Low | High | Involve Regulatory Affairs lead in Steering Committee from Day 1, not just at Day 90 gate | Dana Whitfield | Open |

## Assumptions
| ID | Assumption | Validation Plan | Status |
|---|---|---|---|
| A1 | Historical case data volume (8,000 cases) is sufficient for meaningful model calibration | Vendor confirms minimum viable dataset size in Week 2 | Confirmed |
| A2 | Argus Safety system will not require any configuration changes for advisory-layer integration | IT architecture review in Week 1 | Confirmed |
| A3 | QA can dedicate 20% of validation lead's time for 12 weeks | Resourcing confirmed with QA Director at kickoff | Confirmed |

## Issues
| ID | Issue | Raised | Impact | Resolution | Owner | Status |
|---|---|---|---|---|---|---|
| I1 | Historical data extract initially included 3 additional products in error | Week 2 | 2-day delay to model calibration | Re-ran extract scoped to Meridian-X only | PV Data Analyst | Resolved |
| I2 | Vendor sandbox environment had a 4-day provisioning delay due to InfoSec review backlog | Week 1 | Compressed Week 2-3 calibration window | Escalated to CISO; expedited review granted | IT Security Lead | Resolved |

## Dependencies
| ID | Dependency | Depends On | Needed By | Status |
|---|---|---|---|---|
| D1 | Model calibration | De-identified historical dataset | Week 2 | Met |
| D2 | Pilot go-live | Approved validation protocol | Week 5 | On track |
| D3 | Rollout business case | Confirmed pilot KPI results | Week 11 | Pending |
