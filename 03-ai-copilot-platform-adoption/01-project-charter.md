# Project Charter — ScribeOS: Ambient Clinical Documentation Copilot Rollout

**Organization:** Crestview Health System, a 6-hospital regional system (fictional)
**Sponsor:** Dr. Anthony Reyes, Chief Medical Information Officer (CMIO)
**Project Manager:** Marcus Ilić
**Date:** 2026-09-22 | **Duration:** 90 days (Pilot phase, 3 outpatient clinics)

## Background
Crestview physicians report averaging 2.1 hours of after-hours EHR documentation ("pajama time") per clinical day, cited as the top driver of reported burnout in the last engagement survey. Crestview wants to pilot an ambient AI scribe — listening to (with consent) patient encounters and drafting structured notes directly into Epic — to reduce documentation burden without degrading note quality or introducing new compliance exposure.

## Objectives
1. Deploy an ambient documentation AI copilot, integrated with Epic, across 3 outpatient primary care clinics (~35 physicians/APPs).
2. Reduce average after-hours documentation time by ≥40% (from 2.1 hrs to ≤1.3 hrs/day) by Day 90.
3. Maintain note quality: ≥95% of AI-drafted notes require no more than minor physician edits (measured via chart audit), with zero critical documentation errors reaching the signed note.
4. Establish patient-consent workflow and data governance model compliant with HIPAA and state consent-to-record requirements, ready for system-wide scaling decision.

## Scope
**In scope:** 3 outpatient primary care clinics, English-language encounters, integration with Epic ambulatory notes, physician opt-in participation, patient verbal consent workflow.
**Out of scope:** Inpatient/ED encounters, non-English encounters, specialty clinics (cardiology, oncology — planned as future phases), automatic note sign-off (physician review/sign remains mandatory).

## Success Criteria
- Live in all 3 pilot clinics by Day 45.
- Documentation-time and note-quality KPIs tracked weekly against a matched non-pilot clinic.
- Consent workflow audit shows 100% documented patient consent for all AI-assisted encounters.
- System-wide scaling recommendation delivered to Clinical Informatics Steering Committee by Day 90.

## Assumptions
- Epic integration can use existing vendor-certified API (no custom interface build required).
- IT Security can complete a security/privacy risk assessment within 3 weeks of contract signature.
- At least 25 of 35 eligible physicians/APPs will opt in for the pilot cohort.

## Constraints
- No PHI may be stored by the vendor beyond the transient processing window required to generate the note draft (per Crestview's data retention policy).
- Union/medical staff bylaws require physician opt-in cannot be made mandatory during pilot.
- Pilot budget capped at $180,000; go/no-go for system-wide license required by Day 90 to hold current vendor pricing.

## High-Level Budget
| Category | Estimate |
|---|---|
| Vendor pilot license (35 seats, 90 days) + Epic integration fee | $120,000 |
| Security/privacy risk assessment (external) | $30,000 |
| Change management, physician champions stipend, training | $20,000 |
| Internal labor (PM, IT, CMIO office) | ~0.5 FTE-quarter, dept. OpEx |
| **Total incremental cash spend** | **$170,000** |

## Governance
- Steering Committee: CMIO (sponsor), CMO delegate, CISO, Compliance/Privacy Officer, Clinic Medical Directors (3) — biweekly.
- Working team: PM, IT/Epic Integration Analyst, Physician Champions (3, one per clinic), Vendor Implementation Lead, Privacy/Compliance Analyst.

## Sign-off
| Role | Name | Approved |
|---|---|---|
| Executive Sponsor | Dr. Anthony Reyes | ☐ |
| CISO | Wendy Alcaraz | ☐ |
| Project Manager | Marcus Ilić | ☐ |
