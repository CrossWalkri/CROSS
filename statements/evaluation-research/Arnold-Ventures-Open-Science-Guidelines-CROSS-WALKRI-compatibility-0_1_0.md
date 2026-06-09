---
title: Arnold Ventures Open Science Guidelines Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.4 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - Arnold Ventures Open Science Guidelines (arnoldventures.org/work/evidence-based-policy)
  - OSF Registries (osf.io/registries)
  - AsPredicted (aspredicted.org)
lens_tags:
  calibration_tier: independently_verified
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: private_foundation
  framework_scope_type: grantee_outcome_measurement
  # Arnold Ventures (Laura and John Arnold Foundation) open science guidelines for funded research
---

# Arnold Ventures Open Science Guidelines

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

Arnold Ventures publishes formal Open Science Guidelines governing all social science research it funds, requiring preregistration, pre-analysis plans, open data, open code, and publication of results regardless of direction. These requirements constitute a published, institutional form of the same pre-specification primitive that CROSS codifies. The structural alignment between the two frameworks is direct: Arnold requires that the measurement plan be committed to in advance, independently and verifiably, before the behavior that produces the data begins; CROSS requires that indicators be specified before applications open. Both implement the same architectural logic at different layers of the grant pipeline. A CROSS-conformant program funded by Arnold satisfies the preregistration and PAP requirements structurally, without separate procedural conformance work.

---

## The Arnold Ventures Open Science Guidelines

Arnold Ventures publishes Open Science Guidelines that apply to all social science research it funds, available at arnoldventures.org/work/evidence-based-policy. The Guidelines have five substantive structural requirements distinguishing them from general evaluation policies.

**Preregistration mandate.** All studies must be preregistered on a recognized registry, including AsPredicted, OSF Registries, or a domain-specific registry such as ClinicalTrials.gov. Preregistration must occur before any data collection begins. This is a gate condition: funding commitments are conditioned on completion of preregistration, not merely encouraged by it.

**Pre-Analysis Plans (PAPs).** For studies with causal identification, including randomized controlled trials and quasi-experimental designs, grantees must file a pre-analysis plan specifying primary and secondary outcomes, analysis strategy, sample size targets, and how subgroup analyses will be handled. PAPs must be filed before data collection begins. Arnold considers unregistered PAPs insufficient; the plan must appear in a recognized public registry to satisfy the requirement.

**Open data requirement.** Study datasets must be made publicly available in a format and location accessible to independent researchers, typically within one year of study completion or publication. The requirement is not conditional on positive findings.

**Open code requirement.** Analysis code must be made publicly available alongside the data. Code and data are treated as a package, not separate optional supplements.

**Publication commitment.** Results must be published regardless of the direction of findings. Null results and negative results must be published, not suppressed. This is an anti-suppression obligation that applies to all funded studies.

---

## How CROSS Satisfies the Arnold Ventures Open Science Guidelines

CROSS addresses the Arnold preregistration and PAP requirements at the architectural level. The preregistration mandate and PAP requirement share a single structural logic: the measurement plan must be committed to before the behavior that generates data begins, in a form that is publicly verifiable and independent of the researcher's post-hoc interpretation. CROSS's entry specification gate implements this same logic: all indicators must be fully specified, with all eleven fields complete, before any application window opens. The entry gate is a published, timestamped commitment to the measurement plan, visible to all prospective applicants before any data collection or grantee selection occurs.

A CROSS-conformant program can use its entry specification gate publication as the preregistration mechanism. The gate specification satisfies the structural requirements of a preregistration: it names the outcomes to be measured, defines them operationally, specifies the unit of analysis, declares the baseline, sets the target, identifies the data source and collection method, and declares the causality stance, including whether the program claims attribution or contribution and what the counterfactual baseline is. This is the substantive content of both a registry preregistration and a PAP. The CROSS Attestation Corpus record of the gate publication provides the independent, timestamped, publicly verifiable record that Arnold's guidelines require of registered preregistrations. Where a program chooses to file additionally on OSF Registries or AsPredicted for ecosystem interoperability, the CROSS gate specification provides the content.

Arnold's open data and open code requirements go beyond what CROSS requires. CROSS does not require datasets or code to be made publicly available; it requires that the indicators specified at entry be documented sufficiently to make independent verification possible in principle. A CROSS-conformant program wishing to satisfy Arnold's full Guidelines must add open data and open code commitments as explicit gate criteria in the round configuration, using CROSS's external standard reference mechanism in Part IV to bind those commitments to gate criteria with specified conformance thresholds. Arnold's publication commitment for null and negative results is also outside CROSS's core architecture; it is best captured as a coherence disclosure obligation in the program's round configuration, requiring the grantee to report results to the Attestation Corpus regardless of direction.

| Arnold Open Science Requirement | CROSS Provision |
|:--|:--|
| Preregistration before data collection | Entry specification gate: all indicators specified before applications open; Attestation Corpus publication provides timestamped independent record |
| Pre-analysis plan: primary and secondary outcomes | Eleven-field indicator specification: Fields 1-5 (name, definition, unit, baseline, target) for all primary and secondary outcome indicators |
| Pre-analysis plan: analysis strategy | Causality stance field: attribution or contribution declared, counterfactual baseline specified |
| Pre-analysis plan: subgroup analysis specification | Disaggregation ratchet: disaggregation categories established at entry gate and protected from removal in subsequent rounds |
| Open data requirement | Outside CROSS core scope; addable as explicit gate criterion using external standard reference mechanism |
| Open code requirement | Outside CROSS core scope; addable as explicit gate criterion using external standard reference mechanism |
| Publication of results regardless of direction | Outside CROSS core scope; addable as coherence disclosure obligation in round configuration |

---

## How WALKRI Complements This Alignment

Arnold's PAP requirement is, at its core, a field specification problem: the plan must specify what the primary outcome is, how it is measured, what counts as evidence, and what analysis will be performed. Poorly specified PAPs produce plans that are formally preregistered but substantively unverifiable because the outcome definitions and analysis rules are too vague to constrain post-hoc interpretation. WALKRI's five pre-publication field requirements address this problem at the source. A WALKRI-conformant intake field collecting data on a study's primary outcome specifies criterion intent (what the field is measuring and why), operational definition (what counts as one instance, with inclusion and exclusion criteria), response form (how the applicant documents the outcome), evidence form (what documentation is required), and conformance threshold (what standard the evidence must meet). These five elements are the operational content a pre-analysis plan must contain to be substantively, not merely procedurally, preregistered.

WALKRI's conformance threshold requirement is particularly relevant to Arnold's subgroup analysis specification. A PAP that states "we will analyze results by gender and income quartile" without specifying the minimum detectable effect size, the sample size required per subgroup, or the evidence standard for a subgroup finding to be reported is not a constraint on analysis; it is a placeholder. WALKRI's conformance threshold requirement, applied to each subgroup analysis commitment, forces the specification of what evidence standard a subgroup finding must meet to be included in the report, eliminating the analytic flexibility that registered but vaguely specified PAPs permit.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
