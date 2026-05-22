---
title: PCORI Methodology Standards Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.5 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - PCORI Methodology Standards, March 2024 (pcori.org/sites/default/files/PCORI-Methodology-Standards.pdf)
  - Affordable Care Act, Section 6301 (Patient-Centered Outcomes Research Institute)
  - PCORI Engagement Rubric (pcori.org/sites/default/files/Engagement-Rubric.pdf)
  - ClinicalTrials.gov (clinicaltrials.gov) and PCORI Study Registration Requirements
---

# PCORI Methodology Standards

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Patient-Centered Outcomes Research Institute (PCORI), established under Section 6301 of the Affordable Care Act, funds comparative clinical effectiveness research under a board-adopted Methodology Standards framework (most recently updated March 2024) that is mandatory for all funded studies. The PCORI Methodology Standards are structurally distinct from NIH grant requirements and from the general 2 CFR 200 uniform guidance in three ways: they impose mandatory compliance organized by domain at the award level, they require patient and stakeholder engagement in research design as a structural standard (not a preference), and they make public study protocol registration a binding requirement. CROSS+WALKRI satisfies the PCORI Methodology Standards structurally: PCORI's mandatory public study protocol registration is the direct regulatory form of CROSS's entry specification gate and attestation corpus operating simultaneously, and WALKRI's pre-publication requirements applied before any patient-reported outcome instrument is deployed produce the instrument-level specification that PCORI's data integrity standards require.

---

## The PCORI Methodology Standards Framework

The PCORI Methodology Standards establish a domain-organized compliance architecture applied at the point of award. The March 2024 version organizes standards by domain, each domain containing numbered standards that funded researchers must satisfy as conditions of their award.

**Patient-centeredness domain:** The patient-centeredness domain contains the most structurally distinctive standards in the PCORI framework. Four standards require that patients, caregivers, and other stakeholders be engaged throughout research design and conduct: in developing the research question, in selecting outcomes, in designing the study protocol, and in interpreting and disseminating results. This engagement is a structural standard, not a procedural recommendation. PCORI assesses compliance with engagement standards in progress reports and final deliverables. The requirement that the population served participate in shaping the measurement plan corresponds to CROSS's population scope declaration: who the research serves must be declared at the entry gate, and that population's participation in indicator selection is a structural feature of a CROSS-conformant program operating in the PCORI context.

**Study protocol registration:** PCORI standards require that funded studies register a publicly accessible study protocol before any data collection begins. Registration through a recognized registry (ClinicalTrials.gov or equivalent) must include the research question, study design, primary and secondary outcomes with their definitions, data sources, planned analyses, and expected timeline. This is a binding methodology standard, not a suggestion. Non-registration constitutes non-compliance. The public study protocol is simultaneously the entry specification gate (measurement plan committed to before any data is collected) and the attestation corpus (the registered protocol is independently accessible and permanently timestamped).

**Data integrity and missing data standards:** The data integrity domain includes standards for handling missing data, specifying that the analytic approach to missing data must be pre-specified in the study protocol and that sensitivity analyses must be conducted when missing data is substantial. This pre-specification requirement removes the post-hoc latitude that makes missing data handling a common source of publication bias in comparative effectiveness research.

**Analysis of clustered and longitudinal data:** Studies involving clustered data (patients within practice sites, practice sites within health systems) must specify the clustering structure and the planned statistical approach in the protocol. The level of clustering must correspond to the level at which the intervention is applied. This standard corresponds to CROSS's population scope declaration and disaggregation ratchet: the unit at which data is collected and analyzed must be specified before enrollment, and more granular specifications introduced during the study cannot replace less granular ones that were declared at protocol registration.

**Formulating research questions:** The research question domain requires that the PICO structure (Population, Intervention, Comparator, Outcome) be specified in the study protocol with sufficient precision to guide data collection and analysis. Each element of the PICO must be operationally defined: population eligibility criteria, intervention components, comparator type, and primary outcome with its measurement instrument and scoring convention.

---

## How CROSS Satisfies the PCORI Methodology Standards

CROSS addresses the PCORI Methodology Standards at the structural level.

**Entry specification gate and public protocol registration:** PCORI's mandatory public study protocol registration, required before any data collection begins, is the direct regulatory form of CROSS's entry specification gate applied to research programs. The registered protocol must contain what CROSS's entry gate requires: pre-specified outcomes with definitions (Fields 1 and 2), units of measurement (Field 3), baseline values (Field 4), targets (Field 5), timing of measurement (Field 6), data sources (Field 7), collection methods (Field 8), comparison groups (Field 9), causality stance (Field 10), and evidence thresholds (Field 11). A CROSS-conformant study protocol satisfies the PCORI protocol registration content requirements as a structural consequence of conformance with the eleven-field indicator specification.

**Attestation corpus and public protocol registry:** The publicly registered protocol creates the independently accessible attestation corpus that CROSS's attestation gate is designed to produce. The registry timestamp establishes that the measurement plan preceded any data collection, which is the core anti-manipulation function of CROSS's entry gate. When the study reports results, reviewers can compare the reported outcomes against the pre-registered protocol with confidence that the comparison reflects an independently verifiable baseline.

**Patient-centeredness and population scope declaration:** PCORI's patient-centeredness standards require that the population served participate in shaping the research design, outcome selection, and measurement approach. This corresponds to CROSS's population scope declaration applied in a research context: the population whose outcomes are measured participates in defining what outcomes are measured and how. CROSS's entry gate requirement that the population scope be declared before any application is accepted creates the structural condition under which patient and stakeholder engagement in outcome selection can occur; engagement cannot be retrofitted into a measurement plan that was finalized before the affected population was consulted.

**Causality stance and PCORI comparator requirement:** The PICO structure's comparator element corresponds to CROSS's causality stance field (Field 10) and comparison group field (Field 9). PCORI requires that the comparator be specified in the protocol with precision: active comparator, usual care, or placebo, each with its own operational definition. CROSS's causality stance field requires the same declaration, extended to include whether the program claims attribution or contribution and what counterfactual baseline informs the claim. A CROSS-conformant PCORI study applies both frameworks to the same field: the PICO comparator satisfies CROSS's Field 9 requirement, and the causality stance declaration (attribution or contribution) satisfies CROSS's Field 10 requirement in a way the PICO structure alone does not require.

**Disaggregation ratchet and subgroup analysis pre-specification:** PCORI standards require that subgroup analyses, including by age, sex, race, and clinical subgroup, be pre-specified in the study protocol if they are to be interpreted as confirmatory rather than exploratory. This pre-specification requirement corresponds to CROSS's disaggregation ratchet: once a demographic disaggregation is declared at the entry gate, it cannot be removed in later reporting. PCORI's distinction between pre-specified confirmatory subgroup analyses and post-hoc exploratory ones is the statistical form of CROSS's ratchet: the more granular specification established in the protocol cannot be replaced with a less granular one at the reporting stage.

| PCORI Methodology Standard | CROSS Provision |
|:--|:--|
| Mandatory public study protocol registration (pre-data collection) | Entry specification gate (all indicators pre-specified before data collection opens) |
| PICO population specification | Population scope declaration (who is served and what eligibility criteria apply) |
| PICO intervention and comparator specification | Causality stance field (Field 10) + comparison group field (Field 9) |
| PICO primary and secondary outcome specification | Eleven-field indicator specification (Fields 1-5: name, definition, unit, baseline, target) |
| Outcome measurement instrument and scoring convention | Fields 7-8 (data source and collection method) + Field 11 (evidence threshold) |
| Pre-specified missing data analytic approach | Field 11 (evidence threshold specifies what level of missing data renders a finding invalid) |
| Pre-specified confirmatory subgroup analyses | Disaggregation ratchet (demographic categories established at entry gate and maintained) |
| Clustering structure pre-specification | Population scope declaration + Field 9 (comparison group level corresponds to clustering level) |
| Patient-centeredness engagement throughout design | Population scope declaration with structural participation requirement in PCORI context |
| Public attestation of results against registered protocol | Attestation gate (structured evidence review against pre-specified protocol, publicly accessible) |

---

## How WALKRI Complements This Alignment

PCORI's Methodology Standards specify that outcomes must be operationally defined in the study protocol but do not prescribe, at the instrument field level, how patient-reported outcome (PRO) instruments must be specified before deployment. A PCORI-funded study measuring a PRO such as pain interference, functional status, or quality of life must select a validated instrument and report it in the protocol, but the protocol registration requirement does not extend to specifying, for each intake field, what the criterion intent is, what the operational definition of a qualifying response is, and what the compliance threshold is for individual field completion. This is the level at which WALKRI operates.

WALKRI's five pre-publication requirements applied to PRO instrument fields before any patient sees the instrument resolve the most common source of data quality problems in PRO-based comparative effectiveness research: ambiguous item wording, undefined response anchors, and unspecified threshold for what constitutes a valid (as opposed to missing) response. WALKRI's operational definition requirement forces each field in the instrument to specify what the item is designed to measure and what a qualifying response means in the context of this study's population. The evidence form requirement specifies what response format is used, what the anchor labels mean, and how responses map to the scoring convention declared in the protocol. The compliance threshold requirement specifies what response rate and what response pattern constitute the threshold below which a participant's data is treated as missing rather than incomplete.

For multi-site PCORI studies, the WALKRI pre-publication audit across all participating sites' intake instruments ensures that the PRO instrument is implemented consistently across the clustering structure declared in the study protocol. A WALKRI audit confirms that each site's intake fields match the protocol's instrument specification, so that the clustering analysis pre-specified in the protocol reflects actual data collection practices rather than site-level implementation variation. This audit function is particularly valuable for PCORI's clustered data methodology standards, where the statistical approach to clustering assumes equivalent measurement across the clusters.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
