---
title: DDI Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.3.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - DDI Codebook 2.5 (ddialliance.org/Specification/DDI-Codebook/2.5/)
  - DDI Lifecycle 3.3 (ddialliance.org/Specification/DDI-Lifecycle/3.3/)
  - DDI-CDI 1.0 (ddialliance.org/Specification/DDI-CDI/)
lens_tags:
  calibration_tier: process_conformant
  authority_source: professional_society_standard
  cultural_methodological_lineage: western_institutional
  funder_typology: pooled_fund_or_intermediary
  framework_scope_type: accounting_financial
  # Data Documentation Initiative metadata standard for research data; professional society DDI Alliance; data documentation framework treated as accounting/disclosure analog; alternative framework_scope_type professional_practice_ethics
---

# DDI Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

WALKRI's field specification requirements produce DDI-compatible variable-level metadata as a structural consequence of conformance. Programs using WALKRI-conformant collection instruments produce datasets that satisfy DDI Codebook 2.5 documentation requirements for variable metadata without additional work.

DDI (Data Documentation Initiative) is the metadata standard for social science and research data documentation. It specifies how datasets, variables, and collection instruments should be documented for archiving, discovery, and reuse by other researchers and data consumers. WALKRI is the field-level precision standard for grants and program evaluation intake instruments. They address the same problem from different disciplinary starting points: both require collection instruments to be documented with enough precision that a data consumer who did not design the instrument can understand what it measured and reproduce the collection methodology.

---

## What DDI Is

The Data Documentation Initiative is an international metadata standard maintained by the DDI Alliance. Three versions are in active use:

**DDI Codebook (2.x)**: The most widely deployed version. Used by national statistics agencies, social science data archives (ICPSR, GESIS, UK Data Service), and survey research organizations. It documents studies, questionnaires, variables, and datasets in XML. The `var` element (variable) is the primary unit for field-level documentation.

**DDI Lifecycle (3.x)**: A more comprehensive version covering the full research data lifecycle from conceptualization through archiving. The `StudyUnit` element corresponds to a study or program; the `QuestionItem` and `Variable` elements document collection instruments and their outputs.

**DDI-CDI (Cross Domain Integration)**: A newer version for federated data integration across disciplines and systems. Not yet widely deployed but relevant for the cross-program data aggregation that CROSS+WALKRI enables.

---

## WALKRI Mapping to DDI Variable Metadata

The DDI Codebook `var` element specifies the documentation required for each variable in a dataset. WALKRI's five criterion specification requirements produce all required DDI variable metadata:

| DDI `var` Element | WALKRI Equivalent | Notes |
| :-- | :-- | :-- |
| `var/labl` (label) | Field label | The display label. WALKRI requires the label to be distinct from the criterion intent; DDI accepts the label as the primary identifier. |
| `var/concept` (concept) | Criterion intent (Section 3.1) | DDI's concept element specifies the underlying construct being measured. WALKRI's criterion intent is the precise statement of that construct. |
| `var/universe` (universe) | Operational definition scope (Section 3.2) | DDI's universe specifies who or what the variable applies to. WALKRI's operational definition specifies the qualifying and non-qualifying cases, which is a more precise statement of universe. |
| `var/qstn` (question text) | Field label + operational definition | DDI documents the question as it appeared to respondents. WALKRI requires this plus the operational definition that constrains interpretation. |
| `var/catgry` (categories) | Operational definition options (Section 3.2) | For categorical variables, DDI documents each category. WALKRI requires each option to be defined with qualifying and non-qualifying examples. |
| `var/varFormat` (format) | Response form (Section 3.3) | DDI specifies the data type. WALKRI requires the response form with a justification for why that type is appropriate. |
| `var/sumStat` (summary statistics) | Evidence form (Section 3.4) | DDI documents summary statistics for archiving. WALKRI documents the evidence artifact that validates the collected value. These are complementary: DDI describes the data; WALKRI describes the evidence. |
| `var/notes` (notes) | Conformance threshold (Section 3.5) | DDI's notes field captures supplementary documentation. WALKRI's conformance threshold specifies the minimum evidence requirement for external standard references. |
| (not in DDI `var`) | Criterion specification version | WALKRI's provenance fields (Part VII) include the field specification version and the specification timestamp. DDI's dataset-level metadata tracks data collection dates; WALKRI tracks the instrument specification dates separately. |

### Provenance Mapping

WALKRI's provenance fields (Part VII) map to DDI dataset-level and variable-level provenance elements:

| WALKRI Provenance Field | DDI Equivalent |
| :-- | :-- |
| Field creator identity | `var/respUnit` (responsible unit) |
| Specification timestamp | `codeBook/docDscr/citation/prodDate` (production date) |
| WALKRI version | `codeBook/docDscr/citation/verStmt` (version statement) |
| Form tool identifier | `codeBook/stdyDscr/method/dataColl/collMode` (collection mode) |
| Field specification version | `var/verStmt` (version statement) |

A WALKRI-enriched dataset carries sufficient provenance to satisfy DDI archival requirements for variable-level documentation. Datasets produced by WALKRI-conformant programs can be deposited in DDI-aware archives (ICPSR, GESIS, UK Data Service) without requiring additional metadata preparation.

---

## CROSS Mapping to DDI Study-Level Metadata

At the study level, DDI Lifecycle's `StudyUnit` element corresponds to a CROSS round or program:

| DDI Lifecycle Element | CROSS Equivalent |
| :-- | :-- |
| `StudyUnit` | CROSS round (single grant cycle) |
| `StudyUnit/Purpose` | Obligation mode + entry specification |
| `StudyUnit/Coverage/TopicalCoverage` | Domain tags from sufficiency architecture declaration |
| `StudyUnit/Coverage/TemporalCoverage` | Round opening and closing dates |
| `StudyUnit/Coverage/SpatialCoverage` | Geographic scope from program-level ToC declaration (Part IX-B) |
| `DataCollection/QuestionScheme` | Application form (WALKRI-specified fields) |
| `LogicalProduct/VariableScheme` | CROSS indicator specifications (Part V) |
| `Archive/ArchiveSpecific/Collection` | Gate evidence submissions and attestations |

---

## FAIR Alignment: DDI and WALKRI Converge

Both DDI and WALKRI are designed to produce FAIR-compliant (Findable, Accessible, Interoperable, Reusable) data. Their approaches converge:

**Findability**: DDI provides persistent identifiers and searchable metadata at the study and variable level. WALKRI's provenance fields provide field-level identifiers and specification timestamps. Together they produce FAIR-compliant findability at both the dataset and instrument levels.

**Accessibility**: DDI specifies access conditions at the dataset level. WALKRI's access model for external standards (open/free, open/registration, paid/licensed, government/regulatory) specifies access conditions at the field level. Combined, they document access at both levels without duplication.

**Interoperability**: DDI uses XML as its primary format. WALKRI uses JSON Schema as its native format, which underlies all major form tools. The two formats are complementary: JSON Schema covers data collection; DDI XML covers archival documentation. A WALKRI field specification can be transformed to DDI variable documentation programmatically.

**Reusability**: DDI's concept and universe elements make variables reusable by other researchers. WALKRI's criterion intent and operational definition produce the same reusability guarantee at the field level, with the additional requirement that qualifying and non-qualifying examples be documented.

---

## Croissant Alignment: WALKRI, DDI, and ML Pipelines

The Croissant format (ml-croissant.github.io) is a metadata layer for machine learning datasets that bridges human-readable documentation and machine-readable schemas. Both DDI and WALKRI are Croissant-aligned: DDI provides study-level and variable-level metadata that Croissant can consume; WALKRI provides field-level provenance and specification metadata that Croissant requires for ML-ready datasets.

A dataset produced by a WALKRI-conformant program satisfies Croissant metadata requirements through the WALKRI provenance fields (field creator, specification timestamp, version) and the operational definitions (which Croissant uses to describe field semantics to ML pipelines). Where DDI documentation is also available, the combined DDI + WALKRI metadata produces richer Croissant output than either standard alone.

---

## Who Should Declare DDI Compatibility

Programs in the following contexts will find DDI compatibility most valuable:

**Academic and research programs**: Universities, think tanks, and research institutes using grants programs to fund data collection. WALKRI-conformant collection instruments produce DDI-compatible data archival documentation automatically, making the research data archivable in ICPSR, GESIS, or equivalent repositories without additional preparation.

**National statistics integration**: Programs that collect data that will be integrated with national statistics agency datasets. DDI is the standard most national statistics agencies use for variable documentation. WALKRI-conformant programs produce DDI-compatible variable metadata as a conformance consequence.

**Programs bridging research and program evaluation**: Many development programs produce both programmatic data (for reporting) and research data (for publication). WALKRI-conformant instruments produce data that satisfies both evaluation reporting requirements (CROSS's gate evidence standards) and research archival requirements (DDI's variable documentation standards).

---

## Adoption Guidance

Programs that currently use DDI documentation and are adopting CROSS+WALKRI should:

1. Map existing DDI `var` elements to WALKRI field specifications. The DDI concept, universe, and category elements contain the same information as WALKRI's criterion intent, operational definition, and operational definition options respectively. Completing the WALKRI specification fills the DDI gaps (evidence form, conformance threshold) while the DDI documentation fills the WALKRI gaps (summary statistics, archival notes).

2. Use WALKRI's JSON Schema output as the source of truth for field specifications. Generate DDI XML from the JSON Schema using the mapping table in this document. This maintains a single source of truth rather than maintaining parallel DDI and WALKRI documentation.

3. Declare DDI-CDI compatibility where cross-program data aggregation is planned. The `x-walkri` namespace within DDI-CDI can carry WALKRI field specification references, enabling federated data consumers to assess the specification quality of fields across programs.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

DDI Alliance: ddialliance.org

DDI Codebook 2.5: ddialliance.org/Specification/DDI-Codebook/2.5/

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
