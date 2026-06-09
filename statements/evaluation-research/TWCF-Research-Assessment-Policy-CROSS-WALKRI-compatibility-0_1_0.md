---
title: Templeton World Charity Foundation Research Assessment Policy Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - Templeton World Charity Foundation Research Assessment Policy (templetonworldcharity.org/our-policies/research-assessment-policy)
  - Templeton World Charity Foundation Open Access Policy (templetonworldcharity.org/our-policies/open-access-policy)
  - Templeton World Charity Foundation Open Research strategy (templetonworldcharity.org/about-us/our-strategy/open-research)
  - San Francisco Declaration on Research Assessment (sfdora.org/read)
  - DORA Signers Register (sfdora.org/signers)
lens_tags:
  calibration_tier: outcome_specified_self_reported
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: private_foundation
  framework_scope_type: grantee_outcome_measurement
  # Templeton World Charity Foundation Research Assessment Policy
---

# Templeton World Charity Foundation Research Assessment Policy

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

Templeton World Charity Foundation (TWCF) publishes a formal Research Assessment Policy that requires grantee research institutions to implement the principles of the San Francisco Declaration on Research Assessment (DORA) and to monitor and report progress on that implementation. The policy carries a grantee-facing obligation, not merely an internal commitment by the funder: any institution applying for or receiving TWCF research funding is expected to publish a DORA implementation statement, hold an implementation plan with a delivery date, and operate a process for monitoring and reporting progress. Because the obligation is published, externally citable, and binding on grantees, the policy crosses the threshold from internal commitment to compatibility-eligible standard. CROSS+WALKRI satisfies the policy structurally: the entry specification gate carries the implementation-statement disclosure, the continuation gate carries the progress-monitoring requirement, and WALKRI's criterion specification requirements supply the operational definitions that DORA implementation needs in order to be assessable rather than merely declared.

TWCF is a separate legal entity from the John Templeton Foundation (JTF). This statement applies to TWCF only. JTF has not been found to publish a comparable grantee-facing research-assessment standard and remains in the CROSS+WALKRI coverage gap map.

---

## The TWCF Research Assessment Policy

Templeton World Charity Foundation, headquartered in Nassau, The Bahamas, is a grant-making institution that funds scientific and scholarly research in human flourishing, character virtue, religion and science, and related areas. TWCF was established in 1996 by Sir John Templeton as a separate legal entity from the John Templeton Foundation; the two organizations share founding lineage but operate independently with distinct boards, staff, strategies, and policies. Compatibility claims about TWCF policies do not extend to JTF and should not be read across the two entities.

The TWCF Research Assessment Policy was introduced as part of the Foundation's open-research strategy and was published in 2021. It is one of three published TWCF policies that govern grantee research conduct: the Open Access Policy (requiring all final research papers funded by TWCF to be made openly accessible), the Open Research strategy materials (covering data, code, and methodology sharing expectations), and the Research Assessment Policy itself. The Research Assessment Policy is publicly accessible at templetonworldcharity.org/our-policies/research-assessment-policy and is referenced from the Foundation's grantee resources.

The policy commits TWCF as an institution to assessing research on substantive scholarly criteria rather than on journal-based metrics such as Journal Impact Factor. It states that TWCF does not use journal-based metrics as a surrogate measure of the quality of individual research articles, of the contributions of individual scientists, or in funding decisions. This is the DORA principle for funders applied to TWCF's own evaluation practice.

The grantee-facing obligation is the distinguishing feature of the policy. TWCF expects grantee research institutions to have, at a minimum: (1) a published statement of commitment to implementing the DORA principles, accessible on the institution's own website and visible to its researchers and to the public; or, where a full statement is not yet in place, a clear process for developing one with a specified delivery date; (2) an implementation plan covering how DORA principles will be applied in the institution's hiring, promotion, funding, and research-evaluation decisions; and (3) a process for monitoring and reporting progress against the plan, so that implementation is verifiable rather than merely asserted.

This three-part structure is what distinguishes the TWCF policy from a generic DORA endorsement. A funder signing DORA commits the funder to the declaration's principles. The TWCF policy goes further: it conditions the grantee relationship on the grantee institution itself becoming a DORA-implementing entity, with its own published statement, plan, and reporting cadence. This is a published, citable, externally verifiable grantee obligation rather than an internal funder position.

The Declaration on Research Assessment (sfdora.org/read) is the external standard against which the TWCF policy is anchored. DORA was developed in 2012 at the American Society for Cell Biology annual meeting in San Francisco and has been signed by tens of thousands of individuals and organizations across more than 170 countries. Its core recommendations to funders, institutions, publishers, and researchers center on three principles: do not use journal-based metrics as a surrogate measure of the quality of individual research articles; assess research on its own merits rather than on the basis of the journal in which it is published; and capitalize on the opportunities provided by online publication, including relaxing unnecessary limits on numbers of words, figures, and references in articles and exploring new indicators of significance and impact. For funders, DORA additionally recommends being explicit about the criteria used in evaluating the scientific productivity of grant applicants and clearly highlighting that the scientific content of a paper is much more important than publication metrics or the identity of the journal in which it was published.

The TWCF Research Assessment Policy translates these DORA principles into a grantee obligation. A grantee institution that signs no statement, publishes no plan, and operates no monitoring process is not in conformance with the policy regardless of whether its individual researchers personally support DORA's principles.

---

## How CROSS Satisfies the Policy

CROSS satisfies the TWCF Research Assessment Policy structurally through three mechanisms: the external-standard reference at the entry gate, the disclosure architecture that surfaces institutional implementation status, and the continuation-gate progress assessment.

**External-standard reference at the entry specification gate.** CROSS Part IV allows a funder to bind a published external standard to a gate criterion through the external-standard reference mechanism. A TWCF-funded program operating under CROSS records DORA as a named external standard at the entry specification gate, with the TWCF Research Assessment Policy as the conformance threshold document and DORA itself as the substantive standard. The conformance threshold specifies what evidence satisfies the criterion at the entry gate: the URL of the applying institution's published DORA implementation statement; or, where a statement is not yet published, a written commitment naming the delivery date and the responsible signing authority within the institution. This binds the policy to the gate architecture rather than treating it as an ambient expectation. An applicant who cannot supply either form of evidence has not satisfied the entry specification for a TWCF-aligned round under CROSS.

**Organizational identity declaration as the locus for institutional commitment.** CROSS's organizational identity declaration at the entry gate (Part IV) requires the applying entity to declare its legal entity name, jurisdiction, parent organization, affiliated entities, and disbursement authority. For research-grant contexts, the declaration is the natural locus for the DORA implementation-statement disclosure, because the implementation statement is a property of the applying institution itself, not of the individual grant. The applicant submits the institutional DORA implementation statement (or the implementation plan with delivery date) as a field of the organizational identity declaration. Where the applying entity is a research institution, the disclosure is required; where the applying entity is an individual researcher applying with institutional affiliation, the disclosure attaches to the affiliated entity field.

**Indicator specification and the prohibition on impact-factor surrogates.** The substantive content of DORA, and of the TWCF policy that operationalizes it, is that journal-based metrics must not be used as surrogates for research quality. CROSS's indicator specification rules in Part V (the eleven-field structure that requires every indicator to declare its operational definition, unit of analysis, baseline, data source, and collection methodology) prohibit by construction the use of unspecified composite proxies. An indicator named "publication quality" defined only as "Journal Impact Factor of the publishing venue" fails CROSS Field 4 (operational definition) because the operational content of impact factor as a measure of an individual article's quality is precisely what DORA disputes. A CROSS-conformant indicator for research quality must be specified at the article, dataset, code, or methodology level, with a defined evidence form. This is the DORA prohibition expressed as a measurement-specification constraint rather than as a normative declaration.

**Continuation gate and progress monitoring.** The TWCF policy requires grantee institutions to monitor and report progress on DORA implementation. CROSS's continuation specification gate, configured at the program level, provides the structural place for this progress assessment. A multi-year or repeat-applicant grantee passing through the continuation gate must produce evidence of progress against the implementation plan disclosed at the entry gate of the prior round: changes in hiring or promotion criteria, revisions to internal research-assessment procedures, or published updates to the institutional DORA statement. The progress-monitoring requirement becomes a continuation-gate evidence requirement under CROSS Part IV; it is not satisfied by re-asserting the original implementation commitment without evidence of progress.

**Public benefit mechanism and access condition.** Where TWCF-funded research is claimed as a public goods contribution, CROSS Part II activates the public benefit mechanism declaration. For research-publication outputs, the mechanism type is output production and the access condition includes the publication's open-access status under the TWCF Open Access Policy. The Research Assessment Policy and the Open Access Policy interact at this point: an applicant claiming an output production public benefit mechanism must satisfy the open-access requirement (CC-BY license or equivalent, publicly accessible final version) and must operate under an institution with a DORA implementation statement. The two TWCF policies are independent gate criteria; satisfying one does not satisfy the other.

**Scholarly infrastructure compatibility.** CROSS Part XII documents compatibility with scholarly infrastructure identifiers (ROR, ORCID, Crossref DOIs, DataCite fundingReference, schema.org/Grant). For TWCF-funded research programs adopting CROSS, the institutional DORA implementation statement is most usefully published at a stable URL associated with the institution's ROR record, and individual researchers are identified by ORCID. This is not a CROSS requirement but a recommended implementation pattern that makes the DORA implementation status queryable as part of the scholarly identifier graph rather than discoverable only by manual website inspection.

| TWCF Research Assessment Policy Requirement | CROSS Provision |
|:--|:--|
| Grantee institution publishes a DORA implementation statement | Organizational identity declaration: institutional implementation-statement URL as a required disclosure for research-institution applicants |
| Or, in lieu of a published statement, a plan with delivery date | Same field accepts an implementation-plan document with a named delivery date and signing authority |
| Implementation plan covering hiring, promotion, funding, and evaluation decisions | External-standard reference mechanism (Part IV): TWCF Research Assessment Policy as conformance threshold, DORA as the substantive standard |
| Progress monitoring and reporting | Continuation specification gate: progress evidence against the entry-gate implementation commitment, configured at the program level |
| Funder does not use Journal Impact Factor as a research-quality surrogate | Indicator specification rules (Part V): operational definition requirement prohibits unspecified composite proxies; impact-factor surrogates fail Field 4 |
| Research-quality assessment based on article, data, code, methodology | Public benefit mechanism declaration (Part II): output production mechanism scopes evidence to the artifact level |
| Open-access publication (TWCF Open Access Policy interaction) | External-standard reference mechanism: TWCF Open Access Policy as a separate conformance threshold at the completion gate |
| Institutional statement publicly accessible | Access condition declaration: implementation-statement URL must resolve without authentication |

---

## How WALKRI Complements This Alignment

A DORA implementation statement is, in effect, a field specification problem at the institutional level. The reason institutions sign DORA and then implement it inconsistently is not bad faith; it is that the substantive criteria for "research quality assessed on its own merits" are themselves under-specified. An institution can publish a statement committing to DORA principles and continue to operate hiring and promotion processes in which the prestige of publishing venues acts as the actual decision criterion, because nothing in the statement specifies what should replace impact factor at the point of decision. WALKRI's five criterion specification requirements address this problem at the source.

Applied to the institutional research-evaluation criteria that DORA implementation is supposed to govern, the WALKRI requirements force operational content into what would otherwise remain a normative declaration. Criterion intent: what is the institution measuring when it assesses a researcher's contribution, and why does that measurement matter for the decision being made (appointment, promotion, internal funding allocation)? Operational definition: what counts as evidence of a substantive scholarly contribution at the article, dataset, code, or methodology level, with inclusion and exclusion examples? Response form: how does an evaluator record the assessment in a way that is comparable across candidates? Evidence form: what artifact does the candidate submit to satisfy the criterion, and where does it live? Conformance threshold: what level of evidence constitutes a satisfied criterion?

Institutions that complete this specification exercise produce implementation plans that constrain evaluator behavior at the point of decision. Institutions that do not complete it produce statements that are formally DORA-aligned but operationally unchanged. The difference is the WALKRI specification work.

WALKRI's conformance-threshold requirement is particularly load-bearing for the article-level assessment that DORA requires. An institution stating that "the scientific content of a paper is more important than the journal in which it appeared" has not yet specified how an evaluator should weigh, for example, a high-quality methodological contribution published in a low-prestige venue against a less substantive contribution published in a high-prestige venue. The conformance-threshold field, applied to each criterion the institution uses to evaluate research, forces the institution to state what level of evidence satisfies the criterion and what does not. Without this specification, DORA implementation collapses back into evaluator discretion, and evaluator discretion under institutional incentives tends to reproduce the impact-factor heuristic the policy was designed to eliminate.

For TWCF specifically, the WALKRI requirements applied at the grantee-institution level convert the Research Assessment Policy from a published commitment into an auditable institutional process. A grantee institution that has produced WALKRI-conformant specifications for its research-evaluation criteria can present those specifications as evidence at the CROSS continuation gate, satisfying the progress-monitoring requirement with operational evidence rather than narrative report.

---

## Distinction from John Templeton Foundation

This statement applies to Templeton World Charity Foundation only. The John Templeton Foundation (JTF) is a separate legal entity, headquartered in West Conshohocken, Pennsylvania, with its own board, staff, strategy, and policy framework. The two organizations share founding lineage (both were established by Sir John Templeton) but operate independently and publish independent policies. Research conducted on the CROSS+WALKRI coverage gap map identified no published JTF research-assessment standard meeting the threshold of a formally published, externally citable, grantee-facing requirement. JTF remains in the gap map as a Named US Foundation Without Published Frameworks. A compatibility statement covering JTF would require a separate research pass and a separate document; readers should not infer JTF coverage from this TWCF statement.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
