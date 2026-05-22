---
title: HRSA Title V Maternal and Child Health National Performance Measures Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.4 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - HRSA Title V MCH Services Block Grant Guidance (mchb.hrsa.gov)
  - Title V Information System (TVIS) (mchb.tvisdata.hrsa.gov)
  - National Performance Measures (NPMs) 2024 update (mchb.hrsa.gov)
  - HRSA Maternal and Child Health Bureau (MCHB) documentation (mchb.hrsa.gov)
---

# HRSA Title V Maternal and Child Health National Performance Measures

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Title V Maternal and Child Health (MCH) Services Block Grant, administered by HRSA's Maternal and Child Health Bureau, distributes funds to all 59 states and jurisdictions for maternal and child health programs. States must select and report on a minimum of five National Performance Measures (NPMs) drawn from a published menu spanning five population health domains, with two Universal NPMs required of all states: Postpartum Visit and Medical Home. For each selected NPM, states must develop at least one Evidence-based or Evidence-informed Strategy Measure (ESM) specifying how Title V strategies produce the NPM outcome. CROSS+WALKRI satisfies the Title V NPM and ESM framework structurally. The NPM pre-selection requirement, the ESM Theory of Change requirement, and the TVIS reporting infrastructure map directly to CROSS's entry specification gate, Theory of Change architecture, and Change obligation mode indicators. WALKRI's five pre-publication requirements address the ESM specification problem that the current framework leaves underspecified.

---

## The Title V NPM and ESM Framework

The Title V MCH Services Block Grant is structurally distinct from most federal grant programs in that it is a block grant: states have substantial discretion over how they deploy funds within the maternal and child health domain. The NPM framework is the mechanism by which HRSA introduces accountability into this discretionary structure. Rather than mandating specific programmatic interventions, HRSA mandates accountability for outcomes drawn from a pre-specified menu of population health measures, requiring states to choose their priorities before the grant period begins.

The NPM framework has been periodically updated, with the 2024 revision adjusting the measure set to reflect current MCH evidence and priorities. The five population health domains from which states select include: Women/Maternal Health, Perinatal/Infant Health, Child Health, Adolescent Health, and Children with Special Health Care Needs. The two Universal NPMs (Postpartum Visit and Medical Home) reflect HRSA's determination that these outcomes are sufficiently central to MCH that all states must be accountable for them regardless of their other priority selections.

The ESM requirement is the framework's most structurally demanding element. For each selected NPM, the state must specify at least one strategy it is implementing and articulate how that strategy produces the NPM outcome. The ESM thus functions as a micro Theory of Change: it requires the state to document the activity-to-outcome pathway before the grant period begins, and to select strategies with an evidentiary basis for believing the pathway will produce results. All NPM and ESM data is entered and tracked through TVIS, the Title V Information System.

---

## How CROSS Satisfies the Title V NPM and ESM Framework

CROSS satisfies the Title V NPM and ESM requirements at the structural level, covering the indicator pre-commitment architecture, the Theory of Change requirement, and the population-level outcome measurement structure.

**Entry specification gate and NPM pre-selection:** The NPM selection requirement corresponds directly to CROSS's entry specification gate: states choose their NPMs from a published menu and commit to those indicators before any grant period activity begins. This pre-commitment is documented in the Block Grant Application submitted to HRSA and tracked in TVIS. A CROSS-conformant Title V program's entry specification gate documentation reproduces the selected NPMs as the program's indicator set, with all eleven fields completed for each NPM before any state expenditure occurs. The Universal NPMs are non-negotiable entries in the indicator set; the selected NPMs are the state's additional pre-commitments.

**Theory of Change architecture and ESM requirement:** The ESM requirement is the regulatory form of CROSS's Theory of Change hierarchy. The ESM specifies the activity or output (the Title V strategy being implemented) and its relationship to the outcome (the selected NPM). This activity-to-outcome pathway is exactly what CROSS's Theory of Change architecture requires at the entry specification gate: the program must declare not only what outcomes it is pursuing but also what activities and outputs it is delivering as the causal pathway to those outcomes. The ESM requirement makes this declaration mandatory for every selected NPM, which is a stronger requirement than most federal programs impose.

**Change obligation mode indicators at population level:** The NPMs are population-level health measures: postpartum visit rates, medical home access rates for children with special health care needs, breastfeeding rates, and similar measures. These are CROSS's Change obligation mode indicators at the population level, measuring pre-specified condition changes in the target population across the grant period. CROSS's eleven-field indicator specification covers all elements the NPM framework requires: Fields 1-5 (name, definition, unit, baseline, target) correspond to the NPM structure as defined by HRSA, and Fields 6-11 correspond to the data source and collection methodology specifications in the Block Grant Guidance.

| Title V NPM and ESM Element | CROSS Provision |
|:--|:--|
| NPM selection from published menu before grant period begins | Entry specification gate (indicator selection pre-committed and publicly declared) |
| Two Universal NPMs required of all states | Mandatory indicator fields in entry specification gate |
| NPM pre-selection documented in Block Grant Application | Entry gate documentation published before any state expenditure |
| ESM requirement for each selected NPM | Theory of Change architecture (activities and outputs specified in relation to the outcome they are designed to produce) |
| ESM evidence-based or evidence-informed strategy requirement | Causality stance field (Field 10) + evidence threshold field (Field 11) |
| Population-level NPM outcome measures | Change obligation mode indicators (Fields 1-5: name, definition, unit, baseline, target) |
| TVIS tracking of NPM and ESM progress | Completion gate evidence submitted against pre-specified indicators |
| Annual progress reporting via TVIS | Attestation corpus (structured documentary record of program performance) |
| NPM disaggregation by population group | Disaggregation ratchet (demographic categories established at entry gate, maintained across periods) |

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication requirements address the ESM specification problem that is the primary accountability weakness in the current Title V framework. The NPM menu items are well-specified by HRSA: their definitions, data sources, and measurement methodologies are documented in the Block Grant Guidance. The ESMs, however, are state-generated and vary substantially in specificity. A state may commit to an ESM described as "increasing access to postpartum care in rural communities" without specifying what intervention is being implemented, what data will be collected to track implementation, or what constitutes successful implementation as distinct from partial or failed implementation.

WALKRI's five requirements applied to ESM development resolve this at the point of pre-publication specification. The criterion intent field establishes what the ESM strategy is designed to achieve and why it is expected to produce the NPM outcome. The operational definition field specifies exactly what the evidence-based or evidence-informed intervention consists of: which components, delivered to which population, in what sequence. The response form field specifies what implementation data is collected and how. The evidence form field specifies what documentation is required to confirm that the intervention was delivered (enrollment records, visit logs, program attendance data). The compliance threshold field specifies what implementation rate constitutes successful delivery of the strategy, producing an ESM that is a substantive commitment rather than a nominal declaration. Applied before any Title V funds are deployed, these requirements produce ESMs that are commensurable across states and auditable by HRSA, resolving the variability that the ESM requirement currently tolerates.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
