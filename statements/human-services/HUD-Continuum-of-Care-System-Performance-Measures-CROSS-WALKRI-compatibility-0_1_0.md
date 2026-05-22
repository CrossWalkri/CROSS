---
title: HUD Continuum of Care System Performance Measures Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.5 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - McKinney-Vento Homeless Assistance Act, 42 U.S.C. § 11381 et seq.
  - 24 CFR Part 578 (Continuum of Care Program)
  - HUD CoC System Performance Measures Programming Specifications (hudexchange.info)
  - hudexchange.info/programs/coc/system-performance-measures/
  - HMIS Data Standards Manual (HUD, current edition)
---

# HUD Continuum of Care System Performance Measures

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The U.S. Department of Housing and Urban Development requires Continuums of Care to calculate and report seven System Performance Measures as part of the annual CoC Program competition, with performance data directly affecting funding awards through Section 3A of e-snaps. HUD has published these measures and their programming specifications since FY 2015, using the Homeless Management Information System (HMIS) as the mandatory data infrastructure for all CoC-funded programs. CROSS's four-gate sequence is structurally compatible with the CoC System Performance Measures framework: the seven measures constitute the pre-specified indicator set established before each competition opens, HMIS is the attestation corpus through which claims are verified, and the funding decision itself constitutes the completion gate. WALKRI's pre-publication requirements apply to HMIS intake instruments to ensure that the fields recording length of time homeless, exit destination, and income at exit specify their operational definitions and evidence requirements before any client is enrolled in the system.

---

## The HUD CoC System Performance Measures Framework

The Continuum of Care Program, authorized under the McKinney-Vento Homeless Assistance Act (42 U.S.C. § 11381 et seq.) and governed by 24 CFR Part 578, funds local homeless service systems organized as Continuums of Care, each of which is a coordinated network of providers serving a defined geographic area. HUD awards CoC Program funds through an annual competition in which CoC performance on the System Performance Measures directly affects funding awards; Section 3A of the e-snaps application scores CoC performance data, making the seven measures not merely reporting requirements but determinants of funding allocation.

The seven System Performance Measures are: Measure 1, Length of Time Persons Remain Homeless; Measure 2, Returns to Homelessness After Housing Placement; Measure 3, Number of Homeless Persons; Measure 4, Employment and Income Growth for Homeless Persons in CoC-funded Programs; Measure 5, Number of Persons Who Become Homeless for the First Time; Measure 6, Successful Placement from Street Outreach; and Measure 7, Successful Housing Placement from Transitional Housing and Permanent Supportive Housing Exits. HUD publishes programming specifications and table shells for all seven measures, and all CoC-funded programs are required to collect client-level data in HMIS.

HMIS is the mandatory data infrastructure through which all CoC-funded providers collect, maintain, and report client-level data. HUD publishes HMIS Data Standards specifying the required data elements, their definitions, and their collection timing. Because performance on the seven measures is calculated from HMIS data and directly determines funding, the quality of HMIS intake instruments is a direct determinant of funding outcomes for every Continuum of Care.

---

## How CROSS Satisfies the HUD CoC System Performance Measures Framework

The seven System Performance Measures constitute CROSS's pre-specified indicator set at the Continuum level. HUD establishes and publishes these measures and their programming specifications before each annual competition opens, satisfying CROSS's entry specification gate requirement: the indicators are known, defined, and published before any CoC application is submitted or any client is enrolled in the program year.

**Completion gate and funding decision:** Because Section 3A of the annual e-snaps application scores CoC performance on the seven measures and this score directly affects funding awards, the funding decision constitutes CROSS's completion gate. Continuums that demonstrate performance improvement on the measures receive higher scores and are more competitive for continued funding; those that underperform face funding reductions or reallocation. This is a consequential completion gate with direct financial implications, operating at the Continuum level rather than the individual grantee level.

**HMIS as attestation corpus:** HMIS is the mandatory, queryable record of client-level data through which all performance claims are verified. This corresponds directly to CROSS's attestation corpus: a persistent, auditable dataset that supports both the completion gate assessment and independent verification of claims. HUD's annual analysis of HMIS data to produce the Annual Homeless Assessment Report (AHAR) constitutes a system-level attestation against the pre-specified indicators. CROSS's attestation gate requirement, that claims be supported by a documented evidence corpus maintained in a form accessible to independent verification, is satisfied by HMIS as a structural consequence of CoC program participation.

**Change and Retroactive obligation modes:** Measure 1 (length of time homeless) and Measure 2 (returns to homelessness) are longitudinal indicators requiring tracking across multiple program contacts and multiple years. CROSS's Retroactive obligation mode applies to these measures: outcome claims for clients whose homelessness history spans prior program years require that prior-period data be brought forward into the current assessment. CROSS's Change obligation mode applies to Measure 4 (employment and income growth), which requires a documented change in a client's economic status between program entry and exit.

| HUD CoC Measure | CROSS Provision |
|:--|:--|
| Seven pre-specified System Performance Measures | Entry specification gate; Change obligation mode indicator set |
| Measure 1: Length of time homeless | Field 4 (baseline: initial shelter entry date) + Field 6 (timing) + Retroactive obligation mode |
| Measure 2: Returns to homelessness | Longitudinal tracking; Retroactive obligation mode; causality stance field |
| Measure 3: Number of homeless persons | Population scope declaration; disaggregation ratchet |
| Measure 4: Employment and income growth | Change obligation mode; Field 4 (baseline) + Field 5 (target) |
| Measure 5: First-time homeless | Population scope declaration; comparison group field |
| Measure 6: Successful placement from street outreach | Completion gate outcome indicator; evidence threshold field |
| Measure 7: Successful housing placement | Completion gate outcome indicator; evidence threshold field |
| HMIS mandatory data infrastructure | Attestation corpus; attestation gate |
| Section 3A funding score | Consequential completion gate |

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication field requirements apply to HMIS intake instruments to ensure that the fields recording the seven measures' underlying data elements specify their operational definitions and evidence requirements before any client is enrolled. HMIS intake fields appear technically defined by the HUD Data Standards Manual, but the Standards Manual addresses field definitions at the data system level, not at the instrument level at which CoC-funded providers collect client information. The gap between a HMIS data element definition and a client intake field that reliably captures that element in real program settings is where the seven measures' data quality problems originate.

WALKRI's operational definition requirement, applied before any client intake form is deployed, addresses the most consequential ambiguities. "Housing situation at program entry" for Measure 1 requires a precise operational definition of which living arrangements qualify as homelessness under the four HUD homeless definitions, how split-situation households are classified, and what documentation is required. "Exit to permanent housing" for Measure 7 requires a precise operational definition of what qualifies as permanent housing in the local housing market, what documentary evidence (lease, letter of acceptance, address verification) is required, and how situations of uncertain permanence are classified. Without WALKRI-level pre-publication specification for each of these fields, individual case managers make inconsistent classification decisions that produce HMIS data that is technically compliant with the Data Standards but that generates non-comparable performance scores across providers within the same Continuum.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
