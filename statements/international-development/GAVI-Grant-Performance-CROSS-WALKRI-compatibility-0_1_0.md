---
title: GAVI Alliance Grant Performance Framework Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - GAVI Alliance Grant Performance Framework (2015, revised 2018), https://www.gavi.org/our-support/grant-performance-frameworks
  - GAVI Results Framework and Indicator Guidance
  - GAVI Country Grant Portfolio Review Documentation
---

# GAVI Alliance Grant Performance Framework Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS+WALKRI-conformant program satisfies GAVI Alliance Grant Performance Framework documentation requirements as a structural consequence of conformance. The GAVI Grant Performance Framework (2015, revised 2018) requires countries to define both crosscutting and grant-specific indicators before implementation begins, with baselines and targets set before programming starts and progress measured at designated review points.

CROSS's eight obligation dimensions produce the structural architecture that the GAVI two-tier indicator system requires. CROSS's eleven-field indicator specification covers GAVI's baseline, target, and data source requirements. WALKRI's five data quality standards ensure that intake fields collecting GAVI indicator data are measurement instruments that can withstand the quality scrutiny the Grant Performance Framework applies at country review points.

---

## What the GAVI Framework Requires

The GAVI Grant Performance Framework applies to all country-level health system strengthening and immunization program grants. Its core requirements at program design stage:

1. Crosscutting metrics: a set of indicators applied uniformly across all GAVI-supported countries
2. Grant-specific indicators: a second tier selected according to grant type and country context
3. Baselines established before implementation, with documented data sources
4. Targets set before implementation, with documented rationale
5. Progress measured at annual country portfolio reviews and mid-term reviews
6. Data sources specified and confirmed as available before indicators are adopted
7. Reporting aligned to the GAVI country grant portfolio review cycle

GAVI-supported countries represent a major share of global health and immunization funding. The framework is designed to balance standardization (through crosscutting metrics) with country-level flexibility (through grant-specific indicators).

---

## Two-Tier Indicator Structure and CROSS Obligation Dimensions

The GAVI framework's most distinctive structural feature is its two-tier indicator architecture. Crosscutting metrics apply to every grantee and cannot be modified by individual countries. Grant-specific indicators are selected by the country program from a menu of eligible indicators, or defined specifically for the grant context.

CROSS's eight obligation dimensions provide the configuration mechanism that produces this same structural distinction. Obligation dimensions allow the grant program to specify which indicators apply to all applicants universally and which apply only to specific applicant categories or program types. Assigning crosscutting metrics to universal-scope dimensions and grant-specific indicators to program-type-specific dimensions produces the GAVI two-tier architecture as a configuration output, not as a separate documentation layer.

This is a structural correspondence, not an approximation. Both frameworks solve the same design problem: some accountability requirements are universal across a grant portfolio, and others are configurable to program context. CROSS's dimension architecture is the mechanism that encodes this distinction at the obligation level.

---

## Indicator Documentation Field Mapping

| GAVI Framework Requirement | CROSS Field | Notes |
| :-- | :-- | :-- |
| Indicator name | Field 1 (Indicator name) | Direct correspondence |
| Indicator definition | Field 4 (Operational definition) | CROSS requires boundary conditions and unit of measure within the operational definition |
| Baseline value | Field 10 (FROM state, baseline) | CROSS requires named data source and population for the FROM state, which exceeds GAVI's minimum baseline documentation |
| Baseline data source | Field 8 (Data source and collection method) | CROSS requires the data source to be specified at the indicator level before the grant opens |
| Target value | Field 11 (TO state, target) | Direct correspondence |
| Target rationale | Field 2 (Rationale for indicator) | CROSS's rationale field covers both the indicator rationale and the basis for target-setting |
| Data collection method | Field 8 (Data source and collection method) | Direct correspondence |
| Review point alignment | Gate configuration (progress verification gate schedule) | CROSS's progress verification gates produce the review point schedule |
| Indicator tier (crosscutting or grant-specific) | Obligation dimension configuration | Encoded in the dimension assignment, not in a separate field |
| Data quality | WALKRI five data quality standards | Applied at field specification stage |

**Result:** Every element of GAVI indicator documentation has a corresponding CROSS or WALKRI provision. The tier classification is handled by the obligation dimension configuration rather than by an additional documentation field, which makes the compliance outcome a structural consequence of how the program is configured.

---

## Pre-Implementation Indicator Definition

The GAVI framework requires that indicators, baselines, and targets all be defined before implementation begins. This requirement corresponds to CROSS's entry specification gate: the complete set of indicator specifications, including all eleven fields per indicator, must be declared and locked before any applicant submits a grant request.

CROSS's gate architecture enforces this sequencing mechanically. The activation gate, at which funding authorization occurs, cannot be reached without a complete entry specification. A program cannot be in active implementation under CROSS without having satisfied the same pre-implementation documentation requirements that GAVI mandates.

---

## WALKRI and Data Quality at Country Review Points

GAVI's country portfolio reviews assess not only whether targets were met but whether the data used to measure progress were of sufficient quality. WALKRI's five pre-publication field requirements (criterion intent, operational definition, response form, evidence form, compliance threshold) ensure that every intake field is a calibrated measurement instrument before it is deployed in a grant round.

WALKRI's five data quality standards match the five criteria GAVI reviewers apply when examining indicator data: validity, reliability, precision, integrity, and timeliness. A WALKRI-conformant field specification is audit-ready by design, which means country portfolio review data quality assessments confirm design quality rather than investigate collection failures after the fact.

---

## Adoption Guidance

Programs implementing GAVI grants that adopt CROSS+WALKRI should:

1. Assign crosscutting metrics to universal-scope obligation dimensions. Assign grant-specific indicators to program-type-specific obligation dimensions. This configuration produces the GAVI two-tier architecture within the standard CROSS obligation framework.

2. Declare GAVI indicator reference codes in Field 10 (institutional framework alignment) for each crosscutting metric. This makes the indicator's GAVI framework provenance explicit and auditable.

3. Configure progress verification gates to align with GAVI annual country portfolio review and mid-term review cycles. The gate schedule produces the review point alignment GAVI requires.

4. Apply WALKRI's five data quality standards to all intake fields before the grant round opens. This produces country review-ready data quality documentation from the start of the program rather than requiring retrospective quality assessment.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

GAVI Alliance Grant Performance Framework: https://www.gavi.org/our-support/grant-performance-frameworks

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. GAVI two-tier indicator structure mapped to CROSS obligation dimensions. GAVI indicator documentation requirements mapped to CROSS eleven-field specification. Pre-implementation definition requirement mapped to CROSS entry specification gate. WALKRI data quality standards mapped to GAVI country review requirements. |
