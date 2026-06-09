---
title: Johns Hopkins Principles for the Use of Funds from the Opioid Litigation Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - https://opioidprinciples.jhsph.edu/
  - https://opioidprinciples.jhsph.edu/the-principles/
  - https://publichealth.jhu.edu/2021/coalition-releases-principles-to-guide-state-and-local-spending-of-forthcoming-opioid-litigation-settlement-funds
  - https://legislativeanalysis.org/principles-for-the-use-of-funds-from-the-opioid-litigation/
  - https://www.naco.org/resources/opioid-solutions/planning-principles-toolkit
lens_tags:
  calibration_tier: outcome_specified_self_reported
  authority_source: civil_society_advisory
  cultural_methodological_lineage: western_institutional
  funder_typology: settlement_administered
  framework_scope_type: allocator_process
  # Johns Hopkins Principles for the Use of Funds from the Opioid Litigation; settlement_administered funder typology
---

# Johns Hopkins Principles for the Use of Funds from the Opioid Litigation

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Johns Hopkins Bloomberg School of Public Health "Principles for the Use of Funds from the Opioid Litigation" (released December 2021) is a published five-principle framework that specifies allocation principles for state and local governments spending opioid settlement and abatement funds. The framework is advisory and academic-authored: it carries no enforcement authority over fund recipients and is endorsed by more than 60 organizations. More than 25 states use the Principles to inform their spending decisions, and county-level adoption is documented through the National Association of Counties planning toolkit.

This compatibility statement maps the five Hopkins Principles to CROSS gate architecture and primitive structure, and documents the conditions under which a CROSS+WALKRI-conformant abatement grants program structurally satisfies the Principles.

A note on the consistency basis for Part XII inclusion. The Hopkins Principles differ from the NCRP "Criteria for Philanthropy at Its Best" in their authorship structure: NCRP was authored by a civil society coalition of more than eighty organizations explicitly representing the recipient side of the philanthropic relationship, including parties whose cost-bearing relation to the system is most direct, while the Hopkins Principles were authored by academic public health experts at a single institution and subsequently endorsed by a coalition of organizations and adopted as voluntary reference guidance by state attorneys general, abatement trust boards, and counties. Both nonetheless qualify for Part XII coverage on the same structural basis: each is a widely-adopted, publicly-available sector-reference framework that specifies allocation principles for the use of public or philanthropic funds, neither carries enforcement authority over downstream grantees, and both function as the de facto rubric against which fund allocators in their respective sectors are publicly legible to grantees, recipients, and cost-bearing parties. The basis for Part XII coverage is whether a framework specifies allocation principles that funders adopt as their stated standard, not whether the framework was authored by recipients, coalitions, or academic experts.

---

## The Hopkins Principles Framework

The five Principles are:

**Principle 1: Spend the money to save lives.** Settlement funds should be directed to interventions that reduce overdose deaths and other opioid-related harms in the affected population. The principle distinguishes between spending that demonstrably reduces mortality (such as evidence-based medication for opioid use disorder, naloxone distribution, and harm reduction services) and spending that does not directly address the mortality crisis. The implicit critique is of allocation decisions that route settlement funds to general budget purposes, law enforcement infrastructure, or interventions without measurable harm-reduction effect.

**Principle 2: Use evidence to guide spending.** Allocation decisions should be informed by the existing evidence base on which interventions reduce opioid-related harm. Programs with established efficacy (medication for opioid use disorder, syringe services programs, contingency management) should be prioritized over programs without an evidence base. The principle requires that funders be able to state the evidence basis for each funded intervention.

**Principle 3: Invest in youth prevention.** A defined share of settlement funds should support primary prevention interventions targeting young people, on the basis that preventing initiation produces larger long-term population-level reductions in opioid use disorder than treatment alone. The principle implies a portfolio composition requirement: across the full allocation, youth prevention must be visible as a category and not displaced entirely by acute treatment and crisis response.

**Principle 4: Focus on racial equity.** Allocation decisions must address the documented racial disparities in opioid-related mortality, in access to treatment, and in the historical criminalization of substance use in Black, Latino, Indigenous, and other communities of color. The principle requires that allocation decisions be examined for whether they reduce or reproduce disparities, and that funding reach communities of color in proportion to need rather than in proportion to political access. The principle frames racial equity as a structural condition on allocation, not as an optional secondary objective.

**Principle 5: Develop a fair and transparent process for deciding where to spend the funding.** Allocation decisions should be made through a publicly documented process with disclosed decision-makers, published criteria, public input mechanisms, and ongoing reporting on how funds were actually spent. The principle treats process legibility as foundational: even allocations that satisfy Principles 1 through 4 in substance fail the Principles overall if the decision process is opaque, lacks a named decision authority, or excludes affected communities from input.

The five Principles operate at the portfolio level of an allocation authority (a state opioid settlement trust, a county abatement board, a state attorney general's office, or an equivalent body). They are not designed to be applied to individual grants in isolation; compliance requires examining the distribution of funding decisions across the full allocation and the process by which those decisions were made.

---

## How CROSS Satisfies the Hopkins Principles

CROSS provides the structural mechanisms by which an allocation authority can demonstrate conformance to the Hopkins Principles as a published, verifiable property of its program rather than as a reputational claim. The mapping below identifies the CROSS primitive and provision corresponding to each Principle.

**Principle 1 (spend the money to save lives) maps to CROSS's Public Benefit Mechanism declaration and the condition change obligation mode.** An allocation authority operating under Hopkins Principle 1 is making a condition change claim: settlement funds will produce a measurable change in opioid-related mortality and morbidity in a defined population. CROSS Part II's Public Benefit Mechanism declaration requires that the applying funder specify which of the four mechanism types its public benefit claim rests on (output production, access provision, condition change, or ecosystem shift) and what access conditions hold. For Principle 1 conformance, the condition change mechanism is the correct declaration, and the access conditions must include the FROM state (current overdose mortality rate in the named population) and a measurable TO state target. The Theory of Build is a failure mode in this context: an abatement grant whose justification describes only what will be built or delivered, without naming the mortality or morbidity condition it addresses in the defined population, does not satisfy Principle 1 even if the deliverables are completed.

**Principle 2 (use evidence to guide spending) maps to CROSS's Evidence Strength taxonomy and the eleven-field indicator specification in Part V.** CROSS requires that every indicator specification declare the evidence basis on which the intervention is expected to produce its claimed outcome, including Field 2 (rationale for indicator) and the evidence form specification at the completion gate. An allocation authority operating under Principle 2 must be able to state, for each funded intervention, what evidence base supports the claim that the intervention produces the claimed outcome. CROSS's Evidence Strength taxonomy (self-report, independent review, independent verification, counterfactual methodology) provides the formal vocabulary for distinguishing interventions with strong evidence backing from those without. The conformance threshold field in WALKRI Section 6.2 provides the mechanism for citing the specific evidence source (a Cochrane review, a National Academies consensus study, a CDC guideline, or equivalent) that justifies inclusion of the intervention in the funded portfolio.

**Principle 3 (invest in youth prevention) maps to CROSS's Population Scope declaration with disaggregation requirements and the Portfolio Position primitive.** Principle 3 is a portfolio composition requirement, not a per-grant requirement. CROSS's Portfolio Position primitive (Layer 7) and the Cohort Position assessment in Part IV together provide the mechanism for declaring, at the round and program level, what share of the portfolio addresses each declared population scope. An allocation authority operating under Principle 3 declares youth as a population scope in its round specification, declares a minimum allocation share to youth-prevention interventions, and demonstrates at portfolio analysis that the declared share was achieved. The disaggregation ratchet provision in Part V ensures that age-disaggregated indicator data, once collected, cannot be discontinued in subsequent rounds, preventing the failure mode in which youth-prevention tracking begins with apparent rigor and is quietly dropped when crisis-response demands consume the visible portfolio.

**Principle 4 (focus on racial equity) maps to CROSS's Population Scope declaration with race and ethnicity disaggregation, the disaggregation ratchet, and the Cohort Position assessment.** This is the strongest structural mapping in the framework. Principle 4 requires that allocation decisions be examined for racial disparities in funding flow and outcomes. CROSS's Cohort Position assessment requires, before final gate determinations are made in any round, an analysis of how applicants and beneficiaries are distributed across population categories defined in the round specification. The disaggregation ratchet provision means race and ethnicity categories declared in a round cannot be dropped in subsequent rounds. Together these provisions produce the longitudinal disaggregated allocation data that a Principle 4 analysis requires. CROSS's Causality Stance field (Layer 4) further supports Principle 4 by allowing programs to declare contribution rather than attribution for outcomes in populations where racial disparities reflect multiple structural causes that no single program controls; this is the structural acknowledgment that Principle 4's framing of racial equity as a structural condition implies.

**Principle 5 (develop a fair and transparent process) maps to CROSS Part IV's pre-round publication requirements, Part XI's funder obligations and redress mechanisms, and Part IX-A's interoperability and attestation requirements.** Principle 5 is the strongest match in the framework to CROSS's funder-side obligations. Part IV requires that the funder publish, before any round opens: the plain-language applicant-facing summary of the round's requirements; the full application question list with criterion intent visible for each question; the gate configuration specifying evidence scope and evidence strength at each gate; and the named, published mechanism by which gate determinations will be made. Part XI specifies funder obligations and redress rights for grantees, including the requirement that gate determinations be documented and that funders have a named authority to whom redress requests can be submitted. Part IX-A specifies that gate determinations are expressible as cryptographically attributed, publicly verifiable records, which is the format-agnostic structural equivalent of Principle 5's transparency requirement. An allocation authority operating under Principle 5 can satisfy the principle through any infrastructure (signed institutional documents, on-chain attestations, published reports) that meets the content requirements CROSS specifies.

| Hopkins Principle | CROSS Primitive / Provision |
|---|---|
| 1. Spend the money to save lives | Public Benefit Mechanism declaration (condition change type); change obligation mode; FROM-TO state specification |
| 2. Use evidence to guide spending | Indicator specification Field 2 (rationale); Evidence Strength taxonomy; WALKRI conformance threshold |
| 3. Invest in youth prevention | Population Scope declaration; Portfolio Position primitive; Cohort Position assessment; disaggregation ratchet |
| 4. Focus on racial equity | Population Scope with race and ethnicity disaggregation; disaggregation ratchet; Cohort Position assessment; Causality Stance (contribution) |
| 5. Fair and transparent process | Pre-round publication requirements (Part IV); funder obligations and redress (Part XI); attestation interoperability (Part IX-A) |

---

## How WALKRI Complements This Alignment

WALKRI's pre-publication audit ensures that the intake fields collecting the data each Hopkins Principle depends on are measurement instruments rather than labeling exercises. A field that asks an applicant whether their proposed program is "evidence-based" without specifying what evidence threshold qualifies, what evidence types are accepted, or what conformance threshold applies under Principle 2 produces data that cannot support a portfolio-level evidence review. WALKRI requires that the criterion intent, operational definition, response form, evidence form, and conformance threshold be specified for every field before the field is presented to applicants. For Principle 2 specifically, this means the conformance threshold field must cite which evidence sources are accepted as qualifying (Cochrane reviews, USPSTF recommendations, SAMHSA evidence-based practice registries, or equivalent) and what minimum evidence rating qualifies an intervention as Principle 2 conformant.

For Principle 4, WALKRI ensures that the race and ethnicity categories built into intake forms have operational definitions specifying which categories are collected, how applicants will self-identify, and what counts as evidence of serving a named community of color. Without these specifications, the disaggregated data produced by intake cannot support the kind of allocation-disparity analysis that Principle 4 requires. WALKRI's bidirectional precision principle applies: an allocation authority cannot ask applicants for the disaggregated data that Principle 4 requires without itself meeting the precision standard for the fields collecting that data.

For Principle 5, WALKRI ensures that the publication of the application question list (required by CROSS Part IV before any round opens) is a substantive transparency commitment rather than a procedural formality. The published question list must show every question the applicant will encounter, in the order they will encounter it, with the criterion intent visible alongside each question label. This is the operational form of Principle 5's transparency requirement applied to the intake stage.

---

## Conditions for Conformance

A CROSS+WALKRI-conformant abatement grants program does not automatically satisfy the Hopkins Principles. The conformance relationship is conditional on five program design decisions that the allocation authority must make explicitly:

The condition change obligation mode must be declared at the program level for any portfolio claiming Principle 1 conformance. Programs operating exclusively in build obligation mode (funding deliverables without a population-level mortality or morbidity outcome claim) cannot claim Principle 1 conformance even if their deliverables are completed.

The Evidence Strength taxonomy must be configured with a published evidence floor at the round level. A program that accepts self-report evidence as the completion gate standard does not satisfy Principle 2 regardless of CROSS conformance, because Principle 2 requires that evidence inform allocation decisions, not merely report on them.

Youth must be declared as a population scope with a minimum allocation share specified in the program-level Theory of Change declaration (CROSS Part IX-B). Without this declaration, the portfolio composition requirement of Principle 3 cannot be assessed.

Race and ethnicity disaggregation must be declared as a required field in the intake and reporting forms, and the disaggregation ratchet must be activated. A program that collects race and ethnicity data at the applicant's discretion does not produce the longitudinal allocation data Principle 4 requires.

The pre-round publication requirements of Part IV must be satisfied in full: the plain-language summary, the full application question list, the gate configuration, and the named gate determination authority must all be publicly accessible before any round opens. Programs that publish some but not all of these elements do not satisfy Principle 5 regardless of other conformance.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
