---
title: USAID PIRS Compatibility - CROSS+WALKRI
version: 0.1.1
date: 2026-05-18
license: CC0
standards: CROSS v0.3.7 (github.com/cross-walkri/CROSS), WALKRI v0.1.6 (github.com/cross-walkri/WALKRI)
references:
  - USAID ADS 201 (Automated Directives System Chapter 201, Program Cycle Policy)
  - USAID Performance Indicator Reference Sheet (PIRS) Requirements
  - USAID Performance Management and Evaluation Policy (2016)
---

# USAID PIRS Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS+WALKRI-conformant program satisfies USAID Performance Indicator Reference Sheet (PIRS) documentation requirements as a structural consequence of conformance. Programs that implement CROSS for obligation architecture and WALKRI for field specification quality produce PIRS-compliant indicator documentation without additional work.

This document maps each PIRS required element to the CROSS and WALKRI provisions that produce it.

---

## What a PIRS Requires

USAID ADS 201 requires that each performance indicator in a program's Performance Management Plan (PMP) be documented in a Performance Indicator Reference Sheet. The PIRS specifies nine required documentation elements per indicator:

1. Indicator name
2. Indicator definition (including unit of measure)
3. Disaggregation
4. Rationale and relationship to project/activity
5. Data acquisition (source, collection method, collection frequency)
6. Data quality assessment procedure
7. Baseline value and data source
8. Targets
9. Notes on indicator limitations

---

## CROSS Mapping

CROSS Part V specifies eleven fields per applicant-declared indicator. These eleven fields are a strict superset of the nine PIRS elements. The mapping:

| PIRS Element | CROSS Field | Notes |
| :-- | :-- | :-- |
| Indicator name | Indicator name (Field 1) | Direct correspondence |
| Indicator definition and unit | Operational definition (Field 4) + Measurement form and evidence classification (Field 3) | CROSS separates these into two fields, providing more specification granularity than PIRS requires |
| Disaggregation | Disaggregation (Field 7) | CROSS adds a disaggregation ratchet: once a disaggregation level is reported, subsequent reports cannot drop to a less granular level |
| Rationale and relationship | Rationale for indicator (Field 2) | Direct correspondence |
| Data acquisition | Data source and collection method (Field 8) + Data cost estimation (Field 9) | CROSS requires both the methodology and a cost estimate for data collection, which PIRS does not require but which is compatible with USAID's efficiency assessment interests |
| Data quality assessment | Five data quality standards (WALKRI Part V): Validity, Integrity, Precision, Reliability, Timeliness | WALKRI's five standards are applied at the field specification stage, before data collection begins. PIRS requires a data quality assessment procedure; WALKRI requires the quality to be built into the instrument design rather than assessed retrospectively |
| Baseline | Baseline / FROM state (Field 10) | CROSS requires the FROM state to include a named data source and a specific population, which exceeds standard PIRS baseline documentation requirements |
| Targets | Target / TO state (Field 11) | Direct correspondence. CROSS additionally requires an indicator specification (data source, collection methodology) for the TO state, which PIRS does not explicitly require |
| Limitations | Construction and aggregation methodology (Field 5) | CROSS's methodology field captures the same information as PIRS's limitations note, but requires it to be stated as a construction rule rather than a caveat |

**Result:** A program operating under CROSS produces PIRS-compliant indicator documentation for every applicant-declared indicator. No additional documentation work is required to satisfy PIRS. The CROSS specification fields produce the PIRS fields as a subset of their output.

---

## WALKRI Mapping

USAID's data quality standards for performance indicators, codified in ADS 201 and the Performance Management and Evaluation Policy (2016), specify five data quality criteria: validity, reliability, precision, integrity, and timeliness. These map directly to WALKRI's five data quality standards.

| USAID Data Quality Standard | WALKRI Standard | Notes |
| :-- | :-- | :-- |
| Validity | Validity (WALKRI 5.1) | Identical criterion: the data actually measure what they are intended to measure |
| Reliability | Reliability (WALKRI 5.4) | Identical criterion: the data collection process is consistent across periods and collectors |
| Precision | Precision (WALKRI 5.3) | Identical criterion: the measurement instrument can detect differences of the magnitude relevant to the decision |
| Integrity | Integrity (WALKRI 5.2) | Identical criterion: evidence collection is separated from the entity that benefits from favorable outcomes |
| Timeliness | Timeliness (WALKRI 5.5) | Identical criterion: data are available in time to inform decisions |

**Result:** A WALKRI-conformant field specification automatically satisfies USAID data quality standards for performance indicators. The five WALKRI data quality standards are not derived from USAID's framework; they are the same underlying measurement quality principles, named consistently. This makes the correspondence exact rather than approximate.

---

## Performance Management Plan (PMP) Alignment

USAID ADS 201 requires programs to maintain a Performance Management Plan documenting: the program's Results Framework, its indicator reference sheets, its data collection and reporting schedule, and its data quality assessment plan.

CROSS's program-level Theory of Change declaration (Part IX-B) maps to the USAID Results Framework:

| USAID Results Framework Level | CROSS ToC Hierarchy Level |
| :-- | :-- |
| Development Objective (DO) | Goal |
| Intermediate Result (IR) | Long-term Outcome or Intermediate Outcome |
| Sub-Intermediate Result (Sub-IR) | Short-term Outcome |
| Output | Output |

CROSS's gate architecture maps to PMP documentation requirements:

| PMP Element | CROSS Provision |
| :-- | :-- |
| Indicator reference sheets | CROSS 11-field indicator specification (Part V) |
| Data collection schedule | Gate configuration with evidence scope and strength (Part IV) |
| Data quality assessment plan | WALKRI field specification with five data quality standards (WALKRI Part V) |
| Results Framework | Program-level ToC declaration with pathway registry (CROSS Part IX-B) |

**Result:** A program operating under CROSS with a declared program-level ToC declaration produces PMP-compatible documentation as a structural consequence of conformance. The Results Framework, indicator reference sheets, data collection approach, and data quality assessment are all specified by CROSS+WALKRI provisions.

---

## Performance Evaluation vs. Impact Evaluation

USAID distinguishes between performance evaluation (are we meeting targets?) and impact evaluation (did the intervention cause the change?). This distinction maps directly to CROSS's causality stance primitive.

A CROSS gate configured at **contribution stance** corresponds to USAID performance evaluation methodology: evidence that the program's activities contributed to observed outcomes, with co-factors acknowledged.

A CROSS gate configured at **attribution stance** (requiring counterfactual reference evidence) corresponds to USAID impact evaluation methodology: evidence that the intervention caused the observed change above the level expected without the intervention.

Most USAID programs use performance evaluation as their default and reserve impact evaluation for selected high-value interventions. The CROSS gate configuration for causality stance makes this distinction explicit at the round level rather than leaving it implicit.

---

## Collaboration, Learning, and Adapting (CLA)

USAID's CLA framework (embedded in ADS 201 since 2016) requires programs to treat their Theory of Change as a learning tool rather than a static accountability document, enabling mid-course corrections as evidence accumulates. This maps to CROSS's developmental gate character for progress verification gates and to the continuation gate's sustainability and cost-effectiveness assessments.

A CROSS-conformant program's progress verification gates are developmental in character: they surface what needs to change before the next gate, generating the mid-course learning and adaptation that CLA requires. The continuation gate's three-position sustainability stance (sustained, conditional, dependent) produces the kind of adaptive evidence USAID's CLA framework is designed to generate and act on.

---

## Adoption Guidance

Programs reporting to USAID that adopt CROSS+WALKRI should:

1. Declare OECD DAC alignment as a measurement framework in the Grant Configurator. This pre-populates external standard references with DAC criteria and connects CROSS's gate architecture to the DAC evaluation criteria USAID uses for program assessment.

2. Configure the program-level ToC declaration following the USAID Results Framework hierarchy: map the program's Development Objective to the CROSS Goal level, Intermediate Results to the Intermediate Outcome register, and Sub-Intermediate Results to the Short-term Outcome register.

3. Declare causality stance at each gate: contribution stance for standard program performance reporting, attribution stance for designated impact evaluations.

4. Use WALKRI's calibration record requirement (Part V Section 5.4) to document reviewer calibration for each compliance-threshold field. This produces the inter-rater reliability documentation USAID Data Quality Assessments examine.

Programs reporting to USAID do not need to produce separate PIRS documentation for indicators that have been specified through CROSS's 11-field indicator specification. The CROSS specification is PIRS-compatible and satisfies PIRS requirements directly.

---

## Further Information

CROSS: github.com/cross-walkri/CROSS

WALKRI: github.com/cross-walkri/WALKRI

USAID ADS 201: usaid.gov/ads/policy/200/201

USAID PIRS requirements: usaid.gov/performance-monitoring-and-evaluation

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.1 | 2026-05-17 | Standards references updated to CROSS v0.3.2 and WALKRI v0.1.1. |
| 0.1.3 | 2026-05-18 | Standards references updated to CROSS v0.3.7 and WALKRI v0.1.6. |
| 0.1.2 | 2026-05-18 | Standards references updated to CROSS v0.3.4 and WALKRI v0.1.2. |
| 0.1.0 | 2026-05-16 | Initial draft. Nine-element PIRS mapping to CROSS eleven-field specification. Five USAID data quality standards mapped to WALKRI five standards. PMP alignment with Results Framework, gate architecture, and data quality plan. Causality stance mapped to performance vs. impact evaluation distinction. CLA framework mapped to developmental gate character. Adoption guidance for USAID-reporting programs. |
