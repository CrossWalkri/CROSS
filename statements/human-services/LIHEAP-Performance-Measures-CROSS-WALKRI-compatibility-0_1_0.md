---
title: LIHEAP Performance Measures Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.5 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - Low Income Home Energy Assistance Act, 42 U.S.C. § 8621 et seq.
  - 42 U.S.C. § 8629(b) (LIHEAP performance measurement authority)
  - Federal Register, June 2013 (LIHEAP performance measures formal establishment)
  - liheappm.acf.hhs.gov (LIHEAP Performance Management system)
  - Administration for Children and Families, HHS (acf.hhs.gov)
---

# LIHEAP Performance Measures

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Low Income Home Energy Assistance Program (LIHEAP), authorized under 42 U.S.C. § 8621 et seq. and administered by the Administration for Children and Families (ACF) within HHS, requires all state grantees to report annually on three statutory outcome measures established under 42 U.S.C. § 8629(b) and formally published in a June 2013 Federal Register notice: average reduction in energy burden for households receiving fuel assistance, percent of households where LIHEAP prevented a potential energy crisis, and percent of households where LIHEAP restored home energy after a crisis or disconnection. These three measures are the most compact pre-specified indicator set in the federal human services grant landscape: three indicators, established by statute and Federal Register notice, mandatory for all 50 states and DC before any program year begins. CROSS's four-gate sequence is structurally compatible with this framework, and WALKRI's pre-publication requirements address LIHEAP's primary data quality challenge: the statutory terms "energy crisis" and "energy burden" lack field-level operational definitions, producing non-comparable data across states in the national LIHEAP dataset.

---

## The LIHEAP Performance Measures Framework

LIHEAP provides federal block grant funding to all 50 states, the District of Columbia, U.S. territories, and federally recognized tribes to assist low-income households with home energy costs. The program is authorized under 42 U.S.C. § 8621 et seq. and administered by ACF within HHS. The LIHEAP Statute at 42 U.S.C. § 8629(b) establishes the performance measurement authority and requires states to submit data on LIHEAP outcomes annually as part of their reporting obligations. The three performance measures were formally established in a June 2013 Federal Register notice and are collected through the LIHEAP Performance Data Form submitted by all states and DC.

Measure 1 captures the average reduction in energy burden for households receiving fuel assistance, where energy burden is defined as the share of household income spent on home energy costs. This is a change indicator requiring both a baseline energy burden calculation and a post-assistance calculation for the same household. Measure 2 captures the percent of households where LIHEAP prevented a potential energy crisis, requiring a counterfactual determination: what would have happened to this household's energy access without LIHEAP assistance? Measure 3 captures the percent of households where LIHEAP restored home energy after a crisis or disconnection, requiring a documented status change from disrupted access to restored access. The LIHEAP Performance Management system at liheappm.acf.hhs.gov provides data collection infrastructure and technical assistance for state grantees.

The three measures' statutory origin means they cannot be modified by individual states. All states report on the same three outcomes using the same form. This creates a nominally uniform dataset that should support national comparison and benchmarking across the 50-state LIHEAP network. In practice, the absence of field-level operational definitions for the key statutory terms produces data that is formally comparable (all states report on the same three measures) but substantively heterogeneous.

---

## How CROSS Satisfies the LIHEAP Performance Measures Framework

The three LIHEAP statutory performance measures are pre-specified by statute and Federal Register notice before any program year begins, satisfying CROSS's entry specification gate requirement in the strongest possible form. No state can modify, replace, or supplement these measures as the primary performance indicators for LIHEAP reporting purposes; they are fixed by statute. This is the entry specification gate operating at the federal statutory level.

**Change obligation mode indicators:** All three measures are Change obligation mode indicators, each requiring a documented change in a household's energy status or condition. Measure 1 requires a before-and-after measurement of energy burden, corresponding to CROSS Fields 4 and 5 (baseline and target) applied at the household level. Measure 2 requires a counterfactual determination, corresponding to CROSS's causality stance field: what would have happened without the intervention? This is one of the few instances in federal human services grant reporting where a statutory performance measure explicitly requires a counterfactual element. Measure 3 requires a documented status change from crisis to resolution, corresponding to CROSS's completion gate outcome evidence requirement: verified change in a binary household energy access condition.

**Attestation gate and federal reporting:** The LIHEAP Performance Data Form submitted annually by all states to ACF constitutes the attestation gate. State grantees must document their performance on all three measures and submit data to the national LIHEAP Performance Management system, creating a persistent, nationally queryable record of verified performance claims. CROSS's attestation gate requirement is satisfied by this formal annual submission, which is publicly accessible and used by ACF for program oversight and Congressional reporting.

| LIHEAP Performance Measure | CROSS Provision |
|:--|:--|
| Three statutory performance measures (pre-specified) | Entry specification gate at statutory level; Change obligation mode indicator set |
| Measure 1: Energy burden reduction | Fields 4-5 (baseline/target); Change obligation mode; completion gate evidence |
| Measure 2: Energy crisis prevention | Causality stance field; counterfactual determination requirement |
| Measure 3: Energy restoration after crisis/disconnection | Completion gate outcome evidence; binary status change documentation |
| LIHEAP Performance Data Form (annual) | Attestation gate; attestation corpus |
| All-state mandatory reporting | Disaggregation ratchet; population scope declaration (50-state coverage) |
| 42 U.S.C. § 8629(b) statutory authority | Entry specification gate at statutory level |

---

## How WALKRI Complements This Alignment

LIHEAP's three statutory measures are CROSS-compatible in structure but face an acute operational definition gap that WALKRI is specifically designed to resolve. "Energy crisis," "energy burden," and "energy restoration" are statutory terms that carry legal weight but lack field-level operational definitions specifying what documentary evidence, what classification rules, and what thresholds apply when a caseworker records a household's situation. The result is that states make different definitional decisions about what qualifies as a prevented energy crisis or a restored energy supply, producing national LIHEAP data that appears comparable but is not.

WALKRI's five pre-publication field requirements, applied to LIHEAP intake instruments before any state deploys the Performance Data Form collection process, resolve this at source. WALKRI's criterion intent requirement specifies what the statute intends each measure to capture: not merely that assistance was provided, but that a documented change in energy access or burden occurred as a result. WALKRI's operational definition requirement specifies the precise threshold for each term: what income percentage qualifies as energy burden, what utility notice or disconnection documentation qualifies as an energy crisis, and what documentation of reconnection or payment arrangement qualifies as restoration. WALKRI's evidence form requirement specifies what source documents satisfy each classification: utility bills, reconnection notices, benefit determination letters, or caseworker-observed status. Applied to all 50 states' LIHEAP intake instruments before any program year begins, these requirements transform the three statutory measures from nominal uniform indicators into genuinely commensurable outcome metrics producing a national dataset capable of supporting meaningful cross-state comparison and program improvement.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
