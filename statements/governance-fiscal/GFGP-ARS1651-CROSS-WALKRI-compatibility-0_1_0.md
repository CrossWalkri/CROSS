---
title: Good Financial Grant Practice (GFGP / ARS 1651) Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.4 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - https://www.globalgrantcommunity.com/standard
  - https://health-policy-systems.biomedcentral.com/articles/10.1186/s12961-025-01343-7
lens_tags:
  calibration_tier: independently_verified
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: multilateral_bank_or_fund
  framework_scope_type: certification
  # Good Financial Grant Practice (ARS 1651 African Regional Standard); certification scheme administered through African Organisation for Standardisation; primary funder typology multilateral; alternative bilateral_aid_agency
---

# Good Financial Grant Practice (GFGP / ARS 1651)

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

GFGP (ARS 1651), published by the African Organisation for Standardisation and managed by the Global Grant Community, is the only internationally recognized formal standard governing the grant management capacity of recipient organizations. CROSS+WALKRI and GFGP operate at different architectural layers: GFGP assesses organizational readiness to manage grants, while CROSS+WALKRI specifies the measurement architecture for what funded programs must demonstrate. The two standards are complementary and together address the full verification chain from organizational systems quality through program evidence quality.

---

## The Standard's Approach

GFGP was published by the African Organisation for Standardisation (ARSO) in June 2018. It covers more than 300 requirements across four practice areas: financial management, human resources management, procurement management, and governance. Compliance is tiered across Bronze (70 clauses), Silver, Gold, and Platinum (300 clauses), allowing organizations to achieve and demonstrate progressive capacity development rather than a single pass/fail threshold.

The standard has significant institutional backing, including UKAID, the Wellcome Trust, UKRI, EDCTP, and the African Union. It has been submitted for consideration as an ISO standard and is increasingly required as a grant eligibility condition for African civil society organizations and research institutions. A 2025 peer-reviewed implementation study published in Health Policy and Systems documents real-world uptake patterns across health-sector organizations, confirming that the standard is operating as a live eligibility filter rather than a theoretical aspirational framework.

GFGP is a supply-side standard. It assesses the organizational readiness and systems of the grantee before and during the grant relationship. It does not prescribe how programs should measure their outputs or demonstrate impact; it assesses whether the organization managing those programs has the financial, governance, procurement, and personnel systems to do so responsibly. This distinction is architecturally important: a GFGP-certified organization has demonstrated that its organizational infrastructure meets a defined standard, but GFGP certification says nothing about whether the programs it runs produce verifiable evidence of what they claimed to achieve. That gap is precisely what CROSS+WALKRI addresses.

The four GFGP practice areas reflect this organizational focus. Financial management covers budgeting, accounting, cash flow management, financial reporting, and audit readiness. Governance covers board structure, conflict of interest policies, strategic planning, and organizational compliance. Human resources management covers personnel policies, job descriptions, performance management, and named personnel accountability. Procurement management covers purchasing policies, vendor selection, contract management, and documentation of procurement decisions. Each of these areas has corresponding requirements that must be evidenced for certification at each tier.

---

## How CROSS Satisfies the GFGP Framework

CROSS and GFGP do not map in a one-to-one provision-to-provision relationship, because they address different objects. GFGP addresses the organization; CROSS addresses the program run by that organization. However, several CROSS provisions directly produce documentation that satisfies GFGP evidence requirements, and the table below captures those alignments.

| GFGP Practice Area | CROSS Provision |
|---|---|
| Governance: board independence, legal status, jurisdiction, registration, disbursement authority | CROSS organizational identity fields (legal name, jurisdiction, registration, governance structure, disbursement authority) |
| Governance: conflict of interest management | CROSS conflict of interest provisions (Part VII): board independence declaration, conflict management policy requirements |
| Financial management: audit trail and record retention | CROSS completion gate evidence documentation + Attestation Corpus, retained indefinitely in verifiable form |
| Financial management: budget management documentation and concurrent funding transparency | CROSS concurrent funding disclosure, documenting all active funding relationships for a given program |
| Human resources management: personnel governance and named personnel accountability | CROSS organizational identity declaration, including named personnel fields for named responsible individuals |
| Procurement management: purchase documentation trail | CROSS Attestation Corpus, which retains evidence submitted at each gate and is independently verifiable |

Three of these alignments warrant fuller explanation.

The governance alignment is the tightest. GFGP Platinum tier requires extensive evidence of governance quality: board meeting records, conflict of interest declarations, organizational registration documents, and evidence that disbursement authority is clearly defined and exercised by appropriately authorized individuals. CROSS organizational identity fields collect exactly this data in structured form at entry, and CROSS Part VII conflict of interest provisions require documented conflict management as a condition of gate passage. An organization that has completed CROSS entry and passed Part VII review has produced, in structured and independently verifiable form, most of the decision-standing documentation GFGP requires.

The financial management alignment centers on audit trail quality. GFGP financial management requirements emphasize that financial records must be complete, accurate, and independently verifiable. CROSS's Attestation Corpus, by retaining a timestamped record of every claim and every piece of evidence submitted at each gate, with independent attestation at each completion gate, provides exactly the audit trail structure that GFGP financial management auditors look for. The CROSS record is program-level rather than organizational-level, but it provides the program-specific financial documentation that a GFGP auditor would then integrate with the organizational financial records.

The procurement documentation alignment is partial and complementary. GFGP governs organizational procurement comprehensively; CROSS does not prescribe procurement management. What CROSS does provide is a gate-level evidence record that includes any procurement-related documentation submitted as evidence of program activities, which means that procurement decisions relevant to program delivery appear in the Attestation Corpus even though CROSS does not govern procurement policy directly.

---

## How WALKRI Complements This Alignment

WALKRI's pre-publication audit requirement, which specifies that every intake field must define what it measures, how it measures it, and what evidence path an independent reviewer would follow, has a specific relationship to GFGP's financial documentation independence requirement. GFGP requires that financial records be independently verifiable, meaning that an auditor who did not participate in generating the record can trace it to source documentation without relying on the organization's own explanations. WALKRI's evidence form requirement imposes an equivalent discipline at the field level: every field in an intake instrument must specify an independent access path for its evidence before any applicant sees the form. An organization applying through a WALKRI-structured instrument submits data whose evidentiary basis has already been defined independently of the applicant, which is the field-level expression of the same independence principle that GFGP's financial documentation requirements embody.

More broadly, GFGP certification represents a claim about organizational systems quality. WALKRI represents a claim about measurement instrument quality. An organization with GFGP certification operating programs assessed through WALKRI-structured instruments provides funders with two independent quality signals at different levels of the verification chain: the organizational systems are sound and the measurement instruments are specified to professional standards. Neither signal substitutes for the other; together they address the two most common failure modes in grant-funded programs, which are poor organizational financial controls and poorly specified program measurement. The combination of GFGP certification with CROSS+WALKRI conformance represents the most complete verification architecture currently available for grant-funded programs operating in the African civil society and research institution context where GFGP is most widely deployed.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
