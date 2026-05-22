---
title: SAMHSA National Outcome Measures and GPRA Measurement Tools Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.4 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - SAMHSA National Outcome Measures (NOMs) documentation (samhsa.gov)
  - GPRA Measurement Tools: CMHS, CSAP, CSAT tracks (samhsa.gov)
  - SPARS Performance Accountability and Reporting System (spars.samhsa.gov)
  - SAMHSA Programmatic Progress Report guidance (samhsa.gov)
---

# SAMHSA National Outcome Measures and GPRA Measurement Tools

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Substance Abuse and Mental Health Services Administration distributes $6-7 billion annually in discretionary grants for behavioral health programs across the United States. All SAMHSA discretionary grantees are required to collect and report client-level outcome data under the National Outcome Measures (NOMs) and the Government Performance and Results Act (GPRA) Measurement Tools, administered across three programmatic tracks: CMHS (mental health), CSAP (prevention), and CSAT (substance use treatment). CROSS+WALKRI satisfies the NOMs and GPRA evaluation requirements structurally. The mandatory client-level interview instruments, multi-domain outcome tracking, and SPARS reporting infrastructure map directly to CROSS's indicator architecture, disaggregation ratchet, and completion gate. WALKRI's five pre-publication requirements address the field specification problem that NOMs instruments currently leave to grantee interpretation.

---

## The SAMHSA NOMs and GPRA Measurement Framework

SAMHSA's NOMs represent one of the most comprehensive mandatory client-level outcome measurement systems in United States federal grantmaking. Unlike many federal grant programs that require aggregate progress reporting, SAMHSA requires grantees to administer structured interview instruments to individual clients at three points: baseline (at program entry), reassessment (mid-program), and discharge. The three GPRA tracks each have a distinct instrument tailored to their programmatic domain, but all share a common structure of client-level data collection across multiple life domains.

The mandatory data domains are: behavioral health diagnosis and symptom severity, employment status, housing stability, social functioning, criminal justice involvement, and program-specific outcomes (such as substance use frequency for CSAT grantees or mental health symptom scores for CMHS grantees). These domains constitute the NOMs indicator set. All data collected under these instruments flows into SPARS, the SAMHSA Performance Accountability and Reporting System, which is the authoritative federal repository for grantee outcome data and the basis for Programmatic Progress Reports submitted to SAMHSA.

The framework creates a mandatory pre-specified indicator set: SAMHSA establishes the NOMs domains and GPRA instrument fields before any grant competition opens. Grantees do not select their outcome indicators; they are specified by the program as a condition of funding. This structure is the behavioral health analog to the CPR's mandatory common indicator sets: a pre-specified, cross-grantee comparable measurement system established by the funder before any application is submitted.

---

## How CROSS Satisfies the NOMs and GPRA Framework

CROSS satisfies the NOMs and GPRA requirements at the structural level, addressing both the indicator specification architecture and the accountability gate structure.

**Disaggregation ratchet and baseline interview:** The mandatory GPRA baseline interview establishes each client's demographic status (age, gender, race/ethnicity, veteran status, housing status, employment status) at program entry. CROSS's disaggregation ratchet requirement directly maps to this structure: demographic and status disaggregation established at program entry must be maintained across all subsequent reporting periods. For SAMHSA grantees, the GPRA baseline interview is the operational form of the entry specification gate's disaggregation declaration. Once a client is enrolled and baselined, that client's demographic record anchors all subsequent outcome measurement, exactly as CROSS requires that disaggregation categories established at the entry gate cannot be removed in later rounds.

**Change obligation mode and multi-domain indicators:** NOMs' multi-domain outcome domains (housing, employment, functioning, criminal justice involvement, substance use) are the regulatory form of CROSS's Change obligation mode indicators. Each domain tracks a pre-specified condition change in the target population across a defined program period, measured against the baseline established at enrollment. CROSS's eleven-field indicator specification covers all elements the NOMs framework requires: Fields 1-5 (name, definition, unit, baseline, target) correspond to the NOMs domain structure, and Fields 6-11 (timing, data source, collection method, comparison group, causality stance, evidence threshold) correspond to the GPRA instrument design requirements that SAMHSA specifies in its Question-by-Question codebooks.

**Completion gate and SPARS reporting:** SPARS's structured data submission requirement is the regulatory form of CROSS's completion gate: outcome data are submitted against pre-specified indicators before any program completion determination is made. A CROSS-conformant SAMHSA grantee cannot close a program period without submitting the GPRA discharge interview data, which constitutes the completion gate evidence review. The Programmatic Progress Report incorporating NOMs data corresponds to the attestation corpus: the structured documentary record that the program completed what it stated it would complete.

| NOMs and GPRA Element | CROSS Provision |
|:--|:--|
| Mandatory NOMs domain set established before applications open | Entry specification gate (all indicators pre-specified) |
| GPRA baseline interview at program entry | Entry specification gate + disaggregation ratchet (demographic status established and locked) |
| Reassessment and discharge interviews | Completion gate evidence review against pre-specified indicators |
| Multi-domain outcome tracking (housing, employment, functioning, criminal justice, substance use) | Change obligation mode indicators (Fields 1-5: name, definition, unit, baseline, target) |
| GPRA instrument design (Question-by-Question codebooks) | Indicator specification Fields 6-11 (timing, data source, collection method, comparison group, causality stance, evidence threshold) |
| SPARS structured data submission | Completion gate: outcome data submitted before program completion determination |
| Programmatic Progress Report | Attestation corpus (structured documentary record of program completion) |
| Disaggregation by age, gender, race/ethnicity, veteran status | Disaggregation ratchet (categories established at entry gate, maintained across all periods) |

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication requirements address a structural gap in the NOMs framework that CROSS alone cannot resolve. The GPRA instruments specify which domains must be measured, but the operational definitions for key status categories are left to grantee interpretation or stated at a level of generality that produces non-comparable data across programs. What counts as "housed" for the housing stability domain? Does a client staying temporarily with family while awaiting a housing voucher count as stably housed, precariously housed, or homeless? The GPRA Question-by-Question codebooks provide guidance, but the guidance is not always operationally complete at the field level.

WALKRI's five requirements applied to NOMs intake instruments produce the specificity the framework currently lacks. The criterion intent field establishes what the housing stability measure is designed to assess. The operational definition field specifies exactly which housing arrangements qualify under each status category. The response form field specifies what the interviewer actually records. The evidence form field specifies what documentation is required to corroborate the client's self-report (a lease, a shelter intake form, a statement from a case manager). The compliance threshold field specifies what change in housing status constitutes a positive program outcome. These five requirements, applied before any client is enrolled, produce NOMs data that is commensurable across grantees in the way the SPARS system assumes it to be, but which the current framework does not structurally guarantee.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
