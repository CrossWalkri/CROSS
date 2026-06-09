---
title: CROSS Runbooks - Second Edition
version: 0.3.1
date: 2026-06-05
license: CC0
status: Second edition, synced to the CROSS Common Reporting Outcome Standards Schema version 0.5.0. Companion document. Extends the first edition (0.1.0) with seven configurations derived from structural primitives identified during worldwide compatibility research. Each configuration is brought into sync with the dimensions the spec made required across versions 0.3.5 through 0.5.0: the organizational identity declaration, the sufficiency architecture declaration, the public benefit mechanism and access condition declaration, the development stage declaration, Continuity Capacity, and the obligation fulfillment record. Read CROSS-runbooks-0_1_0.md first; this document assumes familiarity with the gate architecture and the six runbooks defined there.
related_documents:
  - CROSS/CROSS-common-reporting-outcome-standards-schema-0_5_0.md
  - CROSS/CROSS-runbooks-0_1_0.md
  - CROSS-WALKRI-primitives-framework-index-0_1_0.md
changelog:
  - "0.3.1 (2026-06-08): Frame Language own-voice pass. Own-voice watchlist terms were replaced with the structural act each names (the govern family became covers, sets, or effects; accountability became obligation or answerable; mandatory became required; compliance became conformance; enforces became effects; credible became verifiable; legitimate became genuine). Two renames the earlier cascade had missed were applied: the Part II dimension Governance and continuity resilience is now Continuity Capacity, and Runbook 13 names its construct the feedback-and-response mechanism rather than the accountability mechanism. Framework names, named principles, and citations were preserved. Em-dash sweep clean. No runbook or requirement changed; vocabulary and naming only."
  - "0.3.0 (2026-06-05): Synced to spec 0.5.0. Added a Required Dimensions Across All Runbooks section recording the entry-gate declarations the spec made required since 0.2.0 (organizational identity, sufficiency architecture, public benefit mechanism and access condition, development stage, governance and continuity resilience, obligation fulfillment record), each of which now applies to every runbook in this document. Reframed Runbook 13 as the rich build (a standing feedback channel for the served population) and distinguished it from the served-population risk-bearer floor, which is a baseline consideration in every population-serving round rather than a separate runbook. Added a CRAFT inheritance note recording that CROSS is the first CRAFT domain application (spec Part XIII receipt). No runbook was restructured; no new requirement was invented beyond what the spec states."
  - "0.2.0 (2026-05-19): Second edition. Added seven configurations (Runbooks 7 through 13) derived from structural primitives identified in worldwide compatibility research across 95+ grant frameworks."
---

# CROSS Runbooks - Second Edition

Version 0.3.1 | 2026-06-08 | CC0

---

## About This Document

The six runbooks in CROSS-runbooks-0_1_0.md address the core program types: discovery sprint, staged development, community allocation, retroactive impact, graduated evidence, and institutional conformance. This document adds seven runbooks derived from structural primitives identified during worldwide compatibility research across 95+ grant frameworks. Each new runbook names the primitive that generates it and the frameworks that exemplify that primitive in practice.

The universal gate requirements from the first edition's final section apply to all runbooks in this document without exception. Nothing in this document reduces or supersedes any requirement of the CROSS Common Reporting Outcome Standards Schema.

This edition is synced to schema version 0.5.0. Between schema versions 0.2.0 and 0.5.0 the standard made several entry-gate declarations required across all conformant rounds. Those declarations are recorded once in the next section and apply to every runbook below; the per-runbook gate tables state only the additions specific to each configuration, not the universal entry-gate declarations.

---

## CRAFT Inheritance

CROSS is a domain application of CRAFT (Chains Reveal Attested Falsifiable Truth). A program that adopts CROSS, and therefore any runbook in this document, satisfies CRAFT's six conditions for its grant evaluations without a separate CRAFT implementation. The full inheritance receipt is schema Part XIII. Two consequences are load-bearing for the runbooks here. First, the served population is a named risk-bearer of every round's evaluation under CRAFT Condition 1, carried through every gate, not validated only at entry; this is the floor described in the next section. Second, the pre-specified gate criteria, published before the round opens, are CROSS's realization of CRAFT Condition 4, which is why every runbook below requires its added gate elements to be published in the round configuration before any applicant submits.

---

## Required Dimensions Across All Runbooks

The schema made the following entry-gate declarations required since this document's first edition. Each applies to every runbook below regardless of program type. They are recorded here once rather than repeated in each runbook's gate table. A runbook's gate table states only the gate elements specific to that configuration; these required declarations are assumed present at the entry specification gate in addition to whatever the runbook's table names.

**Organizational identity declaration (schema Part IV).** Every entry specification gate, in every obligation mode, requires the applicant to declare six fields: legal entity name and jurisdiction; parent organization; affiliated entities sharing name, brand, personnel, or codebase; prior round history with this program; disbursement authority (individual, collective, or delegated); and an on-chain identity anchor. The declaration is a pre-condition for gate assessment, not a scored criterion: a submission missing it is incomplete and is not assessed until provided. For each application that supplies an on-chain identity anchor, the funder runs an Attestation Corpus query against named public sources before gate assessment is complete; a prior grant or obligation the query reveals that the applicant did not disclose is a material discrepancy.

**Sufficiency architecture declaration (schema Part IV).** Every entry specification gate requires a scope declaration, a sufficiency position (critical gap, partial, approaching, or surplus, declared at the declared scope), a portfolio context statement, a grant contribution statement, and the revenue architecture type (grant-only, fee-for-service, commercial, or hybrid). The sufficiency position requires at least one piece of corroborating evidence from a source outside the applicant's control; where the funder configures this declaration at independent review strength or above, corroborating evidence is required before gate assessment proceeds. For runbooks with a continuation or retrospective gate, the sufficiency architecture is part of what the continuation determination assesses, since a program's resource position at its declared scope bears on whether further funding closes a real gap.

**Public benefit mechanism and access condition declaration (schema Part II and Part IV).** In every round whose eligibility includes a public goods claim, the entry specification gate requires the applicant to declare which of the four mechanism types the claim rests on (output production, access provision, condition change, or ecosystem shift) and the access condition under which that mechanism holds. The declared mechanism type constrains the evidence scope required at the completion gate: output production commits to output evidence, access provision to usage evidence, condition change to outcome evidence, ecosystem shift to a documented impact contribution argument. For the output production mechanism, the access condition must include the SPDX license identifier and the location of the license file at the completion gate; an all-rights-reserved copyright does not satisfy it. This declaration is a pre-condition for gate assessment in every public-goods runbook below.

**Development stage declaration (schema Part II and Part IV).** Every entry specification gate, in every round, requires the applicant to declare one of five development stages with evidence from a source outside their control. The declared stage constrains which obligation modes are coherent and which evidence scopes are achievable at the completion gate. Funder round configuration must declare which stages are within scope before any applicant submits. A declared stage not supported by the provided evidence is a material discrepancy. For runbooks that target a specific maturity band (for example, retroactive recognition of established infrastructure, or growth-stage scale-up), the stage targeting is stated in the round configuration as a published design decision, not applied as an evaluation judgment after submission.

**Continuity Capacity (schema Part II).** Triggered by grants above a funder-defined size threshold, grants producing ongoing infrastructure with continuing operational requirements, and any applicant with a single named primary contributor and no documented backup capacity. For infrastructure-maintenance and sustained-service runbooks, this dimension is always active regardless of threshold. The applicant declares one of three continuity capacity states (single, partial, or resilient) with supporting evidence; a single-point-of-failure declaration must name the person on whom continuation depends and state what would happen to active grants and funded deliverables if that person became unavailable. The disclosure is not a disqualifier; it is a material fact that affects the continuation determination and the funder's configuration of completion gate conditions. A funder may configure the completion gate to require evidence of partial or resilient continuity as a condition of final disbursement for grants above the threshold.

**Obligation fulfillment record (schema Part IV).** Required at the entry gate before assessment proceeds wherever the applicant has received prior grants from this funder, cites prior work as evidence of capability, or has a prior round history with unresolved KarmaGAP milestones or open gate conditions. The record documents, for each prior grant from this funder: what was committed at that prior round's entry gate, what was produced (with a publicly accessible link), and whether the commitment was fulfilled, partially fulfilled, or unfulfilled with the applicant's explanation. An unfulfilled prior obligation is a disclosed fact, not an automatic disqualifier; an unfulfilled obligation discovered through research that the record omitted is treated more seriously than the failure itself. This record is load-bearing for the multi-cycle and continuation runbooks below, where each cycle's fulfillment feeds the next cycle's entry gate and the retrospective assessment.

**Served-population risk-bearer floor (schema Part II).** In every round whose eligibility rests on serving a defined population, the served population is a named risk-bearer of the round's evaluation, carried through every gate. Each gate determination accounts for that population's exposure, not only the applicant's claim about it: at the completion verification gate, the determination and the unintended outcomes disclosure consider whether the served population bears exposure the round has not surfaced, such as work recorded as delivered that does not reach them, or effects the declared indicators do not capture. The determination record must show the consideration was applied, not merely that the population was named at entry. This floor is a baseline consideration in every population-serving round and is not a separate runbook. A standing feedback channel through which the served population raises concerns during the grant period is the richer build, configured by Runbook 13; the floor does not by itself require that channel.

---

## Runbook 7: Adaptive Learning Cycle

**Primitive this runbook implements:** Inter-cycle reflection stage. A formally required stage between the close of one programme cycle and the opening of the next, in which learning from the completed cycle is reviewed, synthesized, and institutionalized before the next round opens. This primitive is distinct from the completion gate (which closes the current cycle) and the entry specification gate (which opens the next). No runbook in the first edition accommodates a gate between cycles; this runbook formalizes it.

**Framework sources:** World Vision LEAP Programme Cycle (Reflect stage as a required programme cycle component), USAID CLA Collaborating Learning and Adapting Framework (adaptive management embedded in the grant lifecycle), CGIAR MELIA (systematic portfolio-level learning).

**Program type this runbook serves.** Multi-round programs where learning from each round is designed to improve the next. The funder's intent is not only to fund individual grants but to accumulate institutional knowledge about what works in the program's domain. The reflection stage is the mechanism through which that accumulation happens; it is not a retrospective report but a structured review that produces documented changes to the next round's gate configuration, eligibility criteria, or rubric.

**Obligation mode: Build obligation or Change obligation, configurable per round.** The obligation mode sets the individual grant obligations within each round. The reflection stage is a program-level gate, not a grantee-level gate.

**Gate configuration for an individual round.**

| Gate | Active | Evidence scope | Evidence strength | Infrastructure requirement |
|---|---|---|---|---|
| Entry specification | Yes | Output or Outcome (per obligation mode) | Third-party verifiable or Independent review (per obligation mode) | Entry specification must reference findings from the prior reflection stage if a prior round has been completed |
| Progress verification | Configurable | Per obligation mode | Per obligation mode | Standard configuration per obligation mode |
| Completion verification | Yes | Per obligation mode | Per obligation mode | Named reviewer confirms completion and submits learning documentation alongside evidence |
| Reflection gate (between rounds) | Yes | Program-level learning | Facilitated documentation | Designated facilitator or staff synthesizes completion findings into a structured reflection record before the next entry specification gate opens |
| Next entry specification gate | Yes | Per obligation mode | Per obligation mode | The opening of this gate is conditioned on completion of the reflection gate |

**Reflection gate requirements.** Before the next round's entry specification gate may open, the program operator must complete and publish a reflection record covering: (1) what the prior round's completion evidence showed, including unexpected findings; (2) what the round's gate configuration, rubric, or eligibility criteria would be changed to incorporate those findings; (3) what the changes will be in the next round's specification, stated in the form of specific field or criterion modifications; and (4) any indicators that showed insufficient sensitivity or poor commensurability across grantees, with a notation of how they will be revised.

The reflection record is a program-level attestation, not a grantee deliverable. It is produced by the funder or program operator and published before the next round's entry specification gate opens. Grantees may be invited to contribute; they are not required to produce it.

**Entry specification requirements for this runbook.** The entry specification for rounds after the first must reference the prior reflection record: which findings from the prior round informed the current round's design, and what specific criterion or indicator changes were made as a result. An entry specification that does not acknowledge prior reflection findings is a funder-side conformance deficiency.

**Conflict of interest.** Standard three-tier declaration applies per round. Facilitators who produce the reflection record must declare conflicts under Tier 2 (professional relationships with prior-round grantees). The reflection record is a programmatic document, not a funding decision; lower conflict thresholds apply than at the allocation gate. However, a facilitator with a Tier 1 conflict with a prior-round grantee should not produce the sections of the reflection record that assess that grantee's outcomes.

**Infrastructure declaration requirements.** Before each round opens, the funder must publish: who will facilitate the reflection stage, what the reflection process is (structured template, workshop, or peer review), and when the reflection record will be published relative to the next round's opening. The reflection gate is a new gate type and its infrastructure must be declared with the same specificity as completion verification gates.

**Recommended rubric emphasis.** For rounds after the first, the rubric should explicitly credit applications that demonstrate engagement with the prior round's findings: a proposal that addresses a gap identified in the reflection record is more likely to contribute to the program's learning agenda than one that repeats prior-round approaches. The rubric's unintended outcomes section is especially important in adaptive learning programs: unexpected findings from prior rounds are the primary source of reflection record content.

**Required-dimension notes for this runbook.** The obligation fulfillment record (recorded in the Required Dimensions section) is load-bearing here: for rounds after the first, returning applicants must document what they committed and produced in the prior round, and that record is a direct input to the reflection record's account of what the prior round's evidence showed. The development stage declaration also matters across cycles: where an applicant's declared stage advances between rounds, the reflection record should note whether the round's gate configuration still fits the cohort's maturity band. The served-population risk-bearer floor applies to every population-serving round under this runbook; affected-population exposure surfaced at any cycle's completion gate is appropriate content for the next reflection record.

**Recommended evolution path.** A program operating this runbook for three or more cycles will accumulate a body of reflection records that constitutes a longitudinal learning archive. At that point, the program is a candidate for the Multi-Cycle Retrospective configuration (Runbook 8), which formalizes a periodic retrospective assessment across the accumulated cycle record.

**Example programs.** USAID CLA-conformant programs, World Vision and CRS-implemented development programs using LEAP or ProPack, foundations that publish annual learning reports and want to formalize the connection between learning and program design, any multi-round program where the funder wants institutional knowledge to compound across cycles.

---

## Runbook 8: Multi-Cycle Retrospective Program

**Primitive this runbook implements:** Multi-cycle retrospective assessment. A formal evaluation spanning all prior grant cycles in a multi-year grantee relationship, assessing accumulated impact across the full history. This is structurally distinct from a single-cycle final evaluation (which the first edition's runbooks accommodate) and from a retroactive funding round (Runbook 4, which assesses prior work for new funding). The multi-cycle retrospective assesses what a continuing grantee has produced across all prior cycles combined, typically at a defined renewal milestone.

**Framework sources:** National Endowment for Democracy Cumulative Assessment Report (required for renewed multi-year NED grantees; spans all prior grants in a multi-year relationship), CGIAR MELIA (systematic portfolio evaluation across research cycles).

**Program type this runbook serves.** Multi-year programs with continuing grantees who renew funding for the same or related work across multiple grant cycles. At a defined renewal milestone (typically after three to five years or at a defined funding milestone), the continuing grantee undergoes a retrospective assessment covering all cycles in the relationship. The assessment determines whether the accumulated body of work justifies continued investment.

**Obligation mode: Change obligation for ongoing cycles. Retroactive obligation for the retrospective assessment itself.**

The individual cycles use Change obligation: each cycle specifies a FROM state, indicator, and target. The retrospective assessment uses Retroactive obligation: it evaluates what actually accumulated across all prior cycles against the accumulated claims.

**Gate configuration for an individual cycle (same as Institutional Conformance with reduced scope).**

| Gate | Active | Evidence scope | Evidence strength | Infrastructure requirement |
|---|---|---|---|---|
| Entry specification | Yes | Outcome | Third-party verifiable | Named staff reviews the entry specification and the prior-cycle obligation fulfillment record |
| Progress verification | Configurable | Outcome | Third-party verifiable | Standard configuration |
| Completion verification | Yes | Outcome | Independent review | Named independent reviewer confirms the cycle's outcome evidence |
| Continuation specification | Yes (at retrospective milestone) | Accumulated impact | Independent evaluation | See retrospective gate below |

**Retrospective assessment gate (at defined milestone).**

| Gate | Active | Evidence scope | Evidence strength | Infrastructure requirement |
|---|---|---|---|---|
| Retrospective assessment | Yes (at milestone) | Accumulated impact across all prior cycles | Independent evaluation | A qualified evaluator reviews all prior-cycle completion records, obligation fulfillment records, and reflection records (if the Adaptive Learning Cycle configuration was also active) to assess accumulated impact |

**Retrospective assessment requirements.** The retrospective assessment is a structured evaluation by an independent evaluator covering: (1) what outcomes were claimed across all prior cycles, as specified in each cycle's entry specification gate; (2) what evidence was produced at each prior cycle's completion gate; (3) the relationship between claimed outcomes and produced evidence across the full cycle sequence; (4) any evolution in the grantee's indicator specifications across cycles, with assessment of whether the evolution represents genuine learning or a shifting of the measurement goalposts; and (5) a cumulative judgment on whether the accumulated body of work justifies continued investment at the same, reduced, or increased scale.

The critical prerequisite for this runbook is that prior-cycle indicator specifications must be preserved in a comparable form. A multi-cycle retrospective cannot function if each cycle's indicators were defined in inconsistent terms. This is why WALKRI's pre-publication requirements, applied consistently at each cycle's entry gate, are load-bearing for this runbook: they produce indicator specifications that are commensurable across cycles by design.

**Trigger conditions for the retrospective gate.** The funder publishes the trigger conditions before the first cycle of the multi-year relationship opens. Trigger conditions may include: completion of a defined number of cycles, reaching a cumulative funding threshold, reaching a defined program milestone, or a calendar-fixed review date. The trigger conditions must be published and cannot be moved to avoid triggering the retrospective.

**Conflict of interest.** The independent evaluator for the retrospective assessment must have no prior involvement in any individual-cycle completion review for this grantee. The cumulative assessment is a higher-stakes determination than any individual-cycle gate; the evaluator independence standard is correspondingly higher. The evaluator must declare conflicts under all three tiers and receive formal approval before accessing any cycle documentation.

**Infrastructure declaration requirements.** At the first cycle's entry gate, the funder must publish: when the retrospective assessment will be triggered, who will commission the evaluator (and that they will be independent of prior-cycle reviewers), and what the assessment will cover. This pre-commitment at the start of the multi-year relationship is what prevents the retrospective from being designed retroactively to favor a preferred outcome.

**Recommended rubric emphasis.** The retrospective assessment rubric must give the highest weight to the comparison between claimed outcomes at entry and produced evidence at completion, across all prior cycles. Consistent overestimates of targets followed by consistent under-delivery at completion is a more disqualifying pattern than one cycle of underperformance. The rubric should distinguish three grantee patterns: consistent delivery against stated targets (strong case for continuation), consistent adaptation of indicators to match achievable performance (medium case; requires close scrutiny), and consistent gap between stated targets and produced evidence (weak case for continuation).

**Required-dimension notes for this runbook.** Three of the required dimensions are load-bearing for the retrospective. The obligation fulfillment record, submitted at each cycle's entry gate, is the running ledger the retrospective assessment reads: the retrospective compares what each prior cycle committed against what it produced, and the fulfillment record is where those commitments and outcomes are documented cycle by cycle. The sufficiency architecture declaration is part of the continuation determination at the retrospective milestone: whether the accumulated body of work justifies continued investment at the same, reduced, or increased scale is in part a question about the grantee's resource position at the declared scope, which the sufficiency position and grant contribution statement carry. Continuity Capacity is active throughout a multi-year relationship: a continuing grantee that remains a single point of failure across all cycles is a continuity exposure the retrospective should surface, since the accumulated impact depends on a person whose departure would end it. The development stage declaration across cycles also informs the retrospective's judgment of whether indicator evolution reflects genuine maturation or a shifting of measurement goalposts.

**Recommended evolution path.** A grantee who passes a retrospective assessment is a candidate for scale-up. A grantee who fails should have their continuation gate suspended and enter a remediation cycle before any new entry gate is opened.

**Example programs.** NED multi-year grantee relationships, USAID long-term partner programs, foundation programs with multi-year cohorts, any program where the funder intends to maintain a continuing relationship with a grantee across multiple cycles and wants a formal obligation structure for that relationship.

---

## Runbook 9: Threshold-Scaled Independence

**Primitive this runbook implements:** Threshold-based independent evaluation. Evaluator independence scales with grant size automatically, as a published structural feature of the round rather than a case-by-case determination. Below a defined threshold, self-report or staff review is sufficient. Above the threshold, independent evaluation is required. The threshold, the independence requirement, and the evaluator criteria are published before any application is submitted.

**Framework sources:** UN Women UNTF (grants over USD 150,000: required final external evaluation; grants under USD 150,000: co-managed evaluation with the UNTF Secretariat), AmeriCorps State and National (grants above USD 500,000 average annual: independent evaluation required and submitted with competitive reapplication), CROSS standard evidence strength taxonomy (tiered from self-report through independent evaluation).

**Program type this runbook serves.** Programs with a wide range of grant sizes, where the appropriate level of independent verification is proportional to the funding level. Rather than requiring the same evidence strength from a USD 5,000 grant and a USD 500,000 grant, this runbook codifies the proportionality principle as a structural feature of the program: the threshold at which independence is required is published and fixed before any application opens.

**Obligation mode: Build obligation or Change obligation, configurable by the funder.**

**Gate configuration.**

| Gate | Active | Evidence scope | Evidence strength | Infrastructure requirement |
|---|---|---|---|---|
| Entry specification | Yes | Per obligation mode | Self-report with documentation (all tiers) | Staff review of entry specification |
| Progress verification | Configurable | Per obligation mode | Per obligation mode (tiered) | See tier configuration below |
| Completion verification: Tier 1 (below lower threshold) | Yes | Per obligation mode | Self-report with documentation | Named staff reviews submitted evidence against published completion criteria |
| Completion verification: Tier 2 (at or above lower threshold, below upper threshold) | Yes | Per obligation mode | Third-party verifiable | Named staff or designated community reviewer with no relationship to the applicant confirms evidence from publicly accessible sources |
| Completion verification: Tier 3 (at or above upper threshold) | Yes | Per obligation mode | Independent review or Independent evaluation | Named independent reviewer (at lower end of Tier 3) or qualified independent evaluator (at higher end of Tier 3) conducts structured evidence review |
| Continuation specification (for reapplication) | Configurable | Per obligation mode | Per prior-cycle tier | If the program requires reapplication, Tier 3 completion verification results must be submitted with the reapplication |

**Threshold publication requirement.** Before the round opens, the funder must publish three values: the lower threshold (below which Tier 1 applies), the upper threshold (above which full independent evaluation is required), and the definition of the Tier 2 zone. The thresholds must be published in the same currency and accounting unit as the grant amounts. Thresholds may not be adjusted after the round opens without a formal round specification amendment that is published and timestamped before any application is submitted.

**Evaluator qualifications for Tier 3.** The infrastructure declaration must specify what qualifications a Tier 3 evaluator must hold. Qualifications must be stated in terms of domain expertise and structural independence, not as named individuals (the specific evaluator is typically selected after award). The evaluator selection process must be described: who selects, what the evaluator declaration of independence covers, and who reviews the declaration.

**Reapplication requirements for Tier 3 grantees.** If the program allows or requires reapplication, Tier 3 grantees must submit their completed independent evaluation results with their reapplication. A Tier 3 grantee who has not completed the evaluation at the time of reapplication does not qualify for the continuation gate until the evaluation is submitted. This is the structural implementation of AmeriCorps's requirement that evaluation results accompany competitive reapplication.

**Conflict of interest.** Standard three-tier declaration applies at all tiers. Tier 3 evaluators must complete a full independent declaration before accessing any grant materials.

**Recommended rubric emphasis.** The threshold determination should be made at the grant size calculation stage, not at the completion gate. For programs where award amounts are not fixed at entry (quadratic funding, community allocation), the threshold determination must be based on a published rule for how final award amounts translate to tier assignment. The rubric for Tier 3 completion verification should specify exactly what the independent evaluation must include to satisfy the independence requirement: the evaluator's declared independence, the evidence sources reviewed, and the evaluation methodology applied.

**Required-dimension notes for this runbook.** This runbook scales evidence strength with grant size; two required dimensions scale alongside it. Continuity Capacity is triggered above a funder-defined size threshold, so the same upper threshold that activates Tier 3 independent evaluation typically also activates the requirement for evidence of partial or resilient continuity as a completion-gate condition: a large grant carries both a higher verification bar and a higher continuity bar. The funder may align the two thresholds or set them independently, but each must be published before the round opens. The development stage declaration is required at every tier and constrains which obligation modes are coherent at that grant size; a Tier 3 grant declared at an early development stage warrants scrutiny that the independent evaluation can in fact reach the declared mechanism's evidence scope. The sufficiency architecture declaration is required at all tiers regardless of grant size.

**Recommended evolution path.** A program running this runbook over multiple cycles should track whether the threshold levels remain appropriate. If Tier 3 evaluations are consistently finding strong evidence, the lower threshold may be raised. If Tier 2 reviews are consistently finding weak evidence that a proper Tier 3 evaluation would have surfaced, the thresholds should be lowered.

**Example programs.** Programs with a wide range of grant sizes; grantmaking programs within foundations that fund both small community grants and large institutional partnerships; any program where the funder wants to apply proportional verification without making independence determinations case-by-case.

---

## Runbook 10: Participatory Indicator Selection

**Primitive this runbook implements:** Participatory indicator selection from a published menu. Grantees choose from a published set of indicators rather than freely designing their own. The menu constitutes the funder's pre-commitment; selection from it is the grantee's pre-commitment; funder confirmation of the selection is the gate. This preserves grantee agency while ensuring that all selected indicators are commensurable across the grantee cohort.

**Framework sources:** Inter-American Foundation Grassroots Development Framework (41-indicator menu; participatory selection with IAF technical assistance; baseline established before grant activities begin), SNAP-Ed Evaluation Framework (priority indicator selection from a published 51-indicator set; state plans specify which indicators apply before funding is released), Head Start/ELOF (five developmental domains as a fixed indicator menu to which grantees align their school readiness goals).

**Program type this runbook serves.** Programs where grantees operate in diverse contexts that cannot be served by a single fixed indicator set, but the funder requires commensurability across the grantee cohort. Rather than imposing a uniform fixed indicator or allowing unconstrained indicator design, the funder publishes a curated indicator menu and grantees select the applicable subset. This is the appropriate configuration for community development, agricultural extension, grassroots development, and other programs where context variation is high and grantee agency in indicator design is a value.

**Obligation mode: Change obligation.** Participatory indicator selection is meaningful only where the program targets measurable condition changes. Build obligation programs with specific deliverables do not benefit from indicator menus because the deliverable is already defined. This runbook assumes Change obligation throughout.

**Gate configuration.**

| Gate | Active | Evidence scope | Evidence strength | Infrastructure requirement |
|---|---|---|---|---|
| Indicator menu publication | Required before round opens | Not a gate in the standard sense | Published documentation | The funder publishes the indicator menu with complete specifications (all five WALKRI requirements satisfied for each indicator) before the application window opens |
| Entry specification | Yes | Outcome | Third-party verifiable | Grantee submits indicator selections from the published menu with baseline documentation; funder confirms or returns for revision |
| Indicator confirmation gate | Yes | Outcome | Third-party verifiable | Named staff confirms the grantee's selected indicators are drawn from the published menu and the baseline documentation satisfies the WALKRI operational definition for each selected indicator |
| Progress verification | Configurable | Outcome | Third-party verifiable | Standard configuration; data collected against confirmed indicator selections |
| Completion verification | Yes | Outcome | Third-party verifiable or Independent review | Evidence submitted against the confirmed indicator selections; no substitution of indicators after the confirmation gate |
| Continuation specification | Configurable | Outcome | Third-party verifiable | If continuation is configured, prior-period indicator selections must be maintained unless a formal indicator revision process is completed |

**Indicator menu requirements.** The indicator menu is the funder's primary pre-commitment under this runbook. Each indicator in the menu must satisfy all five WALKRI pre-publication requirements before the menu is published: criterion intent, operational definition, response form, evidence form, and conformance threshold. A menu that contains label-level indicator names without operational specifications is not conformant. The menu must be published as a stable document with a version number and date before the application window opens; revisions to the menu require a new version with a new date and a documented reason for each change.

**Baseline requirement.** Before any grant activity begins, the grantee must document a baseline for each selected indicator using the evidence form specified in the menu. Baseline documentation is submitted alongside the indicator selections at the entry specification gate. Funder confirmation of the baseline is part of the indicator confirmation gate. A grantee who selects indicators but cannot document baselines at the menu's specified evidence standard fails the indicator confirmation gate.

**Indicator revision procedure.** After the indicator confirmation gate, indicator substitution is not permitted except through a formal revision procedure. The revision procedure must be published before the round opens and must require: a written request from the grantee explaining why the original indicator cannot be measured as specified, funder review of the request, and publication of the revision decision and rationale. Approved revisions must include a bridging baseline connecting the prior indicator's data to the replacement indicator's data, where possible.

**Portfolio commensurability.** The indicator menu design is the tool through which the funder ensures that data from different grantees can be compared. At round close, the funder should be able to produce aggregate data for each indicator in the menu across all grantees who selected it. This requires that the menu's operational definitions be specific enough that data from different grantees in different contexts reflects the same underlying construct. The WALKRI pre-publication audit of the menu is the instrument that confirms this before any grantee selects an indicator.

**Conflict of interest.** Standard three-tier declaration applies. Staff who developed the indicator menu must declare conflicts before participating in indicator confirmation gate reviews for individual grantees.

**Infrastructure declaration requirements.** The indicator confirmation gate requires a named staff member or reviewer. The funder must also publish who developed the indicator menu and what process was used to validate the menu's operational definitions, to establish that the menu is not simply a set of labels.

**Recommended rubric emphasis.** The indicator confirmation gate rubric should weight the baseline documentation most heavily. A grantee who selects appropriate indicators but cannot document a verifiable baseline is not ready to implement the program; the indicator confirmation gate should return their submission for revision before any grant funds are disbursed. The portfolio commensurability dimension should be an explicit rubric criterion: does this grantee's baseline documentation use the same data collection method specified in the menu, or has the grantee substituted a different method that produces non-comparable data?

**Required-dimension notes for this runbook.** This runbook operates in Change obligation, so the public benefit mechanism declaration where eligibility includes a public goods claim typically rests on the condition-change mechanism type, which commits the applicant to outcome evidence at the completion gate; the selected indicators from the menu are the operational form of that commitment, and the mechanism type declared at entry must be consistent with the indicators selected. Because this runbook serves community development, agricultural extension, and grassroots development programs, the served-population risk-bearer floor is active in nearly every round under it: each gate determination accounts for whether the funded work reaches the population the selected indicators are meant to measure, not only whether the indicator moved. Where a funder wants a standing channel for that population to raise concerns during the grant period, that is the richer build configured by Runbook 13, which combines naturally with this runbook. The development stage declaration is required at entry and bears on whether a grantee can reliably document the baselines the menu requires.

**Recommended evolution path.** After three or more cycles, the funder should review the indicator menu to identify which indicators were selected frequently, which were rarely selected, and which produced baseline documentation that was consistently non-comparable. Rarely selected indicators may indicate poor fit with the program's context; consistently non-comparable baseline documentation may indicate that the indicator's evidence form specification is insufficiently precise and needs revision in the next menu version.

**Example programs.** IAF grassroots development programs, SNAP-Ed state plan programs, community foundation programs where grantees operate in diverse contexts and need to select from a common vocabulary, national service programs where local chapters implement different program types but must report against a common indicator set.

---

## Runbook 11: Computational Retroactive Allocation

**Primitive this runbook implements:** Formula-based retroactive allocation with a pre-specified metrics formula, an impact chain dependency declaration, and a human-in-the-loop override with published override conditions. This runbook extends Runbook 4 (Retroactive Impact) to address the structural innovations introduced in Optimism's 2025 Retro Funding methodology: replacing subjective badgeholder voting with a mathematical formula, requiring projects to declare their position in a causal chain, and pre-specifying the conditions under which the formula output can be overridden by a committee decision.

**Framework sources:** Optimism Retro Funding 2025 methodology (weighted impact metrics formula replacing subjective voting; Impact Chain dependency graph; human-in-the-loop override with published conditions; formula and weights committed before applications open).

**Program type this runbook serves.** Retroactive funding programs that want to reduce the role of subjective preference in allocation decisions by using a pre-specified formula applied to independently verifiable impact metrics. The formula replaces or supplements badgeholder voting, expert panel scoring, or other deliberative mechanisms with a computable allocation based on metrics committed to before the assessment period opens.

**Obligation mode: Retroactive obligation.**

**Gate configuration.**

| Gate | Active | Evidence scope | Evidence strength | Infrastructure requirement |
|---|---|---|---|---|
| Metrics formula publication | Required before round opens | Not a gate in the standard sense | Published documentation with formula and weights | The funder publishes the complete metrics formula, all input weights, and the computation methodology before any application or nomination opens |
| Impact chain declaration | Yes (at application) | Usage and Outcome | Third-party verifiable | Each applicant declares the position of their contribution in a causal chain showing how their outputs connect to the ecosystem outcomes the round is designed to fund |
| Entry specification | Yes | Output, Usage, and Impact chain | Third-party verifiable | Applicant submits impact evidence for each input metric in the formula, with evidence references accessible from independent sources |
| Formula application | Yes | Computed allocation | Deterministic | Named staff or automated system applies the published formula to the submitted and verified metric inputs; the computed allocation is published before the override review |
| Override review | Configurable (if override conditions exist) | Computed allocation | Committee decision against pre-specified conditions | A designated committee reviews the computed allocation against the published override conditions; override requires documentation of which condition was triggered and how |
| Final allocation | Yes | Published record | Committee approval or formula output | The final allocation is published with documentation of whether the formula output was applied unchanged or an override was invoked |

**Metrics formula requirements.** The funder must publish, before the round opens: the complete list of impact metrics, the formula for combining metric inputs into a final allocation score, the weights applied to each metric input, the data source or verification standard for each metric input, and the computation methodology in enough detail that an independent party could reproduce the computation from the same metric inputs. The formula is a gate criterion: once published, it cannot be changed after any application or nomination opens.

**Impact chain declaration requirements.** Each applicant must declare the position of their contribution in an impact chain: which downstream outcomes their outputs enable or contribute to, what the dependency pathway is, and whether any other projects in the round depend on or are depended upon by their contribution. Circular impact chains (a project claiming to enable an outcome that, in turn, claims to produce the output this project depends on) fail the impact chain review. Unverifiable dependency claims (claiming to enable downstream outcomes for which no independent evidence exists) fail the impact chain review. The impact chain declaration must be submitted before metric inputs are collected.

**Override conditions.** If the funder intends to allow committee override of the formula output, the conditions under which override may be invoked must be published before the round opens. Conditions must be specific enough that a committee decision invoking override can be verified against the published conditions after the fact. "The formula produced a result inconsistent with the round's goals" is not a specific enough override condition. A specific override condition is: "The formula produced a result where more than [X]% of total allocation flows to projects with fewer than [Y] independent users, which the funder's published definition of ecosystem alignment prohibits." Every override invocation must document which condition was triggered, by what evidence, and what the override decision was. Override decisions that do not reference a published condition are a funder-side conformance failure.

**Conflict of interest.** Committee members who participate in override review must declare conflicts under all three tiers before reviewing any formula output. A committee member who is affiliated with a project whose computed allocation would be materially affected by an override is a Tier 1 conflict and must recuse from the override review.

**Infrastructure declaration requirements.** Before the round opens, the funder must publish: who will apply the formula, what data validation procedure applies to submitted metric inputs, who will constitute the override committee if override is configured, and what the timeline is from formula application to publication of the final allocation.

**Recommended rubric emphasis.** The impact chain declaration quality is the most load-bearing rubric criterion in this runbook. A formula-based allocation that accepts any claimed impact without impact chain validation is vulnerable to inflation of upstream outputs (a project claiming to enable ten downstream outcomes when evidence supports only one). The rubric should specify what constitutes a verifiable dependency claim versus an unverifiable one: a dependency claim is verifiable when the downstream project has publicly acknowledged the upstream contribution, when on-chain usage data shows the dependency, or when public documentation records the relationship.

**Required-dimension notes for this runbook.** Two required dimensions are especially load-bearing in a formula-based retroactive round. The organizational identity declaration's on-chain identity anchor is the key the funder uses to run the Attestation Corpus query, which in an on-chain retroactive program is a primary input to verifying the metric inputs the formula consumes: an applicant's prior attestations, milestones, and endorsements across named public sources corroborate or contradict the claimed impact before the formula is applied. The development stage declaration is also material: retroactive recognition of prior contribution is Stage 5 in the spec's stage taxonomy, and the round configuration should declare whether it accepts only Stage 5 retroactive applicants or also accepts established-infrastructure applicants presenting prior contribution as a baseline. Where the round's eligibility includes a public goods claim, the ecosystem shift mechanism type is the natural fit for the impact chain declaration, and the access condition statement names the causal pathway and co-factor list the impact chain review then tests. The obligation fulfillment record applies to any applicant with prior grants from this funder, and an undisclosed prior obligation that the Attestation Corpus query reveals is a material discrepancy that the impact chain review must surface before formula application.

**Recommended evolution path.** After two or more rounds using this configuration, the funder should review whether the formula's metric weights are producing allocations that reflect the program's intended priorities. If consistently high-metric-scoring projects are consistently producing lower-than-expected downstream impact, the formula weights may need revision. Any revision to the weights must go through the metrics formula publication requirement before the next round opens.

**Example programs.** Optimism Retro Funding, any retroactive public goods program that wants to reduce subjectivity in allocation, protocol treasury programs distributing retroactive rewards to infrastructure contributors.

---

## Runbook 12: Portfolio Benchmark Program

**Primitive this runbook implements:** Portfolio-level continuation benchmark applied to the funder. A published performance threshold applies to the funder's entire grant portfolio rather than to individual grantees. The funder pre-commits to a portfolio-level outcome before the round opens; if the portfolio fails to meet the threshold, the funder is answerable for explaining why and what changes will be made to the program design. This is structurally distinct from grantee-level gate obligation: the portfolio benchmark is a funder-side obligation.

**Framework sources:** SBIR/STTR statutory benchmarks (Phase I-to-Phase II transition rate minimum of 0.25 and USD 100,000 commercialization revenue per Phase II award average; applied to the federal agency's full SBIR/STTR portfolio; failure triggers conformance review), ESIF CPR Performance Framework (portfolio-level milestones and targets at the programme level with mid-term consequences).

**Program type this runbook serves.** Grant programs where the funder's own performance is answerable alongside grantees' performance. The funder commits to a portfolio-level outcome before any round opens - a minimum rate of successful completion, a minimum aggregate outcome, or a minimum rate of advancement from one stage to the next - and publishes the portfolio results alongside individual grantee results at round close.

**Obligation mode: Build obligation or Change obligation per individual grant, configurable. Portfolio benchmark mode is an additional program-level obligation layer.**

**Gate configuration for individual grants.** Standard configuration per the applicable runbook for the individual grant type (Discovery Sprint, Staged Development, Graduated Evidence, or other). No modification to individual grant gate configuration is required.

**Portfolio benchmark configuration.**

| Portfolio gate | Active | Evidence scope | Evidence strength | Infrastructure requirement |
|---|---|---|---|---|
| Portfolio benchmark publication | Required before round opens | Not a grant gate | Published documentation | The funder publishes the portfolio benchmark before the first round opens: what threshold the portfolio must meet, how it is measured, and what the consequences are if the threshold is not met |
| Portfolio outcome tracking | Active throughout round | Aggregate output and outcome | Third-party verifiable | Named staff tracks completion rates and outcome evidence across all active grants; portfolio data is aggregated and prepared for publication |
| Portfolio assessment | Yes (at round close) | Aggregate outcome | Independent review (for programs with explicit consequences) | Named reviewer or designated audit function assesses whether the portfolio benchmark was met |
| Portfolio results publication | Required at round close | Aggregate outcome | Published documentation | The funder publishes the portfolio results, the benchmark, whether the benchmark was met, and if not, what changes to the next round's design are planned |

**Portfolio benchmark requirements.** The benchmark must be specific enough to be verifiable. Acceptable benchmark forms include: minimum proportion of grantees that pass the completion gate (e.g., "at least 70% of grantees must pass the completion gate within the grant period"), minimum aggregate outcome (e.g., "the portfolio must produce at least X total instances of the primary outcome indicator across all grantees"), or minimum stage-advancement rate (e.g., "at least 25% of Stage 1 grantees must qualify for Stage 2 within 18 months"). The benchmark must be published in the same units as the tracking measure, so that portfolio results can be compared to the published benchmark without ambiguity.

**Consequences of benchmark failure.** If the portfolio fails to meet the published benchmark, the funder must publish: an explanation of why the benchmark was not met, what the funder concludes about the program design from the failure, and what specific changes will be made to the next round to address the failure. A funder who fails the portfolio benchmark and does not publish this explanation has failed to meet the funder-side conformance requirement for this runbook. Benchmark failure does not automatically require the funder to reduce portfolio size or close the program; it requires answerability and explanation.

**Disaggregation of portfolio results.** Portfolio results should be disaggregated where the portfolio's design targeted specific populations or outcome domains. A portfolio benchmark of "70% completion" means less if the completing 70% are all low-complexity grants and the failing 30% are all high-complexity grants. Disaggregated portfolio results allow the funder and the field to understand which program components are performing and which are not.

**Conflict of interest.** The independent review of portfolio assessment must be conducted by a reviewer with no financial relationship with any individual grantee in the portfolio. Portfolio reviewers are assessing funder performance, not grantee performance; the conflict of interest framework applies to the funder's relationships, not only the grantees'.

**Infrastructure declaration requirements.** Before the round opens, the funder must publish the portfolio benchmark, the tracking methodology, the publication schedule for portfolio results, and who will conduct the portfolio assessment. This is a funder-side infrastructure declaration, not a grantee-side one.

**Recommended rubric emphasis.** The portfolio benchmark design rubric (applied by the funder to their own design, not by reviewers to grantees) should ask: is the benchmark set at a level that is demanding but achievable given the program design? A benchmark that is set at a level the program has already consistently met requires no answerability. A benchmark that is set above what any comparable program has achieved is likely to fail and generate noise rather than learning. The benchmark calibration is a program design decision that should be made with reference to comparable programs' historical completion rates.

**Required-dimension notes for this runbook.** This runbook adds a funder-side layer and leaves individual grant gate configuration unchanged, so all required dimensions in the Required Dimensions section apply to the individual grants exactly as they would under whichever runbook applies to those grants. Two interactions are worth naming at the portfolio level. The served-population risk-bearer floor operates per grant, but a portfolio benchmark that aggregates only completion rates can mask served-population exposure: a portfolio reported as meeting its benchmark while individual completion records show work that did not reach the intended population is not a portfolio in good standing, and the disaggregation of portfolio results should make served-population reach visible where the portfolio targeted specific populations. The development stage declaration enables a second useful disaggregation: a portfolio benchmark of stage-advancement (for example, the share of early-stage grantees that reach a later stage) is coherent only when each grant carries a published development stage declaration at entry, which this runbook inherits from the Required Dimensions section.

**Recommended evolution path.** A funder that has run this runbook for two or more rounds with consistent benchmark achievement should raise the benchmark. A funder that has consistently missed the benchmark should review whether the individual grant gate configuration is appropriate for the program's grantees, or whether the benchmark was miscalibrated at program design.

**Example programs.** SBIR/STTR-aligned programs that want to apply the portfolio benchmark primitive in a non-federal context, competitive grant programs that want to be answerable for portfolio-level performance rather than only individual-grant performance, foundation programs with multi-year portfolios where the foundation wants to publish its own performance alongside grantee performance.

---

## Runbook 13: Affected Population Verification Gate

**Primitive this runbook implements:** Affected population verification mechanism as a formal gate element. Community feedback and complaint response mechanisms are required components of the program design that must be specified and published before any grantee or member of the affected population engages with the program, not optional add-ons or retrospective obligation features.

**Framework sources:** CRS ProPack II (community feedback loops and complaint response mechanisms as required MEAL system components; specification of collection, review, and response requirements before program implementation), World Vision LEAP Community Based Feedback and Response Mechanism (integrated across all six LEAP programme cycle components), Core Humanitarian Standard Commitment 5 (access to safe and responsive complaint mechanisms as a humanitarian accountability standard).

**This runbook is the rich build, not the floor.** The schema (Part II) carries a served-population risk-bearer floor: in every round whose eligibility rests on serving a defined population, the served population is a named risk-bearer of the round's evaluation, and each gate determination accounts for that population's exposure rather than only the applicant's claim about it. That floor is a baseline consideration in every population-serving round; it is recorded in the Required Dimensions section above and is not a separate runbook. This runbook is the richer build the schema distinguishes from that floor: a standing channel through which the served population raises concerns during the grant period, specified and published as a gate element before any member of that population engages with the program. A funder that activates this runbook installs the standing channel; a funder that does not still owes the floor. The floor asks each gate to consider served-population exposure; this runbook gives the served population an active route to surface that exposure themselves while the grant is running. Where this runbook is not active, the floor still requires the completion verification gate to consider whether the served population bears exposure the round has not surfaced.

**Program type this runbook serves.** Programs where the people served by grant-funded activities are meaningfully different from the organizations applying for grants; where those people have limited power relative to the organizations that design and implement the programs; and where the funder believes that answerability to those people is a structural requirement rather than a program quality consideration. This typically includes: humanitarian response programs, community development grants, social services programs, and any program where the affected population did not ask to receive the program or cannot easily exit if the program is not working for them.

**Obligation mode: Change obligation.** Affected population verification mechanisms are most meaningful when the program has a declared theory of change specifying how it is intended to affect the people it serves. The completion gate evidence must include not only outcome data but evidence from the verification mechanism.

**Gate configuration.**

| Gate | Active | Evidence scope | Evidence strength | Infrastructure requirement |
|---|---|---|---|---|
| Feedback-and-response mechanism specification | Required before round opens | Not a grant gate | Published documentation | The funder publishes the feedback-and-response mechanism requirements: what type of mechanism is required, what the mechanism must be able to receive, how responses must be documented, and what the minimum response timeframe is |
| Entry specification | Yes | Outcome and Feedback-and-response mechanism design | Third-party verifiable | Applicant specifies not only outcome indicators but the feedback mechanism design, including: how the affected population can submit feedback or complaints, how submissions will be received and recorded, who is responsible for reviewing and responding, and what the response timeline is |
| Feedback-and-response mechanism review | Yes (before disbursement) | Feedback-and-response mechanism design | Staff review | Named staff confirms the proposed mechanism satisfies the published requirements; a mechanism that has not been designed is a disbursement hold, not a grantee deficiency to be remediated post-award |
| Progress verification | Configurable | Outcome and Feedback-and-response mechanism operation | Third-party verifiable | Evidence that the mechanism is operational: number of submissions received, response rate, response time, nature of issues raised |
| Completion verification | Yes | Outcome and Feedback-and-response findings | Third-party verifiable or Independent review | Completion evidence must include: outcome data AND a summary of feedback mechanism findings, including any systemic issues raised, how they were responded to, and whether any program adaptations resulted from feedback |
| Continuation specification | Configurable | Feedback-and-response findings | Third-party verifiable | If continuation is configured, a review of feedback-and-response mechanism findings from the prior period is part of the continuation gate assessment |

**Feedback-and-response mechanism requirements.** The feedback-and-response mechanism must be specified before any member of the affected population is enrolled in or exposed to the program. The minimum requirements, published by the funder before the round opens, must specify: (1) what categories of input the mechanism must be able to receive (feedback, complaints, safety concerns, service quality issues); (2) what channel the mechanism must operate through (in-person, phone, written, digital, or multiple channels, with specification of which channel is primary); (3) what anonymity or confidentiality protection applies; (4) what the maximum response timeline is for an initial acknowledgment and a substantive response; and (5) what records the grantee must maintain of submissions and responses.

A mechanism specification that names a channel without specifying how it operates, what it can receive, and how responses are documented is a label, not a mechanism. WALKRI's operational definition requirement applies to the feedback-and-response mechanism fields in the entry specification: what counts as a valid complaint submission, what counts as a documented response, and what constitutes a timely response must be specified before any member of the affected population can use the mechanism.

**Integration with outcome evidence.** The completion gate requires that feedback-and-response mechanism findings be presented alongside outcome data. A program that produced its stated outcomes but whose feedback-and-response mechanism received multiple unresolved complaints about program delivery is not unconditionally complete: the unresolved complaints are adverse signals that must be addressed before the completion gate closes. The funder must specify in advance what level of unresolved complaints triggers a completion gate delay or a reduced disbursement.

**Conflict of interest.** The feedback mechanism must be structured so that the affected population can submit complaints about the grantee without that complaint going through the grantee's own staff. A mechanism that routes all submissions through the implementing organization's program staff is not independent. The mechanism must have at least one channel that allows submission directly to the funder or to an independent intermediary designated by the funder.

**Infrastructure declaration requirements.** Before the round opens, the funder must publish: the feedback-and-response mechanism requirements in enough detail for grantees to design conformant mechanisms, the review process for the feedback-and-response mechanism review gate, and what the funder will do if a mechanism review finds the proposed mechanism is not conformant. This is especially important for programs with short application timelines: grantees need to know what is required before the application opens, not after.

**Recommended rubric emphasis.** The feedback-and-response mechanism review is the gate where the most common failure occurs: mechanisms are named but not specified. The rubric should give the highest weight to operational specificity: does the proposed mechanism specify what it can receive, how it operates, who is responsible, and what the response timeline is? A mechanism that names a phone number without specifying who answers, when, in what language, and how calls are recorded fails the specification requirement regardless of how accessible the number is.

**Recommended evolution path.** After two or more rounds, the funder should review the aggregate feedback-and-response mechanism findings across the grantee portfolio. Patterns in the nature of submissions (recurring complaints about a specific program component, systematic issues with service quality in a specific geographic area) are portfolio-level signals that should feed into the Adaptive Learning Cycle configuration (Runbook 7) if that runbook is also active.

**Example programs.** CRS and World Vision-implemented development programs, Core Humanitarian Standard-aligned humanitarian response programs, community development grants where the funded organizations serve populations with limited power, any program where the funder has a genuine obligation to the people the grant-funded work is intended to serve.

---

## Combining Runbooks

These runbooks may be combined. The following combinations are natural:

**Runbooks 7 and 8 together (Adaptive Learning + Multi-Cycle Retrospective):** The Adaptive Learning Cycle produces inter-cycle reflection records; the Multi-Cycle Retrospective requires that prior indicator specifications be preserved in comparable form. Together they form a complete multi-year learning architecture: reflection between each cycle, retrospective assessment at the defined milestone. The reflection records are primary inputs to the retrospective evaluation.

**Runbooks 9 and 10 together (Threshold-Scaled Independence + Participatory Selection):** Participatory indicator selection creates a portfolio of grantee-selected indicators; threshold-scaled independence ensures that large grants are independently evaluated against their selected indicators. The combination produces a program that respects grantee agency in indicator design while scaling independent verification with grant size.

**Runbooks 12 and any other runbook (Portfolio Benchmark):** Runbook 12 adds a funder-side obligation layer to any program. It is compatible with all individual grant configurations and simply adds the portfolio-level publication requirement on top of whatever individual gate configuration the program uses.

**Runbooks 13 and 7 together (Affected Population Verification + Adaptive Learning):** The feedback-and-response mechanism findings from Runbook 13 are natural inputs to the reflection stage from Runbook 7. Systematizing this flow - requiring that feedback-and-response findings be a required element of the reflection record - creates a feedback loop from affected population experience to program design.

**Runbook 11 combined with any retroactive configuration:** The Computational Retroactive Allocation configuration is compatible with Runbook 4 (Retroactive Impact) as an extension: a program that already uses Runbook 4 can migrate to formula-based allocation by adding the metrics formula publication gate and the impact chain declaration gate to its existing configuration.

---

## Universal Gate Requirements

All requirements from the Universal Gate Requirements section of CROSS-runbooks-0_1_0.md apply to all runbooks in this document without exception. They are not repeated here; they apply by default.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
