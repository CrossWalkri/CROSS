---
title: 2 CFR 200 (OMB Uniform Guidance for Federal Awards) Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.4 (github.com/cross-walkri/CROSS), WALKRI v0.1.7 (github.com/cross-walkri/WALKRI)
references:
  - https://www.ecfr.gov/current/title-2/subtitle-A/chapter-II/part-200
  - https://www.epa.gov/grants/whats-new-2024-revision-2-cfr-part-200
---

# 2 CFR Part 200 (OMB Uniform Guidance for Federal Awards)

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

Title 2 of the Code of Federal Regulations, Part 200, sets the foundational financial accountability architecture for every recipient of US federal grant funds, regardless of awarding agency. CROSS's gate structure, Attestation Corpus, and conflict of interest provisions directly satisfy the audit trail, internal control, and monitoring documentation requirements that 2 CFR 200 imposes on grant recipients and prime award passthrough entities. WALKRI's pre-publication field specification requirement addresses cost classification at source, reducing the misclassification risk that Subpart E cost principle audits most commonly flag.

---

## The Regulation's Approach

The OMB Uniform Guidance (revised 2024) operates upstream of every agency-specific grant framework. USAID PIRS, NIH grant terms, GREAT Act reporting, and NSF data management requirements must all comply with 2 CFR 200; none of them supersede it. This means that any grantee receiving federal funds occupies two distinct accountability regimes simultaneously: the agency's programmatic performance framework and 2 CFR 200's financial accountability framework. These are not redundant; they govern different things. Agency frameworks address what the program achieved. 2 CFR 200 addresses whether the organization that ran the program can demonstrate that its finances were managed lawfully and its records can withstand independent audit.

Subpart F establishes the Single Audit requirement: any non-federal entity expending $750,000 or more in federal awards during a fiscal year must obtain an independent audit of the entire organization (not merely of the individual award), with findings submitted to the Federal Audit Clearinghouse. The audit assesses the organization's financial statements and its compliance with major federal program requirements. The audit trail that a Single Audit reviewer uses is the same trail that CROSS's completion gate documentation and Attestation Corpus produce: a timestamped, independently verifiable record of what was claimed, what evidence was presented, and what an independent reviewer assessed.

Subpart E establishes the cost principles governing what recipients may charge to a federal award. Direct costs must be allocable, allowable, and reasonable. Indirect costs must be charged at a negotiated or de minimis rate. The critical compliance point in Subpart E is not conceptual understanding of these categories but operational classification: at the moment a cost is incurred, it must be classified correctly. After-the-fact reclassification is a primary trigger for audit findings and disallowed costs.

Subrecipient monitoring under Subpart D creates a secondary compliance obligation. When a prime award recipient passes federal funds to a sub-grantee, it becomes responsible for verifying that sub-grantee's risk posture, audit history, and financial controls before and during each disbursement. This is not optional; failure to perform and document subrecipient monitoring is itself an audit finding.

The record retention requirement (three years post-closeout) and the internal controls requirement (written policies, separation of duties, documentation of all transactions) complete the compliance architecture. Internal controls under 2 CFR 200 are not merely administrative best practice; they are a compliance condition, and their absence or inadequacy constitutes a material weakness reportable in the Single Audit.

---

## How CROSS Satisfies 2 CFR 200

The following table maps the primary 2 CFR 200 requirements to the CROSS provisions that satisfy or directly support them.

| 2 CFR 200 Requirement | CROSS Provision |
|---|---|
| Single Audit (Subpart F): entity-level independent audit | CROSS independent attestation pathway. The completion gate documentation and Attestation Corpus constitute the audit trail a Single Audit reviewer uses to assess program compliance. |
| Subrecipient monitoring (Subpart D): prime must verify sub-grantee identity, risk, and audit status before each disbursement | CROSS organizational identity fields (legal name, jurisdiction, registration, governance structure, disbursement authority) + concurrent funding disclosure. These structured records satisfy the documentation requirements for Subpart D monitoring. |
| Cost principle compliance (Subpart E): allowable vs. unallowable cost classification | CROSS Attestation Corpus. What was claimed at each gate and what evidence was provided creates the verification trail Subpart E auditors require. |
| Record retention: three years post-closeout | CROSS Attestation Corpus persistence. Gate records are retained indefinitely in verifiable form, exceeding the three-year minimum. |
| Internal controls: written policies, separation of duties, documentation of all transactions | CROSS conflict of interest provisions (Part VII) combined with the CROSS pre-commitment record. The pre-commitment record provides independently verifiable evidence that evaluation criteria existed before any submission arrived, which is the structural equivalent of separation of duties in a review process. |

The Single Audit relationship deserves expansion. A Single Audit does not audit a single grant; it audits the organization across all its major federal programs. The auditor selects major programs based on expenditure thresholds and risk factors. For any selected program, the auditor tests whether the recipient maintained adequate records, whether expenditures were allowable, and whether the recipient complied with program-specific requirements. CROSS's gate structure, by requiring that claims and evidence be submitted and reviewed at defined intervals with independent attestation, creates exactly the record structure that this program-specific compliance testing examines. Organizations without a CROSS-equivalent gate structure must reconstruct that record retrospectively, which is both unreliable and a recognized audit risk.

The subrecipient monitoring mapping is equally direct. When a prime award recipient must verify and document its sub-grantees before each disbursement, it needs structured data about those sub-grantees. CROSS organizational identity fields provide that structure in a standardized format that can be referenced across multiple disbursement cycles without reformatting.

---

## How WALKRI Complements This Alignment

WALKRI operates at the field specification layer, before any applicant submits data. Its relevance to 2 CFR 200 compliance concentrates in Subpart E cost classification. WALKRI's pre-publication audit requires that every intake field specify what it measures, how that measure is operationalized, and what evidence path an independent reviewer would follow to verify the field's value. When applied to cost-related fields in a grant application, this requirement forces program operators to define what qualifies as a direct cost versus an indirect cost before applicants self-classify their budgets. This upstream specification reduces the ambiguity that produces misclassification findings.

WALKRI's evidence form requirement, which specifies that every field identify an independent access path for its evidence, also aligns with the 2 CFR 200 requirement that financial documentation be accessible to auditors. A grant application that has been structured through WALKRI's pre-publication audit will have field-level evidence paths defined in advance; this makes the Single Audit reviewer's work of tracing reported amounts to source documentation a structured task rather than an open-ended search. Taken together, CROSS's gate architecture and WALKRI's field specification discipline make the financial accountability requirements of 2 CFR 200 easier to satisfy not by adding parallel compliance machinery but by structuring the underlying documentation in a form that audit processes can directly use.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
