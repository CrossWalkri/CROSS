---
title: World Bank Results Framework Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/cross-walkri/CROSS), WALKRI v0.1.6 (github.com/cross-walkri/WALKRI)
references:
  - Managing World Bank Trust Funds for Results (November 2025, thedocs.worldbank.org)
  - World Bank Results Framework guidance, Annex 2 (November 2025)
  - World Bank Investment Project Financing Results Framework requirements
---

# World Bank Results Framework Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS-conformant program satisfies the indicator documentation requirements of the World Bank Results Framework (RF) as a structural consequence of conformance. The World Bank RF uses terminology distinct from the generic Logframe (Development Objective, PDO-level indicators, Intermediate Results indicators), but the underlying requirements map directly to CROSS's eleven-field indicator specification. The level distinction between PDO and IR indicators maps to CROSS's outcome and output indicator levels in the Theory of Change architecture.

This compatibility statement covers programs seeking World Bank Trust Fund co-financing, Investment Project Financing grants, or co-funding arrangements with programs that must satisfy World Bank reporting requirements.

---

## What the World Bank Results Framework Is

All World Bank Trust Funds are required under Bank Policy to have a Results Framework aligned with relevant country and corporate strategies. Investment Project Financing grants require Results Frameworks as a condition of funding. The RF is the primary instrument through which the World Bank tracks whether funded programs are producing what they were funded to produce.

The World Bank RF organizes indicators at two levels.

PDO-level (Project Development Objective) indicators measure outcomes at the objective level: what the project is designed to change in the world. These correspond to the statement "as a result of this project, the following conditions will be measurably different."

IR-level (Intermediate Results) indicators measure outputs and intermediate results: the deliverables, activities, and intermediate states that contribute to the PDO. These correspond to "as a result of this project's activities, the following artifacts or conditions will exist."

Every indicator at both levels requires: an indicator name, a definition, a unit of measure, a baseline value, a target value, a data source, a collection methodology, a reporting frequency, and a responsible party. The RF additionally requires that each indicator specify whether it is a core indicator (drawing from the World Bank's Results Measurement System standard indicator list) or a custom indicator, and if custom, why a core indicator was not appropriate.

---

## How CROSS Satisfies the World Bank Results Framework

CROSS's eleven-field indicator specification satisfies all required RF indicator elements at both PDO and IR levels.

| World Bank RF element | CROSS field(s) |
|:--|:--|
| Indicator name | Field 1: Indicator name |
| Definition | Field 2: Definition |
| Unit of measure | Field 3: Unit of measure |
| Baseline value | Field 4: Baseline value |
| PDO-level target | Field 5: Target value (outcome-level indicators) |
| IR-level target | Field 5: Target value (output-level indicators) |
| Disaggregation by population | Field 6: Population scope |
| Data source | Field 7: Data source |
| Collection methodology | Field 8: Collection frequency |
| Responsible party | Field 9: Responsible party |
| Institutional framework link | Field 10: Institutional framework alignment |
| PDO indicator designation | CROSS ToC architecture outcome level |
| IR indicator designation | CROSS ToC architecture output level |

The PDO/IR level distinction, which is the structural feature most specific to the World Bank RF, is expressed in CROSS through the Theory of Change architecture's causal hierarchy. Programs declare their ToC at four levels (goal, outcome, output, activity), and indicators are declared at the level corresponding to what they measure. PDO indicators correspond to the outcome level; IR indicators correspond to the output level. A CROSS-conformant program produces this level distinction as a structural output of the ToC declaration.

---

## The Core Indicator Requirement

The World Bank RF distinguishes between core indicators (drawn from the World Bank's Results Measurement System indicator list) and custom indicators (designed by the program team). Programs must justify the use of custom indicators when standard ones exist.

CROSS's Field 10 (institutional framework alignment) accommodates this requirement. When a program's outcome indicators correspond to World Bank core indicators, Field 10 records the core indicator reference code. When custom indicators are used, the CROSS indicator specification provides the justification documentation required by the RF: the definition, unit, baseline method, and data source together constitute the justification for why a custom indicator was designed.

---

## How WALKRI Complements This Alignment

The World Bank RF specifies what indicators must document. It does not specify what makes the intake fields that collect indicator data into measurement instruments. WALKRI fills that gap.

A WALKRI-conformant field collecting baseline data for a World Bank RF indicator must specify the criterion intent, the operational definition (including qualifying counting rules and unit of analysis), the response form justification, the evidence form (the artifact type and access path proving the submitted value), and any applicable compliance threshold.

The World Bank's M&E guidance requires that baseline values be verifiable. A label version of a baseline field accepts any submitted number. A WALKRI-conformant version of the same field specifies the counting rule, the time period, the population boundary, and the evidence the reviewer must verify before the baseline is accepted. WALKRI provides the field architecture that makes the World Bank's verifiability requirement structural rather than dependent on reviewer judgment.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
