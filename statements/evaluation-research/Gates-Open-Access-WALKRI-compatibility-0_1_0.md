---
title: Gates Foundation Open Access Policy Compatibility - WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - Gates Foundation Open Access Policy (January 2025, openaccess.gatesfoundation.org)
  - Gates Foundation Data Sharing Requirements (openaccess.gatesfoundation.org/how-to-comply/data-sharing-requirements/)
  - Gates Foundation Global Health Data Access Principles (docs.gatesfoundation.org/Documents/data-access-principles.pdf)
lens_tags:
  calibration_tier: independently_verified
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: private_foundation
  framework_scope_type: grantee_outcome_measurement
  # Bill and Melinda Gates Foundation Open Access Policy
---

# Gates Foundation Open Access Policy Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A WALKRI-conformant program satisfies the data availability and quality requirements of the Gates Foundation Open Access Policy (updated January 2025) as a structural consequence of conformance. WALKRI's evidence form requirement, applied at the field specification stage, produces the Data Availability Statement content that the Gates Policy requires at publication. WALKRI's five criterion specification requirements encode the same data quality properties that the Gates Global Health Data Access Principles require. Programs funded by the Gates Foundation that implement WALKRI do not produce Open Access Policy conformance documentation separately: WALKRI conformance produces it as a byproduct.

---

## What the Gates Foundation Open Access Policy Requires

The Gates Foundation Open Access Policy, updated January 2025, applies to all grantees receiving funding for research with publishable results. It requires:

**Data Availability Statement.** At the time of publication, grantees must include a statement specifying where underlying primary data, associated metadata, original software or code, and replication materials can be found. The statement must provide access paths that allow independent verification and reuse.

**Data Access Plan.** For grants exceeding $500,000 in global health funding, a Data Access Plan must be prepared before program activities begin. The plan must specify the data types to be collected, the access level (open, controlled, restricted), the access path, and the timeline for data availability.

**FAIR alignment.** The policy explicitly invokes FAIR principles and requires data to be "as open as possible, as closed as necessary." Open access is the default; restrictions require documented justification.

**Global Health Data Access Principles.** The companion Global Health Data Access Principles document specifies that data collected under Gates funding must be: discoverable (findable via a stable access path), accessible (retrievable without undue restriction), interoperable (in formats that allow combination with other datasets), and reusable (with sufficient documentation to support use by others). These are the FAIR principles under a different name.

---

## How WALKRI Satisfies the Open Access Policy

WALKRI's five criterion specification requirements, applied at the field specification stage before any applicant sees the form, produce the structural content of Gates Policy conformance.

**Evidence form requirement and Data Availability Statement.** The WALKRI evidence form requirement specifies, for every intake field, the artifact type that counts as evidence and the access path through which that artifact can be retrieved. Across all fields in a conformant form, the evidence form specifications collectively constitute a Data Availability Statement: they enumerate what data will be collected, in what form, and through which access paths. A program that has run WALKRI audit before publishing its form has already documented, for every data point it will collect, where and how that data can be independently verified.

| Gates requirement | WALKRI provision |
|:--|:--|
| Where primary data can be found | Evidence form: artifact type and access path per field |
| Metadata specification | WALKRI provenance envelope (field-specification-version, form-version, collection-timestamp, certification-level) |
| Software and code location | Evidence form for fields collecting code artifacts (URL to repository, branch or commit reference) |
| Replication materials | Evidence form for fields collecting process or methodology artifacts |
| FAIR compliance | WALKRI satisfies FAIR by construction (see below) |

**FAIR alignment.** WALKRI conformance satisfies the four FAIR principles as follows.

Findable: Every WALKRI-conformant field specification produces a conformance record with a stable URI. At Enhanced certification level the conformance record is published at that URI. Every submitted response envelope carries the conformance record URI in the walkri:provenance.conformance-record-ref field.

Accessible: Field specifications are published as JSON Schema with open, machine-readable format. No authentication is required to read WALKRI field specifications.

Interoperable: JSON Schema with x-walkri- extensions is parseable by any JSON Schema tool. The x-walkri- namespace is reserved for WALKRI use. WALKRI-conformant data from different programs is structurally comparable because the same field specification requirements were applied.

Reusable: The provenance envelope provides the version, specification metadata, and certification level required for a downstream consumer to assess reusability. A consumer who receives WALKRI-enriched data can determine which version of each field definition applied to the data and whether the form was certified.

**Data quality criteria.** The Gates Global Health Data Access Principles' four requirements (discoverable, accessible, interoperable, reusable) map directly to FAIR and are therefore satisfied by WALKRI conformance.

---

## Data Access Plan and WALKRI Stage 1 Audit

The Gates Policy requires a Data Access Plan to be prepared before program activities begin for qualifying grants. WALKRI's three-stage process is structured to produce this plan as a byproduct:

Stage 1 (criterion intent specification) declares, for each intake field, what it measures and why. This produces the data types documentation required by the Data Access Plan.

Stage 2 (operational definition and evidence form) specifies the access path, the artifact type, and the collection conditions for each field. This produces the access level and access path documentation required by the Plan.

Stage 3 (rubric validation and certification) confirms that every field meets conformance requirements before the form is published. This confirms that the Data Access Plan accurately represents what will be collected.

A program that has completed the WALKRI three-stage process before publishing its form has produced a Data Access Plan that satisfies the Gates Policy requirements as a byproduct of specifying its fields correctly.

---

## Scope

This compatibility statement applies to the WALKRI requirements for field specification quality. The Gates Open Access Policy also covers publication requirements (publishing in open-access venues, embargo periods, license requirements for publications). These are outside WALKRI's scope. WALKRI covers the data collection layer; the publication requirements are the responsibility of the program operator and the publishing team.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
