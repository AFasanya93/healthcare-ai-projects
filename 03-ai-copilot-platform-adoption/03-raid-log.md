# RAID Log — ScribeOS

## Risks
| ID | Risk | Likelihood | Impact | Mitigation | Owner | Status |
|---|---|---|---|---|---|---|
| R1 | Patient declines consent at meaningfully higher rate than assumed, undermining volume/ROI | Medium | Medium | Track consent/opt-out rate weekly from Week 5; have non-AI documentation fallback ready | Physician Champions | Open |
| R2 | AI-drafted note contains a clinically significant error that a rushed physician signs without catching | Low | High | Mandatory physician review/edit before signing (no auto-sign); chart audits in Weeks 7 and 10 specifically screen for signed errors | Clinic Medical Directors | Open |
| R3 | Vendor retains PHI beyond the agreed transient processing window | Low | High | Written retention terms in contract; technical verification during security assessment; periodic spot-audit of vendor logs | CISO | Open |
| R4 | Physician opt-in falls short of 25/35 target, undermining statistical power of pilot | Medium | Medium | Early recruitment push in Week 3; champions personally recruit peers; consider incentive/recognition for early adopters | Clinic Medical Directors | Open |

## Assumptions
| ID | Assumption | Validation Plan | Status |
|---|---|---|---|
| A1 | Vendor's Epic integration uses certified API, no custom build needed | IT technical scoping call, Week 1 | Confirmed |
| A2 | ≥25 of 35 eligible physicians will opt in | Recruitment tracking through Week 3 | Confirmed (28 opted in) |
| A3 | State consent-to-record requirements are satisfied by verbal consent + chart documentation (no written signature required) | Legal review, Week 2 | Confirmed |

## Issues
| ID | Issue | Raised | Impact | Resolution | Owner | Status |
|---|---|---|---|---|---|---|
| I1 | Initial security assessment flagged vendor's default 30-day PHI retention (exceeded Crestview's transient-processing requirement) | Week 2 | Blocked contract finalization | Vendor agreed to contractual amendment: processing-only, no retention beyond note generation | CISO | Resolved |
| I2 | Epic sandbox test surfaced a formatting mismatch in structured note templates for 2 of 3 clinics | Week 3 | 3-day delay to integration testing | IT Analyst remapped templates per clinic | IT/Epic Integration Analyst | Resolved |

## Dependencies
| ID | Dependency | Depends On | Needed By | Status |
|---|---|---|---|---|
| D1 | Go-live | Passed security assessment + approved consent workflow | Week 5 | Met |
| D2 | Chart-quality audit | Sufficient note volume (n≥100) | Week 7 | On track |
| D3 | Scaling business case | Confirmed KPI attainment | Week 11 | Pending |
