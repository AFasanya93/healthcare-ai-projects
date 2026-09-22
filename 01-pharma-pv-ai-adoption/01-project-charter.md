# Project Charter — PV-Copilot: AI-Assisted Signal Detection & Case Triage

**Organization:** Meridian Biopharma (fictional)
**Sponsor:** Dr. Elena Kowalski, VP Pharmacovigilance & Drug Safety
**Project Manager:** Dana Whitfield
**Date:** 2026-09-22 | **Duration:** 90 days (Discovery/Pilot phase)

## Background
Meridian's PV team processes ~4,200 adverse event (AE) case reports/month across 3 marketed products. Manual triage and MedDRA coding create a 3.5-day average case-processing time, and case volume is projected to grow 40% with the upcoming oncology launch. Meridian wants to pilot an AI copilot that pre-triages incoming AE cases, drafts MedDRA coding suggestions, and flags potential safety signals for human review — not to replace PV physicians, but to compress cycle time and catch signals earlier.

## Objectives
1. Stand up a validated AI triage/coding-assist tool for spontaneous AE reports within one product line (pilot scope).
2. Reduce average case triage time from 3.5 days to ≤1.5 days for pilot volume by Day 90.
3. Achieve ≥90% concordance between AI-suggested MedDRA codes and final human-coded terms, measured weekly.
4. Produce a validated, auditable process package suitable for QA/regulatory review (21 CFR Part 11 considerations).

## Scope
**In scope:** One product (Meridian-X, cardiology), spontaneous case intake channel only, English-language cases, AI-assisted triage + coding suggestion + signal-flagging dashboard, human-in-the-loop sign-off on every case.
**Out of scope (this phase):** Clinical trial SAE processing, non-English cases, auto-submission to regulatory authorities, full GxP computer system validation (planned as a follow-on project).

## Success Criteria
- Pilot live with real case flow by Day 60.
- ≥90% AI/human coding concordance sustained for 2 consecutive weeks by Day 90.
- Zero missed serious/unexpected AE signals attributable to the tool (validated via parallel manual review during pilot).
- Go/no-go recommendation for broader rollout delivered to Safety Committee by Day 90.

## Assumptions
- Vendor-provided AI model can be configured on de-identified historical case data without PHI transfer issues.
- QA and Regulatory Affairs can allocate 20% time for validation support during the pilot.
- IT can provision a sandboxed environment isolated from production case management system (Argus) within 2 weeks.

## Constraints
- No changes to the system of record (Argus Safety) during pilot — copilot operates as an advisory layer only.
- Vendor contract caps pilot to 90 days before requiring a paid renewal decision.
- PV physicians' review capacity limits pilot volume to ~500 cases/month.

## High-Level Budget
| Category | Estimate |
|---|---|
| Vendor pilot license (90 days) | $85,000 |
| Validation/QA contractor support | $40,000 |
| Internal labor (PM, PV SMEs, IT) | ~0.6 FTE-quarter, budgeted in dept. OpEx |
| **Total incremental cash spend** | **$125,000** |

## Governance
- Steering Committee: VP Pharmacovigilance (sponsor), QA Director, Head of Regulatory Affairs, CISO delegate — biweekly.
- Working team: PM, 2 PV physicians, 1 PV coder/SME, vendor solutions engineer, IT security lead, QA validation lead.

## Sign-off
| Role | Name | Approved |
|---|---|---|
| Executive Sponsor | Dr. Elena Kowalski | ☐ |
| QA Director | Marisol Tan | ☐ |
| Project Manager | Dana Whitfield | ☐ |
