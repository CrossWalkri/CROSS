---
title: Sovereign Tech Fund and Sovereign Tech Agency Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - Sovereign Tech Fund program page (https://www.sovereign.tech/programs/fund)
  - Sovereign Tech Agency FAQ (https://www.sovereign.tech/faq)
  - Sovereign Tech Agency press release on the agency transition (https://www.sovereign.tech/press/release-sovereign-tech-agency)
  - Sovereign Tech Fund Evaluation Report, Pilot Phase, April 2023 (https://www.sovereign.tech/public/files/SovereignTechFund_Evaluation_Report_Pilot_Phase.pdf)
  - Interoperable Europe Portal case study on the Sovereign Tech Fund (https://interoperable-europe.ec.europa.eu/collection/open-source-observatory-osor/document/funding-open-source-case-study-sovereign-tech-fund)
  - Interoperable Europe Portal notice on the BMWK feasibility study (https://interoperable-europe.ec.europa.eu/collection/open-source-observatory-osor/news/feasibility-study-sovereign-tech-fund)
  - SPRIND project page for the Sovereign Tech Fund (https://www.sprind.org/en/actions/projects/sovereign-tech-fund)
lens_tags:
  calibration_tier: process_conformant
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: government_non_aid
  framework_scope_type: allocator_process
  # Sovereign Tech Fund (Germany) public funding for open-source digital infrastructure; government_non_aid as primary; alternative pooled_fund_or_intermediary
---

# Sovereign Tech Fund and Sovereign Tech Agency Compatibility - CROSS+WALKRI

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

This statement documents structural alignment between the Sovereign Tech Fund framework, operated by the Sovereign Tech Agency GmbH under the German Federal Ministry for Economic Affairs and Climate Action (BMWK), and the CROSS+WALKRI specification standards. The Sovereign Tech Fund publishes four formal funding criteria (prevalence, relevance, vulnerability, and public interest), a license requirement (OSI-approved or FSF Free/Libre licenses for code; Creative Commons-style licenses without non-commercial or no-derivatives clauses for documentation), and a milestone-based contracting and disbursement procedure derived from a BMWK-commissioned feasibility study. The framework is structurally a build-obligation funding architecture targeting the maintenance and hardening of widely depended-upon open digital base technologies.

The framework's compatibility with CROSS+WALKRI carries one explicit edge condition. The four published criteria are eligibility criteria, not outcome indicators: they specify which technologies and which work qualify for funding, rather than what outcome a grantee must demonstrate at completion. The framework qualifies for a compatibility statement nonetheless because (1) the criteria are published, stable, and applied across all grantees; (2) the license requirement functions as a CROSS-conformant Access Condition for the Public Benefit Mechanism primitive; and (3) the milestone-based contract architecture, scoping phase, and reporting requirements together constitute a build-obligation gate sequence that CROSS Part IV directly accommodates. The mapping below specifies which CROSS primitives carry the framework's eligibility logic and which carry its delivery and verification logic.

---

## The Sovereign Tech Fund Framework

The Sovereign Tech Fund was launched in 2022 by the German Federal Ministry for Economic Affairs and Climate Action (BMWK) following a feasibility study that documented sustained under-investment in critical open digital base technologies. The Fund was initially housed within the Federal Agency for Disruptive Innovation (SPRIND) and was institutionalised in 2024 as the Sovereign Tech Agency GmbH, an independent administrative entity established as a subsidiary of SPRIND with its own supervisory board. The Agency operates three programs: the Sovereign Tech Fund (direct grants for development and maintenance), the Sovereign Tech Fellowship (individual maintainer contracts), and the Sovereign Tech Challenge and Resilience programs (security-focused work). The framework described below applies across all three program lines.

The framework has three structural components that distinguish it from general FOSS grantmaking practice.

**Four published funding criteria.** Every funded project is assessed against four criteria, published on the Agency's website and applied across all programs. Prevalence describes how widely a technology is used by or within other technologies. Relevance describes the significance of the sectors that depend on the technology, with named examples including education, health care, energy, and industry. Vulnerability describes whether the work required to maintain or enhance the technology is structurally under-funded by other actors. Public interest describes the benefit to society or to critical sectors of society from sustaining the technology. Prevalence and relevance are assessed in tandem and together describe how critical a technology is; vulnerability and public interest are assessed alongside to determine whether public funding is the appropriate instrument. These four criteria are eligibility criteria: they govern which projects qualify, not what each project must produce.

**Open license requirement.** All code and documentation supported by the Fund must be licensed such that it is freely reusable, modifiable, and redistributable. OSI-approved licenses and FSF Free/Libre licenses are accepted for code. For documentation, Creative Commons-style licenses are accepted on the condition that they include neither a non-commercial clause nor a no-derivatives clause. The requirement applies to outputs at the time of delivery, not only at the time of application; a project that intends to release outputs under a non-conformant license, or that has not yet applied a conformant license, does not satisfy the requirement.

**Scoping, contracting, and milestone-based disbursement.** Selected applicants enter a scoping phase, of up to eight weeks, in which the Agency's program team works with the applicant to refine the scope of work, define milestones, and produce a project description. A contracting phase of up to two months follows, during which milestones, scope, and contract terms are finalised under German procurement and transparency requirements. Disbursement is tied to milestone completion: contractors submit invoices with reports against each agreed milestone, and payment follows approval. The 2023 Pilot Phase Evaluation Report documents the framework's operational record and confirms that the milestone-based contract architecture, rather than narrative grantee reporting, is the central evaluation mechanism.

The framework's published documents (the program pages, the FAQ, the application portal, and the Pilot Phase Evaluation Report) together specify what applies. The Sovereign Tech Agency does not publish an aggregate outcome measurement standard distinct from the eligibility criteria and the milestone contract architecture; this is the structural fact that distinguishes its framework from impact-measurement frameworks such as RBA or the OECD DAC criteria.

---

## How CROSS Satisfies the Sovereign Tech Fund Framework

CROSS satisfies the Sovereign Tech Fund framework at three layers: obligation mode, public benefit mechanism, and gate architecture. The mapping is direct on each layer.

**Obligation mode: Build.** The Sovereign Tech Fund finances the maintenance, hardening, and continued development of named open digital base technologies. The obligation object is the deliverable itself: the patched library, the implemented audit recommendation, the released documentation, the migrated dependency. CROSS Part III's Build obligation mode is the operative mode for this framework. The Theory of Build is the correct and complete specification for a Sovereign Tech Fund-style program; an application that names a falsifiable deliverable with independently verifiable completion criteria satisfies the CROSS entry specification gate in build mode. CROSS does not require a FROM-TO change specification in this mode, which matches the Fund's actual practice: the milestone is the obligation object, not a measured shift in a population condition.

**Public benefit mechanism: Output production. Access condition: SPDX license at the time of delivery.** The Sovereign Tech Fund framework rests its public goods claim on the existence and accessibility of the funded artifact. This is the output production mechanism type defined in CROSS Part II and in the Public Benefit Mechanism primitive (CROSS+WALKRI Primitives Foundation, Layer 3). The Fund's license requirement is structurally an Access Condition declaration in the sense defined in Part IV: an applicant must declare a specific SPDX license identifier (OSI-approved or FSF Free/Libre for code; CC-style without NC or ND for documentation) and confirm that the license applies to the output at the time of delivery. CROSS Part IV's access condition language was written precisely to accommodate this kind of requirement: it requires the SPDX identifier and the license file location, and it specifies that a future licensing commitment without a current license does not satisfy the access condition at the entry gate where the artifact already exists. Sovereign Tech Fund applicants whose codebases are already licensed conformantly satisfy the access condition at entry; applicants whose codebases are not yet licensed conformantly commit to applying the conformant license by the completion gate.

**Gate architecture: scoping phase as pre-award indicator confirmation; milestone tranches as progress verification gates; final acceptance as completion verification gate.** The Sovereign Tech Fund's scoping phase (up to eight weeks before contracting) maps onto CROSS Part IV's Pre-Award Indicator Confirmation window. During this window, the funder and the applicant refine the milestone specification, surface ambiguities before work begins, and produce a written project description that applies to subsequent gate assessments. CROSS's pre-award confirmation provision was written to do exactly this work: to surface specification problems when revision is costless rather than at the completion gate, when revision becomes a dispute. The Fund's milestone-based disbursement maps onto CROSS's Progress Verification Gates: each milestone disbursement is contingent on verification of progress against the milestone committed at the prior stage, and the minimum acceptable evidence at a progress verification gate is a publicly linkable artifact demonstrating work toward the specified deliverable, which is the operational form of a Sovereign Tech Fund invoice-with-report. Final milestone acceptance is the Completion Verification Gate, summative in character, with the named funder mechanism (the Agency's program team and contracting authority) determining whether completion criteria have been met.

**Four published criteria: a programme-level eligibility filter, not an indicator set.** The four criteria (prevalence, relevance, vulnerability, public interest) are eligibility filters operating at the round configuration level rather than the per-grantee indicator level. CROSS accommodates this in Part IV by allowing funders to publish round-level eligibility criteria as part of the gate configuration. A CROSS-conformant round operated by the Sovereign Tech Agency would publish the four criteria as round-level eligibility gates, each with an operational definition sufficient for an independent reviewer to apply. This is what the Sovereign Tech Fund's application portal already does in substance: applicants are asked to demonstrate how their proposed work scores on prevalence, relevance, vulnerability, and public interest, and the program team assesses these claims as part of the gate-pass decision. The structural alignment is direct; the four criteria are configured at the round level rather than the per-grantee indicator level, which is consistent with how CROSS Part IV treats round-level eligibility.

The following table summarises the core mappings.

| Sovereign Tech Fund Framework Element | CROSS Mechanism |
|---|---|
| Build and maintenance of named open digital base technologies | CROSS Part III Build obligation mode |
| OSI-approved or FSF Free/Libre license for code; CC-style without NC or ND for documentation | CROSS Part IV access condition declaration for output production mechanism; SPDX identifier and license file location required |
| Public goods claim based on artifact existence and accessibility | CROSS Part II output production public benefit mechanism (Public Benefit Mechanism primitive, Layer 3) |
| Eight-week scoping phase before contracting | CROSS Part IV Pre-Award Indicator Confirmation window |
| Milestone-based disbursement against invoices with reports | CROSS Part IV Progress Verification Gates with output evidence at minimum |
| Final milestone acceptance and contract close-out | CROSS Part IV Completion Verification Gate (summative); confirmation that the deliverable is publicly accessible required for build-obligation rounds |
| Four published criteria: prevalence, relevance, vulnerability, public interest | CROSS Part IV round-level eligibility configuration, published in the gate configuration before the round opens |
| Demonstrated track record of community maintenance or endorsement | CROSS Part IV Prior Work Attribution Statement; Development Stage declaration (typically Stage 3 or Stage 4 for STF-funded projects) |
| BMWK feasibility study; agency status; supervisory board | External standing context arising from BMWK origination and supervisory board oversight, anchoring CROSS Part XI funder obligations; not a per-round artifact |

---

## How WALKRI Complements This Alignment

The four Sovereign Tech Fund criteria are the central case where WALKRI's contribution is operative. Each criterion is a measurement instrument in waiting: an applicant asked "is your technology prevalent?" cannot answer without an operational definition of prevalence, a unit of measurement, and an evidence form that confirms the claim. The Fund's published definitions are conceptual statements rather than measurement specifications; applied as intake fields, they require the five-element WALKRI specification before they function as instruments rather than labels.

The prevalence criterion, applied as a WALKRI-conformant field, would require a criterion intent statement (what prevalence measures, and why), an operational definition (does prevalence count direct dependencies, transitive dependencies, downloads, deployments, or named adopters; over what time window; from what data source), a response form (numeric thresholds, dependency graph evidence, registry counts), an evidence form (the data artifact that confirms the claim, with a public source), and a conformance threshold (the minimum level above which the prevalence criterion is satisfied). Without these five elements, two applicants claiming "high prevalence" may be making non-comparable claims; with them, the criterion becomes a measurement instrument across the cohort.

The same analysis applies to vulnerability and to public interest. Vulnerability as a Fund criterion describes whether the work is structurally under-funded; as a WALKRI field, it requires the funder to specify what counts as under-funding (absolute amount, ratio of available funds to maintenance requirements, named alternative funders contacted), what evidence form satisfies the claim, and what conformance threshold applies. Public interest as a Fund criterion describes the benefit to society or to critical sectors; as a WALKRI field, it requires the funder to specify which critical sectors are within scope for the round, what evidence demonstrates downstream use within those sectors, and what conformance threshold applies. WALKRI does not change the Fund's criteria; it specifies what each criterion requires to function as a measurement instrument that produces comparable assessments across applicants.

WALKRI's bidirectional precision primitive is the load-bearing principle here. The same operational definition rigor the Sovereign Tech Fund expects of applicants describing their projects must be applied by the Fund to the criteria it uses to assess those projects. A criterion that lacks an operational definition cannot be applied consistently across applicants, regardless of how carefully the Fund's program team reviews each application; the inconsistency is in the instrument, not in the reviewer. WALKRI's contribution to the Sovereign Tech Fund framework is to turn the four criteria from conceptual frames into structured fields with the same evidential discipline the Fund already applies to its grantees' technical work.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
