---
title: Global Fund M&E Framework Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - Global Fund Monitoring and Evaluation Framework, https://www.theglobalfund.org/en/monitoring-evaluation/
  - Global Fund Modular Framework for HIV, TB, and Malaria Programs
  - Global Fund Performance Framework, Grant Cycle Requirements
---

# Global Fund M&E Framework Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS+WALKRI-conformant grant program satisfies the Global Fund's Monitoring and Evaluation Framework documentation requirements as a structural consequence of conformance. The Global Fund's Modular Framework and Performance Framework govern grants across HIV, tuberculosis, and malaria programs in more than 100 countries. These frameworks require that monitoring and evaluation activities, performance indicators, baselines, and targets be defined before grants are disbursed.

CROSS's pre-round obligation specification architecture is structurally identical to this requirement. CROSS requires grantors to declare what grantees must demonstrate at each gate before any application is submitted. The Global Fund requires that monitoring and evaluation design be complete before disbursement begins. Both standards enforce the same sequencing principle: accountability infrastructure is specified before funding moves.

---

## What the Global Fund Framework Requires

The Global Fund's Performance Framework mandates the following at the program design stage, before grant disbursement:

1. Defined modules and interventions aligned to the Modular Framework
2. A complete set of Performance Indicators, including baselines and targets
3. Core indicators (standardized across all grants in that disease area)
4. Tailored indicators (grant-specific, selected by the country program)
5. Data sources and collection methods for each indicator
6. Reporting schedule aligned to the grant lifecycle
7. Evidence review at each Grant Management Meeting

Monitoring and evaluation activities must be embedded in the Funding Request. The structural requirement is non-negotiable: the Performance Framework must be complete before a grant enters implementation.

---

## Core and Tailored Indicator Architecture

The Global Fund uses two indicator tiers. Core indicators are standardized across all grants addressing the same disease area. Tailored indicators are program-specific and negotiated between the country program and the Global Fund.

CROSS's eight obligation dimensions allow grant programs to configure which indicators apply universally across all applicants and which are program-type-specific. Universal-scope indicators correspond to the Core indicator tier. Program-type-specific indicators correspond to the Tailored indicator tier. This is not an approximation: both frameworks use the same underlying distinction between indicators that must appear in every grant and indicators that are configurable to program context.

---

## Performance Indicator Field Mapping

| Global Fund Performance Indicator Requirement | CROSS Field | Notes |
| :-- | :-- | :-- |
| Indicator name | Field 1 (Indicator name) | Direct correspondence |
| Indicator definition and unit of measure | Field 4 (Operational definition) | CROSS requires the operational definition to include unit of measure and boundary conditions |
| Data source | Field 8 (Data source and collection method) | Direct correspondence |
| Collection method | Field 8 (Data source and collection method) | Separated into sub-fields within Field 8 |
| Baseline value | Field 10 (FROM state, baseline) | CROSS requires named data source and population for the FROM state |
| Target value | Field 11 (TO state, target) | Direct correspondence; CROSS additionally requires data source for the TO state |
| Reporting frequency | Gate configuration (progress verification gate schedule) | CROSS's gate sequence documents when evidence must be available; this produces the reporting schedule |
| Indicator category reference (Core or Tailored) | Field 10 (Institutional framework alignment) | Global Fund indicator category codes and disease-area classifications can be declared in Field 10 |
| Disaggregation requirements | Field 7 (Disaggregation) | CROSS's disaggregation ratchet ensures granularity cannot be reduced after first report |
| Limitations and notes | Field 5 (Construction and aggregation methodology) | CROSS requires this to be stated as a construction rule rather than a retrospective caveat |
| Data quality assessment | WALKRI five data quality standards | Applied at field specification stage, before data collection begins |

**Result:** Every element of the Global Fund Performance Indicator documentation requirement has a corresponding CROSS or WALKRI provision. A program that implements CROSS's eleven-field indicator specification and WALKRI's five data quality standards produces Global Fund-compliant indicator documentation without separate documentation work.

---

## Pre-Disbursement Design Requirement

The Global Fund's requirement that monitoring and evaluation be designed before grants begin is satisfied by CROSS's gate architecture. CROSS's four-gate sequence begins with an entry specification gate: the complete obligation set, including all indicator specifications and evidence requirements, must be declared before any applicant submits a funding request. This gate is a structural precondition for the round to open.

Programs operating under CROSS cannot reach the activation gate (the point at which funding is authorized to flow) without a complete, declared indicator set. This sequencing is identical to the Global Fund's requirement that the Performance Framework be embedded in the Funding Request before disbursement is approved.

---

## WALKRI and Data Quality

The Global Fund expects grantees to follow rigorous data quality practices throughout the grant lifecycle. WALKRI's five pre-publication field requirements (criterion intent, operational definition, response form, evidence form, compliance threshold) ensure that each data collection instrument is measurement-ready before it is deployed. WALKRI's five data quality standards match the five criteria the Global Fund applies when assessing indicator data quality: validity, reliability, precision, integrity, and timeliness.

A WALKRI-conformant field specification is a measurement instrument, not a data collection template. This distinction matters for Global Fund grant management: when data quality is built into the instrument at design time, retrospective Data Quality Assessments confirm design quality rather than remediate collection failures.

---

## Adoption Guidance

Programs applying for Global Fund grants that adopt CROSS+WALKRI should:

1. Declare Global Fund disease-area indicator category codes in Field 10 (institutional framework alignment) for each indicator. This makes the Core or Tailored designation explicit and produces the framework reference the Performance Framework requires.

2. Configure the entry specification gate to match the Funding Request submission deadline. All indicator specifications must be complete at this gate; this ensures the monitoring and evaluation design is finished before disbursement authorization.

3. Separate Core indicators from Tailored indicators using CROSS's obligation dimension configuration. Assign universal scope to Core indicators and program-type-specific scope to Tailored indicators.

4. Apply WALKRI's five data quality standards to every field collecting Performance Indicator data. This produces the data quality documentation the Global Fund Grant Management Meeting review process examines.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

Global Fund Monitoring and Evaluation Framework: https://www.theglobalfund.org/en/monitoring-evaluation/

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. Global Fund Performance Indicator requirements mapped against CROSS eleven-field specification and WALKRI five data quality standards. Core and Tailored indicator tier structure mapped to CROSS obligation dimensions. Pre-disbursement design requirement mapped to CROSS gate architecture. |
