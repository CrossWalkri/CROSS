---
title: Candid Seals of Transparency Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - https://candid.org/claim-nonprofit-profile/how-to-earn-a-candid-seal-of-transparency/
  - https://candid.org/blogs/candid-2026-seals-of-transparency-made-faster-easier-nonprofits-more-donations/
  - https://developer.candid.org/docs/guidestar-seal-as-eligibility-requirement
  - https://help.candid.org/s/article/How-to-Earn-a-Platinum-Seal-of-Transparency
  - https://cdn.candid.org/seals-of-transparency/2026/candid-seals-guide-2026.pdf
lens_tags:
  calibration_tier: process_conformant
  authority_source: civil_society_advisory
  cultural_methodological_lineage: western_institutional
  funder_typology: pooled_fund_or_intermediary
  framework_scope_type: certification
  # Candid (formerly GuideStar) Seals of Transparency; civil_society_advisory authority; certification scope; primary funder typology pooled_fund_or_intermediary as proxy for organizations seeking certification
---

# Candid Seals of Transparency

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Candid Seals of Transparency (candid.org), administered by Candid (the 501(c)(3) nonprofit formed in 2019 from the merger of GuideStar and the Foundation Center), are the primary voluntary self-disclosure framework for US-registered nonprofit organizations. Four tiers (Bronze, Silver, Gold, Platinum) signal progressively richer disclosure of identity, programs, finances, governance demographics, and outcome metrics on a Candid profile, with IRS Form 990 data serving as the foundational financial source. Adoption is substantial: a Candid profile is a de facto eligibility requirement for many US foundation grant applications, and Candid's Premier API exposes seal status as a structured field that grantmakers query during intake. CROSS+WALKRI produces the evidentiary infrastructure that conformant disclosure against the Gold and Platinum tiers requires, and the CROSS Attestation Corpus provides the persistent, publicly accessible record that organization-driven self-disclosure frameworks of this kind depend on for verifiability against current evidence.

The Candid Seals are structurally distinct from Charity Navigator and similar third-party rating systems. Charity Navigator scores nonprofits according to a methodology it controls, producing a market-facing assessment signal that the rated organization does not author. Candid Seals are organization-driven: the nonprofit completes its own profile and selects the disclosure depth, and the seal recognizes the disclosure rather than rating the organization's quality. The framework is therefore parallel to the Accountable Now Global Standard for CSO Accountability covered in Part XII (member-organization-driven, voluntary, tiered or composite, with an administering nonprofit running the disclosure architecture) and not parallel to Charity Navigator (third-party rating).

---

## The Candid Seals of Transparency

Candid administers a single canonical profile for every US tax-exempt organization, populated initially from IRS Business Master File data and IRS Form 990 filings. The Seals are layered onto this profile substrate. A nonprofit earns a seal by adding successively richer categories of information to its profile; each tier corresponds to a specific disclosure scope.

The **Bronze Seal** requires the basic identity disclosures donors and funders need to find and contact the organization: organization name, mission statement, subject area, population served, geographic area served, and contact information. This tier establishes that the entity is locatable and self-describes its scope of work.

The **Silver Seal** requires program-level disclosure: for each program the organization runs, a name, description, geographic area served, subject area, and population served. The Silver tier moves the disclosure from "who we are" to "what we do," at a granularity sufficient for a potential funder to assess scope alignment.

The **Gold Seal** requires Bronze and Silver plus additional disclosure of financial data, leadership information, and board demographics. The financial disclosure draws on IRS Form 990 data and may be supplemented by audited financial statements. The leadership and demographic disclosure addresses governance composition. The Gold tier is the first that supports the standard funder due diligence question set (programs, finances, governance) at a defensible level of detail.

The **Platinum Seal** requires Bronze, Silver, and Gold plus the publication of at least one impact metric from the most recent year and the public sharing of board demographic information. Platinum tier organizations specify, for each metric, a description of what is measured, the value, the direction in which success would move the metric (increase, decrease, or stay the same), and the relevant time period. Most published metrics are outputs (a reported 64 percent in Candid's own analysis); a smaller fraction are outcomes (approximately 18 percent). Fewer than one percent of US-registered nonprofits hold the Platinum Seal.

Control of the framework rests with Candid as a 501(c)(3) under a board of trustees inherited from the merging organizations. Candid is funded by major US foundations (the merger and platform development were supported by approximately twenty-seven million USD from the Gates, Mott, and Hewlett foundations) and operates as the central self-disclosure utility for the US nonprofit sector. The framework is voluntary in the sense that no nonprofit is legally required to earn a seal; it is de facto required in the sense that an absent or low-tier Candid profile reduces a funder's ability to verify the applicant against the named disclosure conditions, and many grantmaking programs expose the seal status as a screening field through Candid's developer API.

For cohort 1 of the grants ecosystem (civil society organizations as grant recipients), claiming and tiering up a Candid profile is one of the standard structural disclosure moves available to a nonprofit applicant for raising a funder's verification confidence. For cohort 3 (program operators managing grantee programs), the seal status is a structured signal that can be queried, recorded, and referenced in eligibility logic without re-collecting the underlying data.

---

## How CROSS Satisfies the Candid Disclosure Architecture

CROSS provides the structured record from which Gold and Platinum tier disclosures can be drawn without reconstruction, and the Attestation Corpus provides the persistent backing for the public-facing seal that distinguishes a current, evidenced disclosure from a stale claim. The Attestation Corpus, as used in this statement, names a persistent, queryable record of declarations and gate determinations under named legibility conditions: each entry specifies who declared what, when, under which gate configuration, and what evidence accompanied the declaration.

The Bronze tier disclosures map directly to fields in the CROSS organizational identity declaration. The legal entity name, jurisdiction, parent organization disclosure, affiliated entity disclosure, and disbursement authority fields (CROSS Part IV) cover the identity scope a Bronze profile requires. A CROSS-conformant applicant submission contains the data a Bronze profile needs as a structured byproduct rather than as a parallel data collection task.

The Silver tier disclosures (program-level scope) map to the CROSS scope declaration and population scope declaration. The Silver tier asks an organization to describe each program by subject area, population, and geography. CROSS Part IV requires applicants to declare the scope their application covers, the population affected, and the problem area being addressed. An organization operating multiple programs under CROSS will have these declarations on record per program and can publish them as Silver tier disclosures.

The Gold tier disclosures (finances, leadership, governance demographics) map to a combination of CROSS organizational identity fields and the disbursement authority declaration. The disbursement authority field distinguishes individual, collective, and delegated authority states, requiring named persons or named authority-conferring mechanisms; this is the structural information a Gold tier disclosure of board composition rests on. CROSS Part VII conflict of interest provisions provide the surrounding coordination instrument elements (named board standing, named removal mechanism, conflict of interest tier classification) that Gold-level disclosure on named board standing and removal mechanism references. IRS Form 990 financial data is exogenous to CROSS but is referenced by both frameworks as authoritative for US-registered entities.

The Platinum tier disclosures (impact metrics) are the closest tier to grantee MEL in the conventional sense and where CROSS and WALKRI contribute the most substantive infrastructure. Platinum tier metrics ask the organization to specify what is measured, the value, the intended direction of change, and the time period. CROSS-conformant programs operating in change-obligation or build-with-usage-evidence mode already specify these elements at the entry gate (the indicator, the population, the FROM-TO state, the time period) and verify them at the completion gate. The completion gate determination, recorded in the Attestation Corpus, is precisely the evidenced metric an organization would publish as a Platinum tier disclosure. Without this infrastructure, Platinum tier metrics are typically self-reported numbers without an evidence path; with this infrastructure, each published metric traces back to a gate determination an independent reviewer could examine.

| Candid Tier Disclosure | CROSS Provision |
|---|---|
| Bronze (identity, mission, subject area, geography, contact) | Organizational identity declaration (Part IV): legal entity name, jurisdiction, affiliated entity disclosure, parent organization disclosure |
| Silver (per-program scope, subject, population, geography) | Scope declaration and population scope declaration (Part IV); coherence disclosure |
| Gold (finances, leadership, governance demographics) | Disbursement authority declaration (Part IV); conflict of interest provisions (Part VII); organizational identity fields cross-referenced with IRS Form 990 data |
| Platinum (impact metrics with direction and time period) | Entry gate indicator specification and completion gate determination, recorded in the Attestation Corpus |
| All tiers (persistent, publicly accessible disclosure record) | Attestation Corpus: persistent, queryable record of organizational declarations and gate determinations |

The Attestation Corpus mapping deserves expansion. A Candid Seal is renewed annually, and the verifiability of any seal depends on whether the underlying disclosures remain accurate against current evidence. An organization whose Platinum tier metrics were published two years ago without subsequent verification carries a weaker signal than one whose metrics trace to recent, independently reviewed gate determinations. CROSS's Attestation Corpus provides the substrate for time-stamped, queryable disclosure with documented evidence: the seal becomes a pointer to verifiable history rather than a static disclosure that rests on undocumented confidence rather than on a verifiable record.

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication field requirements (operational definition, unit and scale, baseline reference, evidence access path, population scope) address the most common weakness of voluntary self-disclosure frameworks: metrics that are technically published but operationally ambiguous. A Platinum tier metric labeled "people served" with no operational definition, no unit specification, no defined population, and no evidence path is published data; it is not measurement-grade data.

A WALKRI-conformant program defines each metric's operational definition, units, baseline, evidence access path, and population scope before any data is collected. When an organization operating a CROSS+WALKRI conformant grant program then populates its Platinum tier disclosures, each metric carries the specification needed for an independent reader to interpret it consistently. The metric is no longer an isolated number on a public profile; it is a published value backed by a documented measurement instrument.

This complementarity matters specifically for the funder side of the Candid relationship. When a foundation queries Candid's API for seal status as an eligibility check, it learns whether the applicant holds a current seal at a given tier. The seal tier signals disclosure depth; it does not signal disclosure quality. A funder configuring its grant program around CROSS+WALKRI raises the quality floor on the disclosures that subsequently feed seal claims: any applicant funded under such a program produces, through normal participation in the gate architecture, the operationally precise outcome data that a Platinum tier disclosure should rest on. The seal continues to serve its role as a public disclosure signal, and the disclosures behind it become more substantively reliable.

The ethical-disclosure concern that motivates Candid's framework (publicly displayed transparency claims should reflect verifiable underlying practice) is the same concern that WALKRI's evidence form requirement addresses at the field level. A program whose intake forms separate independently verifiable evidence from affected-population self-report, and whose completion gate documents the resulting determinations, produces disclosures that meet the implicit accuracy standard of the Seals framework rather than only its formal disclosure depth.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
