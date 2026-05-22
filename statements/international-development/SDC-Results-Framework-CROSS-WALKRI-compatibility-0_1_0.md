---
title: SDC Results Framework Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - Swiss Agency for Development and Cooperation (SDC), International Cooperation Strategy 2025-2028
  - SDC Aggregated Reference Indicators and Thematic Reference Indicators
  - SDC Policy Markers and Rio Convention Alignment Guidance, https://www.sdc-cde.ch/en/guidance-and-indicators
---

# SDC Results Framework Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS+WALKRI-conformant program satisfies the Swiss Agency for Development and Cooperation (SDC) Results Framework documentation requirements as a structural consequence of conformance. SDC's International Cooperation Strategy 2025-2028 requires all cooperation programs to have outcome statements and impact hypotheses declared before implementation begins. SDC uses Aggregated Reference Indicators (ARI) and Thematic Reference Indicators (TRI) as its measurement architecture, with Policy Markers aligned to Rio Convention environmental targets layered on top.

CROSS's Change obligation mode, combined with the entry specification gate, produces the precise documentation sequence SDC requires: a declared FROM state (baseline), a declared TO state (target), and a stated causal hypothesis linking the program's activities to the expected change. This is not a retrofitted alignment; it is a structural identity between what SDC requires and what CROSS produces as a standard output of conformance.

---

## What SDC Requires

The SDC Results Framework, operating under the International Cooperation Strategy 2025-2028, mandates the following at program design stage:

1. An outcome statement declaring the expected change in the target population's condition
2. An impact hypothesis (the causal argument for why the program's activities will produce the expected outcome)
3. Aggregated Reference Indicators declared before implementation; these are standardized across SDC's portfolio
4. Thematic Reference Indicators for program-specific measurement; these are selected according to the program's thematic focus
5. Policy Markers declared where programs are relevant to Rio Convention environmental objectives, gender equality, or poverty reduction
6. Baselines with documented data sources before implementation begins
7. Targets set before implementation, with documented rationale
8. Progress reporting aligned to SDC's annual review cycle

SDC is a significant bilateral funder with high evidence standards and documented interest in innovation in the development sector.

---

## Change Obligation Mode and the Impact Hypothesis

CROSS's three obligation modes govern how a program's accountability architecture is framed. The Change obligation mode is the structural equivalent of SDC's outcome statement plus impact hypothesis requirement.

In Change mode, the program must declare:

- The FROM state: a specific, measurable description of the condition that the program intends to change, including a named data source and a documented population
- The TO state: a specific, measurable description of the condition the program expects to produce, with a target value and a named data source for measurement
- The causal pathway: the Theory of Change sequence connecting the program's activities to the expected change at outcome level

This three-part declaration is what SDC means by "outcome statement and impact hypothesis." SDC requires the causal argument to be stated before implementation. CROSS requires the FROM state, TO state, and causal pathway to be declared at the entry specification gate, which must be complete before any applicant submits a funding request. The sequencing is identical.

---

## ARI and TRI Architecture Mapped to CROSS

SDC's Aggregated Reference Indicators and Thematic Reference Indicators correspond to CROSS's obligation dimension configuration in the same way that GAVI's crosscutting and grant-specific indicators do. Aggregated Reference Indicators are standardized across SDC's portfolio; Thematic Reference Indicators are selected by the program team based on thematic focus.

CROSS's obligation dimensions allow programs to assign indicators to universal scope (applying to all applicants) or to program-type-specific scope (applying to specific applicant categories). Assigning Aggregated Reference Indicators to universal-scope dimensions and Thematic Reference Indicators to program-type-specific dimensions produces the SDC two-tier architecture.

| SDC Indicator Requirement | CROSS Field | Notes |
| :-- | :-- | :-- |
| Indicator name | Field 1 (Indicator name) | Direct correspondence |
| Indicator definition | Field 4 (Operational definition) | CROSS requires boundary conditions and unit of measure |
| Baseline value | Field 10 (FROM state, baseline) | CROSS requires named data source and population |
| Target value | Field 11 (TO state, target) | Direct correspondence |
| Data source | Field 8 (Data source and collection method) | Direct correspondence |
| Impact hypothesis | Causality stance field + Theory of Change declaration | CROSS's causality stance encodes the methodological basis for the causal claim; the Theory of Change pathway encodes the argument itself |
| ARI or TRI reference code | Field 10 (Institutional framework alignment) | SDC indicator codes declared in Field 10 produce the framework reference SDC requires |
| Policy Marker declaration | Field 10 (Institutional framework alignment) | Rio Convention and other SDC Policy Markers can be declared in Field 10 alongside indicator codes |
| Data quality | WALKRI five data quality standards | Applied at field specification stage |

**Result:** Every element of SDC Results Framework documentation has a corresponding CROSS or WALKRI provision. The ARI and TRI tier classification is handled by the obligation dimension configuration. Policy Markers are handled by Field 10 declarations.

---

## Policy Markers and Field 10

SDC Policy Markers identify the degree to which a program addresses Rio Convention environmental objectives, gender equality, or poverty reduction. These markers are applied at program design stage and reported throughout the grant lifecycle.

CROSS Field 10 (institutional framework alignment) is designed to accommodate external framework codes and sector classifications. SDC Policy Marker codes can be declared in Field 10 alongside ARI and TRI references. This makes the Policy Marker alignment explicit in the program's obligation architecture rather than tracked separately in program documentation.

---

## WALKRI and SDC Evidence Standards

SDC's high evidence standards require that data collection instruments be capable of producing reliable, valid data under field conditions in often-challenging operating environments. WALKRI's five pre-publication field requirements (criterion intent, operational definition, response form, evidence form, compliance threshold) ensure that each intake field is a calibrated measurement instrument before it is deployed. WALKRI's five data quality standards (validity, reliability, precision, integrity, timeliness) correspond to the criteria SDC applies when assessing data quality at annual review.

---

## Adoption Guidance

Programs funded by SDC that adopt CROSS+WALKRI should:

1. Configure the program in Change obligation mode. Declare the FROM state, TO state, and causal pathway at the entry specification gate before implementation begins.

2. Declare SDC Aggregated Reference Indicator codes in Field 10 for universal-scope indicators. Declare Thematic Reference Indicator codes in Field 10 for program-type-specific indicators. Declare applicable Policy Marker codes in Field 10 alongside the indicator references.

3. Configure the causality stance field at each progress verification gate to reflect the methodological basis for progress claims: contribution stance for standard outcome monitoring, attribution stance where SDC requires counterfactual evidence.

4. Apply WALKRI's five data quality standards to all intake fields before the grant round opens. This produces SDC-ready data quality documentation from program design rather than as a retrospective exercise.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

SDC Guidance and Indicators: https://www.sdc-cde.ch/en/guidance-and-indicators

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. SDC outcome statement and impact hypothesis requirement mapped to CROSS Change obligation mode and entry specification gate. ARI and TRI two-tier indicator architecture mapped to CROSS obligation dimensions. Policy Markers mapped to Field 10 declarations. WALKRI data quality standards mapped to SDC evidence requirements. |
