---
title: HRSA Health Center Program Uniform Data System Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.4 (github.com/cross-walkri/CROSS), WALKRI v0.1.7 (github.com/cross-walkri/WALKRI)
references:
  - HRSA Uniform Data System (UDS) annual reporting requirements (bphc.hrsa.gov)
  - HRSA Bureau of Primary Health Care (BPHC) UDS guidance (bphc.hrsa.gov)
  - UDS Modernization Initiative documentation (bphc.hrsa.gov)
  - Health Center Program statute, 42 U.S.C. 254b
---

# HRSA Health Center Program Uniform Data System

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Health Resources and Services Administration (HRSA) requires all Health Center Program awardees, including Federally Qualified Health Centers (FQHCs) and FQHC look-alikes, to report annually via the Uniform Data System (UDS). This requirement is statutory under 42 U.S.C. 254b and administered by HRSA's Bureau of Primary Health Care. The UDS covers three measurement categories: access (patients served, visits, enabling services), quality of care and health outcomes (16 clinical quality measures), and financial cost and viability. CROSS+WALKRI satisfies the UDS evaluation requirements structurally. The mandatory pre-specified clinical quality measure set, longitudinal annual reporting structure, and patient-level numerator and denominator logic map directly to CROSS's entry specification gate, disaggregation ratchet, and eleven-field indicator specification. WALKRI's pre-publication requirements address the field specification problem in UDS patient intake instruments.

---

## The HRSA Uniform Data System Framework

The UDS is one of the most mature mandatory annual reporting systems in United States federal health grantmaking. Unlike grant programs with discretionary indicator selection, the UDS mandates a specific set of clinical quality measures that all health centers must track and report, regardless of size, location, or patient population composition. The 16 clinical quality measures as of the current reporting period include blood pressure control, diabetes management (HbA1c poor control, HbA1c control), colorectal cancer screening, depression screening and follow-up, childhood immunization status, HIV linkage to care, and related measures. Many of these measures are aligned with HEDIS (Healthcare Effectiveness Data and Information Set) and CMS quality measure sets, producing cross-program comparability with the broader health quality measurement ecosystem.

The UDS data covers all patients served by the health center, regardless of payer source. HRSA publicly releases aggregate UDS data annually, making it one of the more transparent federal grantee performance datasets. The UDS Modernization Initiative, underway as of 2024, has been redesigning the reporting infrastructure to support patient-level data submission, shifting the UDS from aggregate reporting toward individual-level data collection more analogous to SAMHSA's GPRA instruments.

Each clinical quality measure is defined by a patient-level denominator (the eligible population for that measure) and a numerator (the subset of the eligible population achieving the clinical target). This denominator-numerator structure is the UDS implementation of pre-specified indicator logic: HRSA specifies the denominator criteria, the numerator criteria, and the measurement period before any health center begins patient care in the reporting year.

---

## How CROSS Satisfies the UDS Framework

CROSS satisfies the UDS requirements at the structural level, covering the indicator specification architecture, the longitudinal reporting structure, and the patient-level disaggregation requirements.

**Entry specification gate and pre-specified clinical quality measures:** The UDS's mandatory pre-specified clinical quality measure set corresponds directly to CROSS's entry specification gate: all indicators are established before the health center operates in any given reporting year, not selected post-hoc based on available data. A CROSS-conformant health center's entry specification gate documentation reproduces the UDS measure set as the program's indicator specification, with all eleven fields completed for each measure before any patient encounter occurs in the reporting period. HRSA, not the grantee, establishes the indicator set; CROSS's gate structure formalizes the accountability relationship that this regulatory design creates.

**Disaggregation ratchet and longitudinal annual reporting:** The UDS requires the same measures to be reported each year using the same denominator and numerator definitions. This longitudinal consistency is the regulatory form of CROSS's disaggregation ratchet: the indicator set is fixed and maintained across reporting periods, and demographic disaggregation (by age, race/ethnicity, income level, insurance status) established in the UDS reporting structure cannot be removed in later rounds. The UDS Modernization Initiative's shift toward patient-level data will make the disaggregation ratchet more precisely enforceable at the individual patient record level.

**Eleven-field indicator specification and UDS measure definitions:** The UDS's patient-level numerators and denominators for clinical quality measures correspond to CROSS's eleven-field indicator specification. Fields 1-5 are directly satisfied: the measure name (e.g., "Hypertension: Controlling High Blood Pressure"), definition (the HEDIS-aligned clinical specification), unit (percentage of eligible patients), baseline (prior year rate), and target (HRSA's Health Center Quality Leader benchmark). Fields 6-11 are satisfied by the UDS reporting instructions: the measurement period (Field 6, timing), the electronic health record and UDS submission (Field 7, data source), the patient encounter documentation requirements (Field 8, collection method), the national benchmark (Field 9, comparison group), the HEDIS attribution methodology (Field 10, causality stance), and the Health Center Quality Leader threshold (Field 11, evidence threshold).

| UDS Element | CROSS Provision |
|:--|:--|
| Mandatory clinical quality measure set established before reporting year begins | Entry specification gate (all indicators pre-specified before program activity) |
| Same measures required across all reporting years | Disaggregation ratchet (indicator set fixed and maintained across periods) |
| Patient-level denominator (eligible population) | Indicator specification Field 3 (unit) + population scope declaration |
| Patient-level numerator (clinical target achieved) | Indicator specification Field 5 (target) + completion gate evidence |
| UDS measure name and clinical definition | Indicator specification Fields 1-2 (name and definition) |
| Prior year rate as baseline | Indicator specification Field 4 (baseline) |
| Health Center Quality Leader benchmark | Indicator specification Field 11 (evidence threshold) |
| HEDIS attribution methodology | Indicator specification Field 10 (causality stance) |
| Annual UDS submission to HRSA | Completion gate (outcome data submitted against pre-specified indicators) |
| UDS patient demographic disaggregation (race/ethnicity, income, insurance) | Disaggregation ratchet (demographic categories established and maintained) |

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication requirements address the field specification problem in UDS patient intake instruments. The UDS measure definitions specify what to count at the reporting stage, but the intake fields that collect the underlying data at the point of patient registration are not specified to the same level of precision. A health center's intake form for race/ethnicity must collect data in a way that supports UDS reporting, but the UDS guidance does not specify at the field level what the intake question must look like, what response options must be offered, what the interviewer instructions must say, or what happens when a patient declines to identify.

WALKRI's five requirements applied to UDS-supporting intake fields resolve these ambiguities before any patient is registered. The criterion intent field establishes what the race/ethnicity field is measuring and why. The operational definition field specifies which OMB race/ethnicity categories are in use and how multiracial patients are classified. The response form field specifies the exact response options the registration form must offer. The evidence form field specifies whether self-report is sufficient or whether documentation is required. The compliance threshold field specifies the minimum data completeness rate required for UDS submission. These requirements, applied to all UDS-supporting intake fields before the health center registers its first patient, produce a registration instrument that generates UDS-compatible data by design rather than by post-hoc data cleaning.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
