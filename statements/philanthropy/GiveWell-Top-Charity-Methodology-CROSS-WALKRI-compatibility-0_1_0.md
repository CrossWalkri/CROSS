---
title: GiveWell Top Charity Methodology Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - https://www.givewell.org/
  - https://www.givewell.org/charities/top-charities
  - https://www.givewell.org/how-we-work/criteria
  - https://www.givewell.org/research/intervention-reports
  - https://www.givewell.org/how-we-work/our-criteria/cost-effectiveness
  - https://www.givewell.org/research/change-our-mind-contest
  - https://www.givewell.org/all-grants-fund
lens_tags:
  calibration_tier: independently_verified
  authority_source: civil_society_advisory
  cultural_methodological_lineage: western_institutional
  funder_typology: private_foundation
  framework_scope_type: third_party_rating
  # GiveWell Top Charity Methodology; third_party_rating scope; primary funder typology private_foundation captures GiveWell-recommended grantee donors though rater typology is itself intermediary
---

# GiveWell Top Charity Methodology Compatibility - CROSS+WALKRI

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

GiveWell publishes an extensive, openly accessible methodology at givewell.org governing how charities are evaluated for inclusion in its Top Charities list and how grants are made through the All Grants Fund. The methodology is framed as a donor-facing selection tool: GiveWell tells individual donors and institutional partners which organizations it believes will achieve the most good per marginal dollar. The published architecture includes four named top-charity criteria (cost-effectiveness, evidence of impact, room for more funding, and transparency), intervention reports synthesizing the evidence base for each program type GiveWell funds, charity-level reviews with full reasoning visible, public cost-effectiveness analysis spreadsheets with assumptions documented and reproducible, and change logs that record when and why GiveWell's recommendations have moved.

The donor-facing framing produces an analytical ambiguity that this statement resolves explicitly. GiveWell does not formally contract grantees to produce reports of a specified form, and its public-facing language describes a recommendation process rather than a grantee MEL standard. However, the documentation that must exist for a charity to be evaluated, recommended, and re-recommended is substantial and recurring: an organization seeking top-charity status or All Grants Fund support must produce intervention-level evidence of effect, must supply or enable GiveWell to construct cost-effectiveness derivations using verifiable cost and output data, must maintain program documentation at the rigor GiveWell's analysts require for review, and must respond to GiveWell's ongoing requests for updated data as recommendations are revisited each year. That functions as a grantee-facing standard, even if administered through a donor-recommendation mechanism rather than a contractual MEL requirement. This statement makes that argument explicit and treats GiveWell's published methodology as a grantee-facing standard in the relevant sense.

GiveWell sits in the impact-investing-adjacent space already covered in CROSS+WALKRI Part XII by IRIS+ (Global Impact Investing Network metadata requirements), the IFC Operating Principles for Impact Management (institutional impact-investor accountability cycle), the Impact Management Norms / IMP Five Dimensions (What, Who, How Much, Contribution, Risk decomposition), and the IDB Invest DELTA Impact Rating System (ex-ante impact rating in development finance). GiveWell's methodology is distinct from these four in that it is selection-and-monitoring rather than rating-or-disclosure, but its substantive content (cost-effectiveness modeling, evidence-of-effect hierarchies, contribution and counterfactual reasoning, and ongoing room-for-more-funding analysis) maps onto the same primitives CROSS+WALKRI already covers in those statements.

GiveWell is a separate entity from EA Funds, Open Philanthropy, and Founders Pledge. Open Philanthropy was originally spun out of a GiveWell research project but has operated as an independent organization since 2017; its grantmaking architecture is not addressed in this statement. EA Funds is a separate grantmaking platform operated by Effective Ventures with its own per-fund methodologies. This statement covers only GiveWell's published Top Charity criteria, intervention-report architecture, cost-effectiveness analysis methodology, and the All Grants Fund insofar as it operates under the same evidentiary standards.

---

## The Donor-Facing vs Grantee-Facing Tension

GiveWell's self-presentation positions it as a donor-decision-support organization. Its public materials describe how donors should choose where to give, how GiveWell's analysts reason about marginal cost-effectiveness, and why specific charities have been moved on or off the Top Charities list. Grantees do not sign a Letter of Agreement specifying CROSS-style indicators, completion gates, or evidence thresholds, and GiveWell does not publish a "GiveWell Grantee Reporting Framework" document by that name.

The structural argument for treating the methodology as a grantee-facing standard, despite the donor-facing framing, has four components.

First, top-charity status is conditional and recurring, not awarded once. GiveWell re-evaluates each top charity annually and may add or remove charities based on updated evidence. To remain on the list, an organization must continue to produce the underlying data that GiveWell's intervention reports and cost-effectiveness models depend on. The documentation requirement is recurring because the recommendation is recurring.

Second, the published intervention reports specify, in operational detail, what counts as evidence of effect for each program type GiveWell funds. An organization claiming to deliver bednets, vitamin A supplementation, deworming, malaria chemoprevention, or any other GiveWell-recommended intervention faces a published evidence hierarchy that defines what randomized controlled trials, observational studies, and operational data are considered relevant. This is functionally a sector evidence standard: a charity that wants to be evaluated for the deworming intervention category must produce evidence that fits the deworming intervention report's evidence framework. The intervention reports are not contractual obligations, but they are public, durable, version-tracked specifications of what evidence will be looked for.

Third, the cost-effectiveness analysis spreadsheets are publicly accessible with their assumptions documented. A charity that wishes to remain in the model must continue to supply or enable the construction of inputs at the granularity the spreadsheet requires: per-unit delivery cost, coverage rates, wastage assumptions, mortality or morbidity reductions per unit delivered, and counterfactual displacement adjustments. The cost-effectiveness analysis is the primary instrument by which top-charity status is contested and confirmed; producing data of the form the analysis requires is the operational condition of remaining recommended.

Fourth, the All Grants Fund operates explicitly as a grantmaking vehicle, not only a donor-recommendation channel. Grantees of the All Grants Fund receive funds directly from GiveWell, with grant agreements and conditions that incorporate the same evidence and cost-effectiveness expectations applied to top charities. For the All Grants Fund portfolio, the donor-facing framing collapses entirely: the recipient is a grantee in the conventional sense, and the published methodology functions directly as a grantee-facing evaluation framework.

These four components, taken together, support the analytical move this statement makes: GiveWell's published methodology functions as a grantee-facing standard in the operational sense, even where the formal instruments are donor-facing. The remainder of the statement treats it as such.

---

## The Published Architecture

GiveWell's methodology has several named components, each publicly accessible at givewell.org.

The **four top-charity criteria** are stated explicitly: evidence of impact (the program type the charity delivers has credible evidence supporting effect, with the strongest evidence concentrated in randomized controlled trials and meta-analytic syntheses of those trials), cost-effectiveness (the marginal dollar delivered through this charity produces verifiable benefit at a level competitive with GiveWell's reference threshold, currently calibrated against multiples of an established benchmark), room for more funding (the charity has the operational and absorptive capacity to deploy additional funds at the marginal cost-effectiveness rate without diminishing returns at the margin), and transparency (the charity discloses what it does, how it spends, what evidence supports its programs, and what its operational data show, at a level sufficient for independent verification).

The **intervention reports** are program-type-specific syntheses of the evidence base GiveWell uses to assess any charity delivering that program type. Each report names the intervention, summarizes the underlying randomized controlled trial and observational evidence, calibrates effect-size assumptions, documents heterogeneity considerations across settings, and provides the evidence input layer for the cost-effectiveness model. Intervention reports are version-tracked, and changes to the underlying evidence base trigger documented revisions.

The **cost-effectiveness analysis spreadsheets** are publicly accessible and reproducible. Each top-charity-eligible intervention has a corresponding spreadsheet specifying delivery costs (sourced from charity financial reporting and operational data), coverage and wastage assumptions, effect-size assumptions (sourced from the intervention report), counterfactual displacement adjustments (how much of the funded activity would have occurred without GiveWell-directed funding), and a final cost-effectiveness estimate expressed in units comparable across interventions. The spreadsheets are explicit about their assumptions and invite challenge: GiveWell runs periodic open competitions (e.g., the Change Our Mind Contest) soliciting external critique of model assumptions.

The **charity-level reviews** synthesize the four criteria for each top-charity-eligible organization. Reviews are durable, dated, and amended over time. Each review names the charity's program, the relevant intervention report, the cost-effectiveness model output, the room-for-more-funding analysis, the transparency assessment, and the recommendation status.

The **change logs and decision histories** record how GiveWell's recommendations have evolved over time, including which charities have been added or removed and why, and how methodology revisions have changed the model outputs. This corpus is the audit trail of the recommendation process.

The **All Grants Fund** operates as an active grantmaking vehicle, distinct from the Top Charity recommendation list. The All Grants Fund makes grants to organizations and interventions that GiveWell's research suggests are competitive with the Top Charities on cost-effectiveness grounds, including organizations that have not been formally evaluated for Top Charity status. Grants are made directly; the fund is broader than the Top Charities list in both scope and evidentiary posture.

---

## How CROSS Satisfies the GiveWell Methodology

CROSS's gate architecture, evidence primitives, and causal architecture cover the four top-charity criteria and the methodology components described above. The mapping is detailed below.

The **evidence of impact** criterion maps to CROSS's evidence scope and evidence strength primitives. GiveWell privileges outcome and impact evidence (in CROSS evidence-scope terms) and independent evaluation evidence strength (in CROSS evidence-strength terms) for the intervention-level evidence base. A CROSS-conformant program operating in change-obligation mode, with outcome evidence at the completion gate and an attribution causality stance at the pathway level, produces the evidential structure that GiveWell's intervention reports require. The CROSS evidence-type primitive distinguishes activity evidence (delivery), outcome evidence (measured change in the specified population), and standing evidence (institutional standing); GiveWell's intervention reports rely primarily on the outcome evidence type, and the cost-effectiveness models rely on activity evidence at the per-unit delivery level. The CROSS pathway specification (source node, target node, causal mechanism, critical assumptions, external risk, dependency declarations, causality stance) maps directly onto the analytical structure of a GiveWell intervention report.

The **cost-effectiveness** criterion maps to CROSS's evidence scope at the impact level (where a verifiable causal link between funded work and measured change is established through methodology sufficient to support causal inference) and to the CROSS causality stance primitive (where contribution and attribution stances are distinguished, and counterfactual reference is required at the attribution stance). GiveWell's cost-effectiveness analysis is explicitly a counterfactual analysis: it asks how much marginal benefit results from the marginal dollar, given the counterfactual scenario in which the dollar were directed elsewhere. The CROSS counterfactual reference requirement at the attribution stance produces the same analytical artifact at the program level. CROSS does not specify a particular cost-effectiveness threshold or reference benchmark; GiveWell does (multiples of a reference benchmark, currently calibrated to GiveDirectly's cash-transfer cost-effectiveness as the unit reference). A CROSS-conformant program that incorporates a published cost-effectiveness threshold by external standard reference (CROSS Part IV external standard reference mechanism) can adopt GiveWell's reference threshold as the conformance condition, with the GiveWell intervention report cited as the external standard.

The **room for more funding** criterion maps to CROSS's sufficiency architecture declaration (the four-state sufficiency position primitive, applied at the declared scope) and to the additionality declaration in CROSS Part VI-A. GiveWell's room-for-more-funding analysis asks the same question CROSS's sufficiency primitive asks at a different layer: what is the gap between current resources at the declared scope and the resources required to deliver at the marginal cost-effectiveness rate, and what would additional funding actually produce given current absorptive capacity? A CROSS-conformant sufficiency position declaration (critical gap, partial, approaching, or surplus, with corroborating evidence from sources outside the applicant's control) provides the structured input that a GiveWell-style room-for-more-funding analysis requires.

The **transparency** criterion maps to CROSS's gate record legibility provisions, the Attestation Corpus query mechanism, the prior work attribution statement, and the obligation fulfillment record. GiveWell's transparency requirement is functionally a requirement that the charity's operational, financial, and outcome data be inspectable by a third party. CROSS's gate record legibility provisions specify that gate determinations be expressed as publicly verifiable records; the Attestation Corpus query mechanism specifies that third-party verifiable claims about an entity be retrievable without the entity's cooperation; the obligation fulfillment record specifies that prior grants from the same funder be documented with publicly accessible evidence of fulfillment. Taken together, these CROSS provisions instantiate the substantive content of GiveWell's transparency criterion at the program level.

The following table summarizes the core mappings.

| GiveWell Component | CROSS Mechanism |
|:--|:--|
| Top-charity criterion: evidence of impact | Evidence scope at outcome/impact level (Layer 4); evidence type primitive (outcome evidence); pathway specification with causality stance |
| Top-charity criterion: cost-effectiveness | Evidence scope at impact level; attribution causality stance with counterfactual reference; external standard reference to GiveWell intervention report as conformance threshold |
| Top-charity criterion: room for more funding | Sufficiency architecture declaration (four-state position); additionality declaration in Part VI-A |
| Top-charity criterion: transparency | Gate record legibility; Attestation Corpus query; prior work attribution statement; obligation fulfillment record |
| Intervention reports (evidence synthesis) | Pathway specification; external standard reference mechanism (intervention report cited as published evidence standard) |
| Cost-effectiveness analysis spreadsheets | Indicator specification (Fields 1-11); attribution stance with counterfactual reference; financial accountability evidence type |
| Change logs and decision histories | Gate determination records; obligation fulfillment record; multi-cycle retrospective assessment (Layer 7) |
| All Grants Fund grants | Direct application of the same evidentiary structure to a grantmaking vehicle rather than a recommendation list |

---

## How WALKRI Complements This Alignment

WALKRI applies to the field instruments by which GiveWell's evidence inputs are collected, whether collected directly from a grantee organization by GiveWell analysts, supplied by the charity in its own reporting, or extracted by GiveWell from public sources. The intervention reports, cost-effectiveness spreadsheets, and charity reviews depend on inputs that must themselves be measurement instruments rather than labels.

WALKRI's five criterion specification elements (criterion intent, operational definition, response form, evidence form, and conformance threshold) apply to every input field a GiveWell-aligned charity must supply. A field collecting "number of treatments delivered" is not a measurement instrument until it specifies what counts as a treatment (operational definition), how the number is documented (evidence form), what unit is used (component of operational definition), and what evidence standard the documentation must meet for inclusion in the cost-effectiveness model (conformance threshold). A WALKRI-conformant intake of the data that flows into a GiveWell cost-effectiveness model is the structural pre-condition for the model to produce reliable outputs. Without WALKRI-conformant field specification, the cost-effectiveness analysis inherits the ambiguities of its underlying field definitions, and the precision facade failure mode (well-formed numbers without operational substance) becomes a structural risk.

WALKRI's conformance threshold requirement is particularly relevant to the cost-effectiveness analysis. Cost-effectiveness models depend on effect-size assumptions sourced from external research, typically published trials or meta-analyses. The conformance threshold specifies which components of the external standard apply (which trial, what effect size, what subgroup), what evidence satisfies the threshold (the published study, with documented confidence intervals and heterogeneity considerations), and what the minimum standard is for the effect-size assumption to be admissible. A cost-effectiveness model that incorporates an effect-size assumption without a WALKRI-conformant conformance threshold has imported a number whose admissibility cannot be independently checked.

WALKRI also complements the transparency criterion. Transparency, in the GiveWell sense, is not a binary disclosure obligation but a precision requirement: the disclosed data must be specific enough to enable independent verification. WALKRI's bidirectional precision primitive applies the same operational-definition rigor to disclosure as to indicator specification. A charity disclosing its operational data in WALKRI-conformant form provides not only the data but the specification of what the data measure, which is what enables the independent verification that GiveWell's transparency criterion requires.

---

## Edge Cases and Operational Notes

Three points require explicit handling.

First, GiveWell's cost-effectiveness reference threshold (currently expressed as a multiple of a reference benchmark) is a moving calibration. The threshold has been revised over the years as the marginal cost-effectiveness of available giving opportunities has shifted. A program adopting GiveWell's threshold by external standard reference must anchor the threshold to the version active at the round opening, using CROSS's archival anchor requirement, and must update the reference at the next round configuration cycle if GiveWell revises the threshold in the interim. This is the standard CROSS treatment for any time-varying external standard.

Second, GiveWell's intervention reports are concentrated in a small number of program types (currently malaria prevention, deworming, vitamin A supplementation, and a small set of others), with the All Grants Fund extending into a broader set of interventions including direct-cash-transfer programs, vaccination, and selected policy and research grants. A CROSS-conformant program adopting GiveWell's methodology must declare which intervention scope is in play: a program scoped only to GiveWell-recommended intervention types operates within the documented intervention-report architecture, while a program scoped to a broader set of interventions extends beyond the documented architecture and must specify the evidence standard for the unanchored interventions.

Third, the donor-facing framing means GiveWell does not formally require conformance to its standards through contract instruments at the Top Charities level (though it does at the All Grants Fund level). A charity that fails to maintain the documentation rigor GiveWell expects loses recommendation status rather than violating a contractual obligation. For CROSS-conformant adoption, this is a structural distinction: a program that adopts GiveWell-style evidence standards must decide whether it is operating in recommendation mode (where loss of recommendation is the consequence of falling below standard) or in contractual mode where gate failure has the consequences specified in the program's gate configuration. Both are CROSS-conformant; the program must declare which it is using.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
