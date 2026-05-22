---
title: IsDB Independent Evaluation Guidelines Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.2 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - IsDB Independent Evaluation Guidelines for Public Sector Project Evaluation, September 2024 (isdb.org/sites/default/files/media/documents/2024-09/Independent%20Evaluation%20Guidelines%20for%20Public%20Sector%20Project%20Evaluation.pdf)
  - IsDB Guidelines for Preparing Project Performance Evaluation Reports, 2024 (isdb.org/publications/independent-evaluation-guidelines-for-project-completion-report)
  - IsDB Evaluation Typology and Nomenclature, September 2024
---

# IsDB Independent Evaluation Guidelines Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Islamic Development Bank's Independent Evaluation Department (IEvD) publishes formal evaluation guidelines specifying what project-level evidence is required at completion and performance evaluation. CROSS's gate architecture satisfies these requirements as a consequence of its compliance with OECD DAC evaluation criteria, which the IsDB RBMF explicitly adopts. A CROSS+WALKRI-conformant program produces, as a structural byproduct of conformance, the gate evidence records that IsDB's IEvD requires for project completion evaluation and performance supervision.

The IsDB Results-Based Management Framework (RBMF) operates across four tiers, and CROSS's layered obligation architecture maps to each tier without additional adaptation. WALKRI ensures that the data feeding IsDB's consolidated results indicators meets the specification quality standards that independent evaluators apply when verifying reported values.

---

## What the IsDB Evaluation Guidelines Are

The Islamic Development Bank is a multilateral development bank headquartered in Jeddah, Saudi Arabia, with 57 member states across the Muslim world and beyond. Its mandate combines conventional development finance with Islamic finance principles. The IEvD is the Bank's independent evaluation function, responsible for assessing whether IsDB-financed projects achieved their intended results.

The IEvD's September 2024 "Independent Evaluation Guidelines for Public Sector Project Evaluation" establishes the methodological framework for all IsDB project evaluations. The guidelines specify: evaluation design principles, evidence standards for each OECD DAC criterion, the typology of evaluation products (project completion reports, performance evaluation reports, thematic evaluations), and the documentation requirements that projects must satisfy for each product type.

IsDB applies six OECD DAC evaluation criteria within its own Results-Based Management Framework: relevance, coherence, effectiveness, efficiency, impact, and sustainability. These criteria are not applied independently; IsDB's RBMF organizes them across a four-tier hierarchy that connects project-level evidence to portfolio-level reporting.

**Tier 1: Goals.** Strategic objectives and development impact at the national or sectoral level. This tier corresponds to the long-term change that IsDB financing is intended to support, expressed as goals in the country or sector strategy.

**Tier 2: Consolidated Results Indicators.** Portfolio-level aggregated indicators across all active projects in a given sector or country. IEvD collects evidence from individual projects and rolls it up to Tier 2 for Annual Development Effectiveness Report publication.

**Tier 3: Operational Effectiveness.** Project-level output and outcome achievement against the logical framework established at appraisal. This is the primary locus of project completion report evidence.

**Tier 4: Organizational Efficiency.** Inputs, processes, and institutional quality: budget adherence, procurement compliance, supervision quality, and reporting completeness.

The Guidelines for Preparing Project Performance Evaluation Reports (2024) specify the evidence structure for Tier 3: what evaluators look for in a project completion report, how achievement is rated against the six criteria, and what documentation constitutes acceptable evidence for each rating. The Evaluation Typology and Nomenclature (September 2024) standardizes the vocabulary across all IEvD products.

---

## How CROSS Satisfies the IsDB Evaluation Guidelines

CROSS satisfies IsDB evaluation requirements as a consequence of its OECD DAC compliance. Because IsDB's RBMF is built on the same six OECD DAC criteria that CROSS's obligation architecture addresses, conformance with CROSS produces project-level evidence records that satisfy IsDB's completion and performance evaluation requirements without any additional documentation effort.

The four-tier RBMF architecture maps to CROSS's layered obligation architecture as follows:

| IsDB RBMF Tier | CROSS Provision |
|:--|:--|
| Goals (Tier 1) | Theory of Change goal-level declaration; the CROSS goal field specifies the long-term system-level change to which the program contributes, matching IsDB's Tier 1 strategic objective |
| Consolidated Results Indicators (Tier 2) | Completion gate evidence against Fields 1-11; the eleven-field indicator specification produces the standardized, baseline-anchored data that IEvD aggregates for portfolio-level reporting |
| Operational Effectiveness (Tier 3) | Progress verification gate records; these constitute the project completion report evidence that IEvD evaluators assess against the six OECD DAC criteria |
| Organizational Efficiency (Tier 4) | Organizational identity declaration; concurrent funding disclosure; procurement and process documentation linked through CROSS document reference fields |

**OECD DAC criterion mapping.** Each of the six criteria that IsDB evaluators apply at Tier 3 corresponds to a structural element in CROSS:

*Relevance*: CROSS's entry specification gate requires alignment between the program's declared Theory of Change and the conditions of the target population. The FROM state (existing conditions, baseline) and the TO state (intended change) provide the evidence base for an evaluator's relevance assessment.

*Coherence*: CROSS's coherence disclosure field requires the program to declare how it relates to other interventions operating in the same domain with the same population. This is exactly the evidence an IsDB evaluator needs to assess internal coherence (alignment with IsDB strategy) and external coherence (complementarity with partner country systems).

*Effectiveness*: CROSS's completion gate evidence, structured around Fields 1-11 with baseline, target, and reported actual values, provides the primary evidence for effectiveness ratings. The gate determination record documents whether the program met its pre-specified completion criteria.

*Efficiency*: The CROSS concurrent funding disclosure and organizational identity declaration provide the financial transparency needed for efficiency assessment, including cost-per-output analysis against the disbursement record.

*Impact*: CROSS's causality stance field, which requires the program to declare whether it claims attribution or contribution and to specify the counterfactual basis for that claim, is the evidence foundation for IsDB's impact assessment.

*Sustainability*: CROSS's continuation gate, when present, provides direct evidence of sustainability: what was achieved in the preceding period, what institutional arrangements sustain the achievement, and how the next phase builds on completed work.

The project completion report format that IsDB's IEvD requires is satisfied by the CROSS gate record architecture: a structured determination at each gate, with evidence references, produces a documentary trail that meets the IEvD's minimum evidence standards for each criterion rating. No separate project completion report format is needed; the CROSS gate records can be directly submitted to or referenced by the IEvD review process.

---

## How WALKRI Complements This Alignment

IsDB's IEvD evaluators, when assessing Tier 2 consolidated results indicators, must determine whether the values reported by individual projects were produced by comparable measurement methodologies. When projects define their indicators differently, use different counting rules, or apply inconsistent disaggregation specifications, the roll-up to Tier 2 becomes analytically unreliable. This is a known limitation in multi-project portfolio evaluation, and it is a primary source of the "results washing" risk that independent evaluators are trained to detect.

WALKRI addresses this limitation at the collection instrument level. By requiring each data field to specify its criterion intent, operational definition, construction methodology, and evidence form before any program operator or beneficiary submits data, WALKRI ensures that the values feeding into IsDB's consolidated results indicators are produced by pre-specified, documented methodologies. This makes the IEvD evaluator's job significantly more tractable: rather than reconstructing measurement intent from ambiguous field labels, the evaluator can read the WALKRI field specification and determine directly whether the reported value is comparable with values from other projects in the same sector.

For programs operating under IsDB co-financing or technical assistance mandates, WALKRI conformance also satisfies the data quality documentation requirement that IsDB project appraisal documents typically impose on implementing partners.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
