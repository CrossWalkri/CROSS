---
title: Research Funder Data Management Plan Standards Compatibility - WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/cross-walkri/CROSS), WALKRI v0.1.6 (github.com/cross-walkri/WALKRI)
references:
  - NIH Data Management and Sharing Policy (oir.nih.gov/sourcebook/intramural-program-oversight/intramural-data-sharing/2023-nih-data-management-sharing-policy)
  - NSF Data Management Plan Requirements (nsf.gov/funding/data-management-plan)
  - Horizon Europe Open Science Requirements (erc.europa.eu/manage-your-project/open-science)
  - Wellcome Trust Data and Materials Policy (wellcome.org/research-funding/guidance/policies-grant-conditions/data-software-materials-management-and-sharing-policy)
---

# Research Funder Data Management Plan Standards Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A WALKRI-conformant program satisfies the structural core of Data Management Plan requirements issued by NIH (2023, updated 2025), NSF (updated NSF-26-202), Horizon Europe, and the Wellcome Trust as a consequence of conformance. All four frameworks require, at or before the research activity stage, a plan that documents data types, metadata standards, data formats, access repositories, access paths, and sharing timelines. WALKRI's five criterion specification requirements, applied before any applicant sees the intake form, produce this documentation as a structural byproduct. WALKRI also satisfies FAIR data principles by construction; all four frameworks explicitly invoke FAIR compliance. Programs operating under any of these funders that implement WALKRI do not produce DMP content separately: WALKRI conformance generates it.

---

## The Four Frameworks

**NIH Data Management and Sharing Policy.** Effective January 2023 and updated 2025, the NIH DMS Policy applies to all NIH grant applications expected to generate scientific data. Applicants must submit a two-page Data Management and Sharing Plan specifying: the types of data to be generated, the metadata standards and data formats to be used, the repository where data will be deposited, the access level and access path, the timeline for sharing, and oversight responsibilities. As of 2025, data underlying publications must be publicly shared at the time of publication. The DMS Plan must be prepared at application stage, before data collection begins.

**NSF Data Management Plan Requirements.** Updated under NSF-26-202, NSF requires a two-page Data Management Plan as a mandatory component of all research proposals. The plan must address data types and sources, standards for data format and metadata, data access and sharing provisions, policies for re-use and redistribution, and plans for archiving and preservation. As of January 2025, data supporting publications must be publicly available. Individual directorates may impose requirements beyond the base plan, but the core DMP structure is shared across all NSF programs.

**Horizon Europe Open Science Requirements.** Under Horizon Europe, a Data Management Plan must be submitted within six months of the grant signature and must be updated at the project midpoint and at conclusion. The DMP must address: what data will be collected and how, what metadata standards will be applied, what repositories will be used (with EOSC-compliant repositories encouraged), what access level will apply, and how FAIR compliance will be achieved. Open access to research data is the default position; exceptions require documented justification.

**Wellcome Trust Data and Materials Policy.** Updated January 2025, Wellcome's policy applies to approximately £1 billion per year in biomedical research funding. An Outputs Management Plan, which functions as a DMP, is required at application stage, not only post-award. The plan must document how research data and materials will be managed and shared, must commit to FAIR compliance, and must specify access and reuse conditions. Wellcome's application-stage timing requirement aligns most closely with WALKRI's pre-publication field specification process.

---

## Unified Mapping: WALKRI Requirements and DMP Core Elements

All four frameworks converge on the same set of structural DMP elements. The table below maps WALKRI's five criterion specification requirements to these shared elements.

| DMP core element (shared by all four frameworks) | WALKRI requirement that produces it |
|:--|:--|
| Data type documentation: what data will be generated or collected | Criterion intent: specifies what each field measures and why it is included |
| Metadata standard and counting rule: how data will be described and categorized | Operational definition: specifies the unit of analysis, qualifying and non-qualifying examples, and the rule governing how responses are counted |
| Data format justification: why the chosen data form matches the data type | Response form justification: specifies why the field type (free text, structured enumeration, file upload, etc.) matches the criterion |
| Repository and access path: where data will be deposited and how it can be retrieved | Evidence form: specifies the artifact type that counts as evidence and the access path through which it can be retrieved |
| External standard reference: applicable data classification, vocabulary, or identifier scheme | Compliance threshold: specifies what external standard applies to the field, which becomes the data classification, vocabulary, or identifier reference in the DMP |

WALKRI's five requirements collectively produce a field-level DMP: one row in the table above is satisfied for every intake field in a conformant form, applied before data collection begins.

---

## FAIR Compliance

All four frameworks require FAIR compliance. WALKRI satisfies FAIR by construction.

Findable: every WALKRI-conformant field specification produces a conformance record with a stable URI. At Enhanced certification level, the conformance record is published at that URI. Every submitted response envelope carries the conformance record URI in the walkri:provenance.conformance-record-ref field.

Accessible: field specifications are published as JSON Schema with open, machine-readable format. No authentication is required to read WALKRI field specifications.

Interoperable: JSON Schema with x-walkri- extensions is parseable by any JSON Schema tool. WALKRI-conformant data from different programs is structurally comparable because the same five field specification requirements were applied to each.

Reusable: the provenance envelope provides the field-specification version, form version, collection timestamp, and certification level required for a downstream consumer to assess reusability and determine which version of each field definition governed the data.

---

## Framework-Specific Considerations

**NIH.** The NIH DMS Policy specifies that the DMP must address oversight responsibilities, including who is accountable for data management. WALKRI's certification levels (Provisional, Standard, Enhanced) provide a structured accountability record: the certification level documents the degree of audited conformance and the certifying party. NIH also requires specifying whether data preservation will be in a repository that assigns a persistent identifier; this maps to WALKRI's evidence form requirement to specify a stable access path.

**NSF.** NSF directorate-specific requirements may impose vocabulary standards, identifier schemes, or repository mandates beyond the base DMP. WALKRI's compliance threshold field is the correct place to record these directorate-level obligations: the field specifies what external standard applies, and a directorate's repository mandate or metadata vocabulary qualifies as such a standard. Programs in directorates with additional requirements should populate the compliance threshold accordingly.

**Horizon Europe.** The six-month post-signature DMP submission timeline and the midpoint update requirement mean that WALKRI audit should be completed before form publication (its normal stage) and that form revisions should be re-audited before the midpoint DMP update is submitted. WALKRI's versioned field specifications support this: each version of the form is a separate auditable artifact.

**Wellcome Trust.** Wellcome's application-stage requirement is the strongest timing alignment with WALKRI: both require data management documentation to be prepared before research activities begin, not retrospectively. A Wellcome applicant using WALKRI can draw the Outputs Management Plan content directly from the five field specification requirements completed during WALKRI Stage 1 and Stage 2 audit.

---

## Scope

This statement covers WALKRI's contribution to the data management planning elements of the four frameworks: data type documentation, metadata standards, data format, repository and access path specification, and external standard reference. Each framework also carries requirements outside WALKRI's scope, including publication venue requirements, embargo policies, license conditions for publications, and institutional sign-off procedures. These remain the responsibility of the program operator. WALKRI governs the data collection specification layer; downstream publication and reporting obligations require separate attention.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
