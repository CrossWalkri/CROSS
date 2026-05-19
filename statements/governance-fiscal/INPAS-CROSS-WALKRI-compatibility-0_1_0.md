---
title: International Non-Profit Accounting Standard (INPAS) Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.3 (github.com/cross-walkri/CROSS), WALKRI v0.1.7 (github.com/cross-walkri/WALKRI)
references:
  - https://ifr4npo.org
  - https://humentum.org/international-financial-reporting-for-nonprofit-organizations/
  - https://www.cipfa.org/about-cipfa/press-office/latest-press-releases/first-global-accounting-standard-for-non-profits-launched
---

# International Non-Profit Accounting Standard (INPAS)

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The International Non-Profit Accounting Standard (INPAS), launched in October 2025 through an initiative led by Humentum and CIPFA under the stewardship of the International Non-Profit Reporting Foundation (INPRF), is the first global accounting standard designed specifically for nonprofit organizations. INPAS governs recognition, measurement, presentation, and disclosure requirements for nonprofit financial reporting, with particular attention to grant income recognition, restricted versus unrestricted fund presentation, and harmonized grant reporting. CROSS+WALKRI produces the intake and program-level documentation that INPAS requires for accurate grant income classification, restriction status determination, and comparative financial reporting, as a structural byproduct of conformance rather than as a separate compliance activity.

---

## The INPAS Framework

Until October 2025, no global accounting standard addressed the specific financial reporting characteristics of nonprofit organizations receiving grants. The International Financial Reporting Standards (IFRS) and Generally Accepted Accounting Principles (GAAP) frameworks were designed primarily for commercial entities and, while adaptable, did not directly address the recognition, measurement, and disclosure questions that arise specifically in grant-funded nonprofit contexts. INPAS fills this gap.

INPAS was developed through an initiative led by Humentum (the global network for operational excellence in international development) and CIPFA (the Chartered Institute of Public Finance and Accountancy), with stewardship by the International Non-Profit Reporting Foundation. The resulting standard is accrual-based, designed to stand alone as a complete accounting framework for nonprofit entities, and covers the four core areas of any accounting standard: recognition, measurement, presentation, and disclosure.

For nonprofit organizations receiving grants, the most consequential areas of INPAS are grant income recognition and restricted versus unrestricted fund presentation. Grant income recognition under INPAS requires that each grant be classified at the point of recognition: whether it is restricted or unrestricted, what the restriction purpose is (if restricted), what period the restriction covers, and what evidence demonstrates that restriction conditions have been met or that the restriction has been lifted. These are not post-hoc financial reporting decisions: they depend on data that must be collected at the intake stage before any programmatic activity begins.

The INPAS Practice Guide for harmonized grant reporting addresses the specific requirements for producing comparative grant reporting data across multiple funders, grant periods, and program types. Harmonized reporting requires that data be collected consistently across programs so that financial statements can present grants on a comparable basis. This places requirements on the intake process that go beyond what most grant programs have historically implemented: the classification data required for a harmonized INPAS financial statement must be collected with the precision and consistency that accrual-based accounting requires.

For cohort 1 of the grants ecosystem (nonprofit grantee organizations) and cohort 3 (program operators producing financial reports), INPAS represents a significant shift in what financial reporting compliance requires. Every nonprofit grantee that produces INPAS-compliant financial statements needs intake data that satisfies INPAS's classification requirements. The demand for that data originates in the financial reporting obligation, but the data itself must be collected at the grant intake and program design stage, before the reporting period begins.

---

## How CROSS Satisfies the INPAS Framework

CROSS produces the program-level documentation that INPAS's grant income recognition and restricted fund presentation requirements demand. The mapping below connects each INPAS requirement to the CROSS mechanism that generates the required data.

| INPAS Requirement | CROSS Mechanism |
|---|---|
| Grant income recognition: restriction status at recognition | CROSS obligation mode declaration: Build/Change mode corresponds to restricted grants designated for specific deliverables or outcomes; Retroactive mode corresponds to unrestricted recognition of prior work already completed. |
| Grant income recognition: restriction purpose | CROSS indicator specification Fields 1-5 (name, definition, unit, baseline, target): the restriction purpose is precisely what these fields document at the indicator level. |
| Grant income recognition: restriction period | CROSS concurrent funding disclosure: all funding sources, amounts, purposes, and periods documented for the same program, providing the period-specific allocation data INPAS requires. |
| Restricted fund presentation | CROSS indicator specification Fields 1-11 collectively: each indicator is associated with the restricted grant purpose, period, and population to which it applies, producing the restricted fund documentation that INPAS requires for financial statement presentation. |
| Practice Guide for harmonized grant reporting | CROSS gate record format: structured determination records at each gate produce harmonized reporting data in a consistent format across programs. The gate record structure ensures comparability across programs, funders, and grant periods. |
| Disclosure requirements (evidence that restriction conditions have been met) | CROSS progress verification gate and completion gate records: each gate record documents what evidence was reviewed and what determination was reached, creating the evidentiary basis for lifting a restriction at the appropriate accounting period. |

The obligation mode declaration mapping is particularly important for INPAS compliance. INPAS requires that restriction status be determined at the point of recognition: a grant classified as restricted must have a documented restriction purpose, and a grant classified as unrestricted must have documentation supporting that classification. CROSS's obligation mode declaration makes this determination explicit at the entry gate: Build mode declares that funds are designated for future deliverables (restricted); Retroactive mode declares that funds recognize work already completed (unrestricted or conditionally unrestricted depending on the specific grant terms). The declaration is timestamped, included in the Attestation Corpus, and independently verifiable.

The concurrent funding disclosure mapping addresses the fund presentation requirement. INPAS requires that restricted funds be presented separately from unrestricted funds, and that restricted funds be further disaggregated by purpose and period where material. CROSS's concurrent funding disclosure documents all funders, funding amounts, restriction purposes, and periods for the same program in a single structured record. A nonprofit grantee with CROSS-conformant programs has the fund-level documentation needed to prepare INPAS-compliant financial statements without reconstructing allocation data after the fact.

The gate record mapping supports the disclosure requirement in a less obvious but operationally critical way. INPAS requires that nonprofit organizations disclose the evidence basis for recognizing restricted grant income: what conditions were required, what evidence demonstrates those conditions were met, and at what point the recognition event occurred. CROSS gate records document precisely this: what evidence was reviewed (progress verification gate), what conditions were satisfied (completion gate), and when the determination was made (timestamped gate record). The audit trail required for INPAS disclosure exists as a byproduct of CROSS conformance.

---

## How WALKRI Complements This Alignment

WALKRI's pre-publication audit requirement addresses the most upstream INPAS risk: erroneous restriction classification at the intake stage. INPAS's grant income recognition requirements depend on data that must be correct at the point of collection. If a grant's restriction purpose is ambiguously specified in the intake form, the resulting classification may be inaccurate, and that inaccuracy propagates directly into financial statement misstatements. Restriction classification errors are not correctable by better reporting practices: the error occurs at intake and compounds through the grant period.

WALKRI requires that intake fields collecting restriction status, purpose documentation, and period specification function as measurement instruments before any applicant responds. Each field must specify the defined term, unit, baseline, evidence access path, and population scope. For INPAS purposes, this means that the fields collecting grant classification data, restriction purpose documentation, and period allocation information must be specified with the precision that accrual-based accounting requires: a defined term that corresponds to a recognized accounting category, a unit that enables consistent classification across applicants, and an evidence access path that an auditor can follow independently.

The practical consequence is significant. A grant program operating WALKRI-conformant intake forms collects restriction classification data that is consistent across all applicants, traceable to specified sources, and precise enough to support INPAS recognition entries. A grant program operating loosely specified intake forms collects restriction classification data that is inconsistent across applicants, dependent on how each applicant interpreted the question, and imprecise enough that restriction classification requires interpretive judgment at the accounting stage. The second approach creates INPAS compliance risk; the first eliminates it structurally.

INPAS is the first accounting standard that directly governs how nonprofit organizations account for grants received. Its arrival makes the quality of grant intake data a financial reporting compliance question rather than merely a program quality question. CROSS+WALKRI produces the structured, consistent, independently verifiable intake and program documentation that INPAS compliance requires, as a natural byproduct of program conformance.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
