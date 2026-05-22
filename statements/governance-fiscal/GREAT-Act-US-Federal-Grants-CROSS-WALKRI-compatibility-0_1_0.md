---
title: GREAT Act - US Federal Grants Data Standards Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - GREAT Act (Grant Reporting Efficiency and Agreements Transparency Act, 2019)
  - OMB M-24-11 (April 2024), Grants Standard Data Elements Implementation
  - Grants Standard Data Elements v2.1 (August 2025), grants.gov/data-standards
  - 2 CFR Part 200 (2024 revision), Uniform Guidance for Federal Awards
---

# GREAT Act - US Federal Grants Data Standards Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

CROSS+WALKRI operates at a different layer than the GREAT Act data standards, but the two frameworks are complementary rather than overlapping. The GREAT Act governs transactional metadata: the administrative and financial identifiers that must be reported per award. CROSS governs obligation architecture and evidentiary standards: the programmatic commitments, indicator specifications, and data quality requirements that determine whether a funded program has done what it said it would do.

Several of the fifteen GREAT Act uniform data elements map directly to CROSS fields. Others are transactional metadata with no CROSS equivalent, which is expected and appropriate. WALKRI addresses the data quality dimension that GREAT Act's plain-language reporting requirements gesture toward but do not specify at the instrument level.

Programs receiving US federal grants that adopt CROSS+WALKRI produce GREAT Act-compatible programmatic documentation as a structural consequence of conformance. They do not satisfy the transactional reporting requirements of the GREAT Act, which are the responsibility of the awarding agency's grants management system rather than the recipient's program design.

---

## What the GREAT Act Requires

The Grant Reporting Efficiency and Agreements Transparency Act (2019) directed the Office of Management and Budget to establish standard data elements for all US federal grant awards. OMB M-24-11 (April 2024) published the implementation framework. Grants Standard Data Elements v2.1 (August 2025) specifies fifteen uniform data elements applicable to all federal awards:

1. Funder agency
2. Program title
3. Award identifier
4. Recipient legal name
5. Recipient address
6. Primary place of performance
7. Award amount
8. Period of performance start date
9. Period of performance end date
10. Project/program description
11. CFDA/Assistance Listings number
12. Recipient UEI (Unique Entity Identifier)
13. Award type
14. Action type
15. Federal action obligation / total federal investment

The 2024 revision of 2 CFR Part 200 (Uniform Guidance) strengthened data-driven reporting requirements for recipients, requiring that performance reporting connect to these standard data elements. US federal grants disburse approximately $800 billion per year across all agencies and programs.

---

## Layer Distinction: Transactional vs. Programmatic

The fifteen GREAT Act data elements fall into two categories relative to CROSS scope.

Transactional metadata (outside CROSS scope) are identifiers and financial figures generated and tracked by the awarding agency's grants management system. They describe the award transaction, not the program it funds. Elements in this category: award identifier, recipient UEI, CFDA/Assistance Listings number, award type, action type, funder agency code, award amount, federal action obligation, total federal investment, recipient address.

Programmatic metadata (inside CROSS scope) describe what the funded program is, what it intends to accomplish, where it will operate, and over what timeframe. Elements in this category: program title, project/program description, primary place of performance, period of performance start date, period of performance end date, recipient legal name.

This distinction is not a gap in CROSS coverage; it reflects CROSS's deliberate scope. CROSS specifies what a program commits to measure and how it commits to demonstrate results. The administrative machinery of the award is managed upstream by the awarding agency.

---

## Element Mapping

| GREAT Act Data Element | CROSS/WALKRI Field | Notes |
| :-- | :-- | :-- |
| Program title | Organizational identity (on-chain identity anchor) | CROSS requires a canonical program name as part of the on-chain identity anchor. Direct correspondence. |
| Project/program description | Theory of Change declaration, Goal level | CROSS's program-level ToC declaration specifies the goal, intended outcomes, outputs, and activities. This exceeds the descriptive requirement of a plain-language program description. |
| Primary place of performance | Population field (Indicator Field 6) | CROSS's population field for each indicator specifies the geographic and demographic scope of measurement. This produces place-of-performance documentation at the indicator level rather than the award level, which is more granular. |
| Period of performance start date | Gate configuration (activation gate) | CROSS's activation gate documents when program obligations take effect. This corresponds to the period start date. |
| Period of performance end date | Gate configuration (continuation gate) | CROSS's continuation gate documents when the obligation cycle closes and whether it sustains. This corresponds to the period end date. |
| Recipient legal name | Organizational identity (on-chain identity anchor) | CROSS requires the recipient organization to anchor its identity on-chain. The legal name is a required component of that anchor. |
| Funder agency | Institutional alignment (Indicator Field 10) | CROSS Field 10 (institutional framework alignment) includes the funding relationship and the external standards to which the program is aligned. The funder agency is captured in this field when the program declares USAID, FCDO, or another bilateral agency alignment. |
| Award identifier | No CROSS equivalent | Transactional metadata generated by the awarding agency. Outside CROSS scope. |
| Recipient UEI | No CROSS equivalent | SAM.gov registration identifier. Transactional metadata. Outside CROSS scope. |
| CFDA/Assistance Listings number | No CROSS equivalent | Catalog of Federal Domestic Assistance identifier. Transactional metadata. Outside CROSS scope. |
| Award amount | No CROSS equivalent | Financial transaction data. Outside CROSS scope. |
| Award type | No CROSS equivalent | Grant, cooperative agreement, contract classification. Transactional metadata. Outside CROSS scope. |
| Action type | No CROSS equivalent | New award, continuation, amendment. Transactional metadata. Outside CROSS scope. |
| Federal action obligation | No CROSS equivalent | Financial transaction data. Outside CROSS scope. |
| Total federal investment | No CROSS equivalent | Financial transaction data. Outside CROSS scope. |

**Result:** Six of the fifteen GREAT Act data elements have direct or functional CROSS equivalents. The remaining nine are transactional metadata that CROSS intentionally does not govern. A GREAT Act-reporting program using CROSS produces the programmatic elements of GREAT Act compliance through its standard obligation architecture. The transactional elements are satisfied by the awarding agency's grants management system.

---

## WALKRI and the Plain-Language Reporting Requirement

The 2024 revision of 2 CFR Part 200 includes a plain-language performance reporting requirement: recipients must report results in terms that non-specialist readers can interpret. This requirement gestures toward data quality and communicability but does not specify how indicators should be constructed to make results interpretable.

WALKRI's five pre-publication field requirements address this gap at the instrument design level. The criterion intent field requires that the evaluative purpose of each indicator be stated explicitly. The operational definition field requires that the indicator's measurement logic be unambiguous. The response form field requires that the evidence collection method be specified in advance. The evidence form field requires that the acceptable evidence types be identified. The compliance threshold field requires that the pass/fail boundary be stated before evidence is collected.

A WALKRI-conformant indicator specification produces a result that is interpretable by non-specialist readers because the operational definition and compliance threshold are explicit. The plain-language reporting requirement of 2 CFR Part 200 is satisfied as a structural consequence of WALKRI conformance, not as a post-hoc writing exercise.

---

## Adoption Guidance

Programs receiving US federal grants that adopt CROSS+WALKRI should:

1. Declare the funder agency in Indicator Field 10 (institutional framework alignment) for all indicators relevant to the award. If the program reports to multiple federal agencies, each agency relationship should be declared separately at the indicator level.

2. Use the program-level ToC declaration to produce the project/program description required by the GREAT Act. The Goal level of the CROSS ToC corresponds to the award-level description; Outcome and Output levels produce the more granular programmatic narrative that 2 CFR Part 200 performance reporting requires.

3. Configure activation and continuation gates with explicit dates. These dates produce the period-of-performance documentation required by the GREAT Act.

4. Apply WALKRI's five pre-publication field requirements to all performance indicators that will appear in federal progress reports. This ensures that reported results satisfy the plain-language interpretability standard in 2 CFR Part 200.

Programs receiving federal awards do not need to produce separate programmatic narrative documentation beyond what CROSS+WALKRI conformance produces. The transactional data elements are the responsibility of the awarding agency's grants management infrastructure and do not require action from the recipient's program team.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

GREAT Act implementation: grants.gov/data-standards

OMB M-24-11: whitehouse.gov/omb/management/grants-management/

2 CFR Part 200 (Uniform Guidance): ecfr.gov/current/title-2/subtitle-A/chapter-II/part-200

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. Fifteen GREAT Act data elements mapped against CROSS fields. Transactional vs. programmatic layer distinction articulated. WALKRI mapping to plain-language reporting requirement of 2 CFR Part 200. Adoption guidance for US federal grant recipients. |
