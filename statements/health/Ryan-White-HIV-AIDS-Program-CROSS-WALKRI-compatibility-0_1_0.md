---
title: Ryan White HIV/AIDS Program Services Report and HAB Performance Measures Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.5 (github.com/cross-walkri/CROSS), WALKRI v0.1.7 (github.com/cross-walkri/WALKRI)
references:
  - Ryan White HIV/AIDS Program (ryanwhite.hrsa.gov)
  - Ryan White Services Report (RSR) Data and Technical Assistance (hab.hrsa.gov/data/data-reports)
  - HAB Performance Measures (hab.hrsa.gov/clinical-quality-management/performance-measures)
  - Electronic Handbook (EHB) (grants.hrsa.gov/grantee)
  - HHS HIV Clinical Guidelines (hivinfo.nih.gov/understanding-hiv/fact-sheets/hhs-guidelines)
---

# Ryan White HIV/AIDS Program Services Report and HAB Performance Measures

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Ryan White HIV/AIDS Program, administered by HRSA's HIV/AIDS Bureau (HAB), distributes approximately $2.5 billion annually to Parts A, B, C, and D grantees and their subrecipients serving people living with HIV. Its reporting architecture is structurally distinct from the HRSA Uniform Data System (UDS) that governs Health Center Program grantees: Ryan White uses the Ryan White Services Report (RSR), submitted through the Electronic Handbook (EHB) with a client-level encrypted unique client identifier (eUCI), a separate indicator set organized around HIV-specific clinical outcomes, and a different bureau entirely. CROSS+WALKRI satisfies the RSR and HAB Performance Measures framework structurally: the HAB performance measures constitute pre-specified Change obligation indicators established by HAB before any program year begins, the RSR's client-level eUCI linking corresponds to CROSS's disaggregation ratchet at its most granular resolution, and WALKRI's pre-publication requirements applied to Ryan White intake instruments eliminate the specification ambiguity that produces the most common data quality problems in HAB Performance Measure reporting.

---

## The Ryan White Services Report and HAB Performance Measures Framework

The Ryan White HIV/AIDS Program reporting framework has five structural features that distinguish it from general HRSA grantee reporting requirements and from the UDS framework that governs the Health Center Program.

**Client-level data with eUCI:** The RSR requires all grantees and their subrecipients to submit client-level data using an encrypted unique client identifier. The eUCI allows HRSA to link a single client's data across multiple Ryan White subrecipients, across program years, and across Parts (A, B, C, D) without collecting identifiable personal information. This client-level longitudinal linking is structurally distinct from aggregate reporting systems: it means that a client's viral load, antiretroviral therapy status, CD4 count, and service utilization are tracked individually over time, not aggregated into program-level counts before submission. The eUCI linking function corresponds to CROSS's disaggregation ratchet operating at its most granular level: individual client trajectories are maintained across reporting periods and cannot be aggregated in ways that obscure individual-level outcomes.

**HIV-specific clinical performance measures:** HAB publishes a Performance Measures set organized around HIV-specific clinical outcomes. The core measures include viral suppression rate (percentage of clients with the most recent viral load below the detectability threshold), engagement in care (percentage of newly diagnosed clients who initiate HIV medical care within 90 days of diagnosis), retention in care (percentage of clients receiving at least two HIV medical visits in a 12-month period with a gap of no more than 90 days), and antiretroviral therapy prescription rate. These measures are established by HAB and aligned to HHS HIV Clinical Guidelines before any program year begins. They are not grantee-designed; they are the national pre-specified indicator set against which all Ryan White programs are evaluated.

**Mandatory annual RSR submission through EHB:** All Parts A, B, C, and D grantees and their subrecipients submit the RSR annually, with a deadline of the last Monday in March each year. Submission is through HRSA's Electronic Handbook, not through the UDS system used by Health Center Program grantees. The EHB submission system enforces field definitions, allowable value ranges, and eUCI encryption at the point of data entry. This enforced standardization at the data submission level functions as a system-implemented form of WALKRI's compliance threshold requirement: data that does not conform to the EHB field specifications cannot be submitted.

**Population restricted to HIV-positive clients:** Unlike the UDS, which covers all patients served by a Health Center Program grantee regardless of condition, the RSR covers only clients who are HIV-positive and receiving Ryan White-funded services. This population restriction means that the RSR's disaggregation data (race, ethnicity, age, gender, HIV transmission category, insurance status) reflects the HIV-positive client population specifically. CROSS's population scope declaration for a Ryan White program must explicitly define this population boundary; a Ryan White program that declares a population scope without specifying the HIV-positive restriction produces a declaration that does not correspond to what the RSR captures.

**Separate HAB Clinical Quality Management requirements:** In addition to the RSR, Ryan White grantees must maintain a Clinical Quality Management (CQM) program as a statutory requirement. The CQM program must assess the quality of HIV-related health care provided, identify ways to improve outcomes, and implement quality improvement activities. The CQM requirement creates a mandatory internal improvement cycle that corresponds to CROSS's completion gate structure: grantees must periodically review evidence of clinical outcomes against the HAB Performance Measures and implement changes when performance falls below acceptable thresholds.

---

## How CROSS Satisfies the RSR and HAB Performance Measures Framework

CROSS addresses the RSR and HAB Performance Measures requirements at the structural level.

**Entry specification gate and HAB Performance Measures:** The HAB Performance Measures, established nationally before any program year begins, constitute the pre-specified Change obligation indicator set that CROSS's entry specification gate requires. Programs do not design their own HIV clinical indicators; they implement the nationally defined measures. CROSS's eleven-field indicator specification applied to each HAB Performance Measure produces the complete entry gate record: viral suppression rate (Fields 1-2: name and definition), percentage (Field 3: unit), prior year program rate (Field 4: baseline), the HAB-specified national benchmark or locally declared target (Field 5), calendar year (Field 6: timing), RSR submission data (Field 7: data source), EHB submission (Field 8: collection method), comparable Ryan White programs in HAB national data (Field 9: comparison group), contribution to viral suppression population targets (Field 10: causality stance), and the HAB-specified detectability threshold for viral load (Field 11: evidence threshold).

**Disaggregation ratchet and eUCI client-level linking:** The RSR's eUCI linking, which maintains individual client trajectories across program years and across subrecipients, corresponds to CROSS's disaggregation ratchet at its most granular resolution. CROSS's ratchet requires that demographic disaggregation established at program enrollment cannot be removed in later reporting periods. The eUCI system enforces this at a more granular level than program-level demographic categories: individual client HIV clinical status is tracked longitudinally and cannot be aggregated away. A CROSS-conformant Ryan White program declares its population disaggregation categories at the entry gate (race, ethnicity, age, gender, HIV transmission category, insurance status) in correspondence with the RSR's mandatory demographic fields, and the eUCI system enforces that these categories are maintained at the individual client level across years.

**CQM improvement cycle and CROSS completion gate:** The statutory CQM requirement, which mandates periodic review of clinical outcomes against the HAB Performance Measures and implementation of quality improvement activities, corresponds to CROSS's completion gate sequence. The CQM program is a structured evidence review against pre-specified indicators (the HAB Performance Measures) conducted at defined intervals within the program year. CROSS's completion gate structure, requiring evidence review at defined intervals rather than only at program end, is satisfied by the CQM cycle as a structural consequence of the CQM statutory requirement.

**Attestation gate and RSR annual submission:** The mandatory annual RSR submission, aggregated by HAB into national program performance data and published through HRSA's data reporting systems, constitutes the attestation gate and attestation corpus simultaneously. The submission is independently accessible, it is produced by a reporting system outside the individual program's control (the EHB), and it documents what the program produced against the nationally pre-specified HAB Performance Measures. A CROSS-conformant Ryan White program uses the RSR submission as the primary attestation document, supplemented by the CQM program's quality improvement records.

| RSR and HAB Performance Measures Requirement | CROSS Provision |
|:--|:--|
| HAB Performance Measures established nationally before program year | Entry specification gate (indicators pre-specified before any client enrolled) |
| Viral suppression rate as primary measure | Change obligation indicator (Fields 1-11 applied to HAB-defined measure) |
| eUCI client-level longitudinal data | Disaggregation ratchet at individual client resolution |
| RSR demographic fields (race, ethnicity, age, gender, transmission category) | Population scope declaration + disaggregation ratchet (categories maintained across years) |
| HIV-positive client population restriction | Population scope declaration (population boundary explicitly declared at entry gate) |
| Annual RSR submission through EHB | Attestation gate (structured evidence submission to independent reporting system) |
| HAB national data publication | Attestation corpus (independently accessible program performance data) |
| CQM periodic clinical outcome review | Completion gate checkpoints (evidence reviewed against pre-specified indicators at intervals) |
| CQM quality improvement implementation | Change obligation follow-through (improvement actions documented when performance falls below threshold) |
| EHB field validation at submission | Compliance threshold enforcement (non-conforming data cannot be submitted) |
| Detectability threshold for viral load | Field 11 (evidence threshold: specific viral copies/mL below which suppression is confirmed) |

---

## How WALKRI Complements This Alignment

The HAB Performance Measures define what must be measured at the clinical indicator level but do not specify, at the intake field level, how Ryan White grantees and subrecipients must design the forms and instruments that collect the underlying data. A program measuring viral suppression rate must collect viral load results from laboratory reports and link them to client identifiers in its own data system before uploading through the EHB. The specification of what qualifies as a valid laboratory report, what the measurement interval is (how recently the lab draw must have occurred to count toward the current program year measure), and what documentation the program must retain in the client record are not specified in the HAB Performance Measures themselves. These are the decisions that WALKRI's pre-publication requirements address.

WALKRI's five pre-publication requirements applied to Ryan White intake fields and data collection instruments resolve the most common sources of inconsistency in HAB Performance Measure data across Ryan White subrecipients: different programs use different definitions of "most recent" viral load, different conventions for handling clients with viral loads measured at non-Ryan White facilities, and different thresholds for what documentation is required to confirm antiretroviral therapy prescription. WALKRI's criterion intent requirement forces each intake field to specify which HAB Performance Measure it feeds and what role it plays in that measure's calculation. The operational definition requirement specifies exactly what qualifies as a valid data entry for that field in the context of this program's client population and data system. The evidence form requirement specifies what source document (lab report, pharmacy record, encounter note) is required, what elements of that document must be present, and how it is recorded in the client's file. The compliance threshold requirement specifies the minimum documentation standard below which a client's data is treated as incomplete for RSR submission purposes.

For subrecipient networks, where a Parts A or B grantee passes Ryan White funding to multiple subrecipients, the WALKRI pre-publication audit conducted across all subrecipients' intake instruments ensures that each subrecipient is collecting the underlying data in a way that corresponds to the same HAB Performance Measure definitions. Without this standardization, a network's aggregate RSR data reflects not only clinical variation but also measurement variation across subrecipients. WALKRI's pre-publication requirement applied before any subrecipient opens enrollment eliminates measurement variation as a source of performance data inconsistency, leaving clinical variation as the only remaining explanation for differences across the network.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
