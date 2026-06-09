---
title: IATI v2.03 Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.3.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - IATI Standard v2.03 (iatistandard.org/en/iati-standard/203/)
  - IATI Activity Standard (iatistandard.org/en/iati-standard/203/activity-standard/)
  - IATI Organisation Standard (iatistandard.org/en/iati-standard/203/organisation-standard/)
  - IATI Codelists v2.03
lens_tags:
  calibration_tier: process_conformant
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: bilateral_aid_agency
  framework_scope_type: accounting_financial
  # International Aid Transparency Initiative; aid transparency data standard; primary funder typology bilateral_aid_agency for the publishing organizations; alternative multilateral_bank_or_fund
---

# IATI v2.03 Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS+WALKRI-conformant program can export its round configurations, gate evidence, and grantee reporting in IATI v2.03 format. CROSS's obligation architecture maps to IATI's Activity Standard, and WALKRI-conformant indicator data maps to IATI's result element with greater precision than IATI itself requires.

IATI is a publication format: it specifies how aid activity data must be structured for public disclosure. CROSS is an obligation architecture: it specifies what funded interventions must demonstrate at each gate. WALKRI is a specification quality layer: it specifies how collection instruments must be designed. The three are complementary at distinct layers. IATI consumes what CROSS and WALKRI produce; CROSS and WALKRI do not depend on IATI.

This compatibility matters for programs reporting to institutional donors who require IATI compliance, and for Web3 grants programs seeking to make their data consumable by the development sector's transparency infrastructure.

---

## What IATI Is

The International Aid Transparency Initiative (IATI) is a voluntary open data standard and publishing framework for development cooperation data. It was established in 2008 and is used by over 1,400 organizations including USAID, DFID/FCDO, UN agencies, the World Bank, the Gates Foundation, and hundreds of NGOs and implementing partners.

IATI specifies two publishing standards:

**The Organisation Standard**: describes the publishing organization's budgets, document links, and relationships to other organizations.

**The Activity Standard**: describes individual funded activities, their objectives, participating organizations, geographic scope, financial flows, conditions, results, and evidence. This is the primary standard for grants-related data.

The Activity Standard organizes activity data into hierarchical XML elements. The elements most relevant to grants programs are: `iati-activity` (the container), `title` and `description` (narrative), `participating-org` (funders and implementers), `activity-status` (lifecycle stage), `activity-date` (key dates), `sector` (thematic codes), `budget` and `transaction` (financial flows), `conditions` (grant conditions), `result` (indicators, baselines, targets, actuals), and `document-link` (evidence documents).

---

## CROSS Mapping to the IATI Activity Standard

### Activity-Level Mapping

| IATI Element | CROSS Equivalent | Notes |
| :-- | :-- | :-- |
| `iati-identifier` | Round identifier + grantee identifier | A CROSS-conformant program produces a stable identifier for each grantee at the entry gate. This identifier serves as the IATI activity identifier for the grantee's funded activity. |
| `title` | Project name from entry specification | |
| `description type="1"` (general) | Entry specification narrative (obligation mode + FROM/TO state or deliverable specification) | The CROSS entry specification is the machine-readable form of the IATI general description. |
| `description type="2"` (objectives) | TO state or completion criteria | The CROSS TO state (change-obligation) or completion criteria (build-obligation) is the objective description. |
| `activity-status` | Round stage + project stage | IATI activity-status codes map to CROSS stages: Pipeline/Identification (configuring), Implementation (active grant), Completion (completion gate passed), Cancelled (gate failure with formal record). |
| `activity-date type="1"` (planned start) | Round opening date | |
| `activity-date type="3"` (planned end) | Completion gate deadline | |
| `participating-org role="1"` (funding) | Funder (from funder configuration) | |
| `participating-org role="4"` (implementing) | Grantee (legal entity from organizational identity declaration) | |
| `sector` | Domain tags from sufficiency architecture declaration scope | CROSS's domain tags can be expressed as IATI sector codes using the OECD DAC sector codelist, the UN SDGS codelist, or a custom vocabulary declared in the measurement framework. |
| `budget` | Award amount from grant configuration | |
| `transaction type="3"` (disbursement) | Gate disbursement records | Each CROSS gate disbursement produces an IATI transaction record with the disbursement date, amount, and gate reference. |
| `conditions` | Gate conditions from completion verification + continuation specification | CROSS's gate conditions (conditions pending status, condition text, verification method) map directly to IATI's conditions element with condition type codes. |
| `document-link` | Gate evidence submissions | Each gate evidence submission is an IATI document-link referencing the evidence artifact (URL or cryptographically attributed attestation reference, in whatever format the program uses for gate records). |

### Result and Indicator Mapping

The IATI `result` element and its nested `indicator` element are the most analytically significant for grants reporting and verification. IATI's result element maps to CROSS's indicator specification as follows:

| IATI Element | CROSS Equivalent | Notes |
| :-- | :-- | :-- |
| `result type` | Obligation mode | IATI result types: 1=Output, 2=Outcome, 3=Impact, 4=Other. CROSS build-obligation indicators are IATI type 1; change-obligation indicators are IATI type 2 or 3 depending on the outcome level. |
| `indicator/title/narrative` | Indicator name (CROSS Field 1) | Direct correspondence. |
| `indicator/description/narrative` | Operational definition (CROSS Field 4) | CROSS requires a complete operational definition; IATI accepts a narrative description. CROSS is more prescriptive. |
| `indicator/baseline value` | Baseline / FROM state value (CROSS Field 10) | |
| `indicator/baseline year` | Baseline date from FROM state (CROSS Field 10) | |
| `indicator/period/target value` | Target / TO state value (CROSS Field 11) | |
| `indicator/period/actual value` | Completion gate reported value | The value reported at the CROSS completion verification gate. |
| `indicator measure` | Measurement form (CROSS Field 3) | IATI measure codes: 1=Unit, 2=Percentage, 3=Nominal, 4=Ordinal, 5=Qualitative. CROSS's open measurement form covers all five. |
| `indicator aggregation-status` | Cumulative/non-cumulative designation (CROSS Field 6) | Direct correspondence. |
| (not in IATI) | Rationale for indicator (CROSS Field 2) | IATI has no rationale field. CROSS requires documented rationale for each indicator choice. |
| (not in IATI) | Construction and aggregation methodology (CROSS Field 5) | IATI has no methodology field. CROSS requires the counting rule and aggregation method. |
| (not in IATI) | Disaggregation specification (CROSS Field 7) | IATI accepts disaggregated actuals but does not specify how disaggregation must be defined. CROSS's disaggregation field specifies which breakdowns are required and enforces a disaggregation ratchet across reporting periods. |
| (not in IATI) | Data cost estimation (CROSS Field 9) | IATI has no data cost field. |
| (not in IATI) | WALKRI criterion specification | IATI has no collection instrument specification requirement. WALKRI fills this gap entirely. |

**Result:** A CROSS-conformant program's indicator data can be exported to IATI result elements without additional mapping work. The CROSS fields that have no IATI equivalent are not lost; they are carried in the CROSS data structure and can be included in IATI document-link references or in the IATI `result/indicator/reference` element using the `x-cross` namespace.

---

## WALKRI and IATI: The Collection Instrument Gap

IATI specifies what to publish but not how the data was collected. A result element in IATI can reference an indicator with a target and an actual value, but it contains no information about how the collection instrument was designed, whether the instrument was valid and reliable, or whether the "actual value" was produced by the same methodology as the baseline and target.

This is IATI's fundamental data quality limitation. It produces transparency (the data is public and machine-readable) without specification quality (the data may be incommensurable across programs because collection instruments were defined differently).

WALKRI addresses this limitation at the collection instrument level. A WALKRI-conformant field specification, when published alongside or embedded within an IATI activity, provides:

- The criterion intent (what the indicator actually measures, not just its name)
- The operational definition (what counts and what does not)
- The evidence form (what artifact verifies the value)
- The data quality standards (validity, integrity, precision, reliability, timeliness)

This information can be expressed in IATI using the `indicator/reference` element with the `x-walkri` vocabulary reference, or as a `document-link` to the published WALKRI field specification. Either approach makes the collection instrument specification machine-readable alongside the IATI data, enabling downstream consumers to assess not only what a program reported but how reliably the reporting instrument was designed.

---

## IATI and DAOIP-5: The Two-World Bridge

IATI is the publication standard of the institutional development sector. DAOIP-5 is the grants metadata standard of the Web3 ecosystem. A CROSS+WALKRI-conformant program exports to both without additional work.

The CROSS round configuration maps to a DAOIP-5 GrantPool object (Part IX-A of CROSS). The same round configuration maps to an IATI activity record following the mapping in this document. The grantee's completed grant maps to a DAOIP-5 Project object and Attestation objects, and to an IATI activity with result actuals and document-links.

This means a CROSS+WALKRI-conformant program produces data that is simultaneously readable by:

- The OpenGrants Gateway API maintained by Metagov (via DAOIP-5 export)
- IATI datastore and tools consuming IATI v2.03 XML (via IATI export)
- Any system processing the attestation format used for gate evidence (W3C VCs, EAS attestations, DAOIP-3 VCs, signed documents, or comparable mechanisms)
- Any FAIR-compliant data pipeline (via WALKRI provenance fields)

No other grants standard produces data that is natively consumable by both the institutional development sector's transparency infrastructure and the Web3 ecosystem's grants infrastructure. This is the two-world bridge that CROSS+WALKRI uniquely enables.

---

## IATI Codes for CROSS Obligation Modes

Programs publishing CROSS-conformant grants data in IATI format should use the following IATI codelist values:

**Result type** (maps to CROSS obligation mode):
- Build-obligation grants: `type="1"` (Output)
- Change-obligation grants targeting short-term or intermediate outcomes: `type="2"` (Outcome)
- Change-obligation grants targeting long-term outcomes or contributing to a goal: `type="3"` (Impact)
- Retroactive-obligation grants: `type="2"` (Outcome), with a `reference` attribute citing the CROSS retroactive obligation specification

**Activity status** (maps to CROSS round and project stage):
- Round configuring: `code="1"` (Pipeline/Identification)
- Round accepting applications: `code="1"` (Pipeline/Identification)
- Entry gate passed, work active: `code="2"` (Implementation)
- Completion gate passed: `code="3"` (Completion)
- Entry gate failed or application withdrawn: `code="5"` (Cancelled)
- Continuation gate passed: begin a new linked activity with `related-activity type="2"` (Parent)

**Condition type** (maps to CROSS gate conditions):
- Entry gate conditions (pre-disbursement): `type="1"` (Policy)
- Completion gate conditions: `type="2"` (Performance)
- Continuation gate conditions: `type="2"` (Performance)

---

## Adoption Guidance

Programs that currently publish IATI data and are adopting CROSS+WALKRI should:

1. Map their existing IATI activities to CROSS obligation modes. Activities with outcome-oriented result types (type 2 or 3) are change-obligation; activities with output-oriented result types (type 1) are build-obligation.

2. Enrich existing IATI result elements with CROSS indicator fields. The CROSS operational definition, methodology, disaggregation specification, and rationale fill the gaps that IATI's result element leaves open. These can be added as IATI `indicator/description` narrative or as referenced documents.

3. Apply WALKRI criterion specification requirements to each field in the data collection instruments that produce IATI result actuals. Publish the WALKRI field specifications as IATI document-link elements with `category="A08"` (Programme/Activity evaluation) or a custom vocabulary reference.

4. Configure DAOIP-5 export alongside IATI export. The same CROSS+WALKRI-conformant data feeds both; the export formats differ but the source data is identical.

Programs that have not previously published IATI data and are adopting CROSS+WALKRI will find that CROSS+WALKRI conformance produces all the data required for IATI publication. No additional data collection is needed; the IATI XML can be generated from the CROSS round configuration, indicator specifications, gate records, and disbursement transactions.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

IATI Standard v2.03: iatistandard.org/en/iati-standard/203/

IATI Datastore: datastore.iatistandard.org

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
