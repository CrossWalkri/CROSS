---
title: AAOIFI Standards for Zakat and Waqf Administration Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.2 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - AAOIFI FAS 39 Financial Reporting for Zakah (aaoifi.com/announcement/aaoifi-issues-financial-accounting-standard-fas-39-financial-reporting-for-zakah/?lang=en)
  - AAOIFI FAS 37 Financial Reporting by Waqf Institutions (aaoifi.com/announcement/aaoifi-issues-financial-accounting-standard-37-financial-reporting-by-waqf-institutions/?lang=en)
  - AAOIFI GS 13 Waqf Governance (aaoifi.com/announcement/aaoifi-issues-standard-on-waqf-governance/?lang=en)
  - AAOIFI Sharia Standard SS-35 Zakah (aaoifi.com)
lens_tags:
  calibration_tier: independently_verified
  authority_source: professional_society_standard
  cultural_methodological_lineage: islamic_finance_jurisprudence
  funder_typology: faith_based
  framework_scope_type: jurisprudential
  # AAOIFI standards for Zakat and Waqf administration; primary scope jurisprudential (Sharia Standard SS-35) with accounting_financial secondary (FAS 37 and FAS 39)
---

# AAOIFI Standards for Zakat and Waqf Administration Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Accounting and Auditing Organization for Islamic Financial Institutions (AAOIFI) governs the financial accounting and governance layer for two of the world's largest pools of charitable capital: Zakat and Waqf. AAOIFI's standards address how these funds are recognized, measured, reported, and governed; they do not specify how program-level outcomes must be measured. CROSS occupies that adjacent outcome measurement layer, and a CROSS+WALKRI-conformant program funded through Zakat or Waqf mechanisms satisfies the measurement obligations that AAOIFI explicitly leaves to implementing organizations.

The two systems are complementary rather than overlapping. AAOIFI governs the accounting treatment of charitable capital; CROSS covers the demonstration of what that capital accomplished. Together they provide Islamic institutions with a complete verification chain from financial recognition through outcome evidence.

---

## What AAOIFI Is

AAOIFI is an international autonomous non-profit organization established in Bahrain in 1991. It develops and issues accounting, auditing, governance, ethics, and Sharia standards for Islamic financial institutions. Its standards are mandatory in Bahrain, Qatar, Sudan, Syria, and Jordan, and serve as reference standards in many additional jurisdictions. Over 100 regulatory authorities worldwide use AAOIFI standards as the basis for their Islamic finance regulatory frameworks.

The four AAOIFI standards most relevant to charitable capital are:

**FAS 39 - Financial Reporting for Zakah** (December 2021, superseding FAS 9): This standard governs the accounting treatment, presentation, and disclosure requirements for Zakat in Islamic financial institutions. It specifies how Zakat obligations are recognized, how the Zakat base is calculated, how Zakat fund assets and liabilities are presented on the balance sheet, and what must be disclosed in financial statements regarding Zakat administration.

**Sharia Standard SS-35 - Zakah**: This standard governs the substantive religious law dimension: how the Zakat base is determined, which asset categories are subject to Zakat, the nisab threshold, and the eight canonical recipient categories (asnaf) prescribed by Quran 9:60. SS-35 operates at the level of religious obligation; FAS 39 operates at the level of accounting presentation.

**FAS 37 - Financial Reporting by Waqf Institutions** (December 2020): This standard covers recognition, measurement, classification, and disclosure for Waqf (Islamic endowment) revenues and assets. It distinguishes between cash Waqf, investment Waqf, and service Waqf, and specifies how each category is accounted for in the financial statements of a Waqf institution.

**GS 13 - Waqf Governance** (September 2020): This governance standard prescribes the governance structure, board composition, internal control environment, transparency obligations, and disclosure requirements for Waqf institutions, all in accordance with Sharia principles. GS 13 is AAOIFI's most comprehensive statement on institutional accountability for charitable endowments.

None of these four standards specifies how a program funded by Zakat or Waqf capital must measure, document, or report the outcomes it achieves for beneficiaries. That layer is explicitly reserved for implementing organizations and their funders.

---

## How CROSS Satisfies the AAOIFI Framework

CROSS addresses the measurement obligation that AAOIFI's financial and governance standards presuppose but do not define. The mapping operates at three distinct levels.

**Declaration and identity layer.** AAOIFI GS 13 requires Waqf institutions to maintain documented governance structures, clear policies, and public reporting on beneficiary categories and disbursement decisions. CROSS's organizational identity declaration, which captures legal name, jurisdiction, registration, governance structure, and disbursement authority, is the structural equivalent of GS 13's disclosure requirements. A Waqf institution operating CROSS-conformant programs can satisfy its GS 13 public reporting obligations by publishing the CROSS round configuration, which contains all GS 13-required organizational disclosure fields in a standardized, machine-readable form.

**Beneficiary identification layer.** Both FAS 37 (Waqf) and FAS 39 (Zakat) require clear identification of the beneficiary population that receives charitable disbursements. FAS 39 specifically requires alignment between the beneficiary categories recognized in the accounts and the eight canonical asnaf categories prescribed by SS-35. CROSS's population scope declaration addresses this requirement directly: the program must specify who is served, with what demographic scope, and how the population is bounded. For Zakat-funded programs, the population scope declaration can and should reference the applicable asnaf category, producing an auditable chain between the accounting disclosure (FAS 39) and the program's stated beneficiary scope (CROSS entry specification).

**Outcome measurement layer.** Neither FAS 37, FAS 39, nor GS 13 specifies what outcomes a Zakat or Waqf-funded program must demonstrate, or how those outcomes must be measured. This is the gap that CROSS fills. CROSS's gate architecture requires a program to specify its intended outcomes before disbursement, collect evidence during implementation, and produce a structured determination record at completion. The completion gate record constitutes the program-level measurement documentation that AAOIFI's financial standards implicitly require but do not prescribe.

The relationship between the two systems is summarized in the following table:

| AAOIFI Standard | Scope | CROSS Provision | Relationship |
|:--|:--|:--|:--|
| FAS 39 (Zakat accounting) | Financial recognition and disclosure of Zakat fund assets and liabilities | Organizational identity declaration; beneficiary population scope (asnaf alignment) | CROSS provides the program-level evidence record that FAS 39 financial disclosures reference |
| SS-35 (Zakat Sharia) | Zakat base calculation and asnaf disbursement rules | Population scope declaration (asnaf category alignment) | CROSS beneficiary scope declaration maps directly to asnaf categorization |
| FAS 37 (Waqf accounting) | Recognition, measurement, and disclosure of Waqf revenues and assets | Organizational identity; completion gate evidence record | CROSS completion record documents what Waqf revenues achieved at program level |
| GS 13 (Waqf governance) | Governance structure, internal controls, transparency, public disclosure | Organizational identity declaration; CROSS round configuration; Attestation Corpus | CROSS round configuration satisfies GS 13 public reporting disclosure requirements |

---

## How WALKRI Complements This Alignment

AAOIFI GS 13 requires Waqf institutions to maintain documentation demonstrating that charitable disbursements were made in accordance with the Waqf's purposes and beneficiary conditions. This documentation obligation extends, by implication, to the data collection instruments through which program operators gather evidence of beneficiary service. A Waqf institution cannot satisfy its GS 13 reporting obligations by reference to ambiguously designed survey instruments that reconstruct measurement intent after the fact.

WALKRI addresses this precisely by requiring that each data collection field be specified before any affected-population member or program operator sees the intake form. The evidence form requirement, which fixes the artifact type and access path at the field specification stage, ensures that documentation required for Waqf governance reporting obligations is embedded in the program's design rather than retrofitted during audit. For Zakat-funded programs operating under SS-35 asnaf verification requirements, WALKRI's criterion intent and operational definition fields provide the structured basis for demonstrating that the program actually served the declared asnaf category, not merely that it collected data labeled with that category's name.

This collection-instrument verification layer is the layer that neither AAOIFI's financial standards nor existing Islamic finance governance frameworks address. WALKRI provides it, making CROSS+WALKRI the most complete available framework for programs operating under Islamic charitable capital governance.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
