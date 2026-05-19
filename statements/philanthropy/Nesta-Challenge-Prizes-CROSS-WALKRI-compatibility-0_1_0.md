---
title: Nesta Challenge Prizes Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/cross-walkri/CROSS), WALKRI v0.1.6 (github.com/cross-walkri/WALKRI)
references:
  - Nesta (Challenge Works), Challenge Prizes: A Practice Guide, 2019, https://media.nesta.org.uk/documents/Nesta_Challenges_Practice_Guide_2019.pdf
---

# Nesta Challenge Prizes Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

CROSS and WALKRI together address the Nesta (now Challenge Works) "Challenge Prizes: A Practice Guide" (2019) at the success criteria specification and evaluation field design layer. The guide requires measurable success criteria defined before a prize is launched, baseline analysis, and evaluation of participant and societal outcomes. CROSS's Build obligation mode is the natural structural fit for challenge prizes: it is designed for deliverable-specification obligations where gate passage depends on falsifiable completion criteria rather than process compliance. CROSS's entry specification gate implements the guide's "measurable success criteria defined upfront" requirement. WALKRI ensures that evaluation fields used to assess prize submissions are measurement instruments with explicit criterion intent, operational definitions, and evidence forms.

---

## What the Nesta Challenge Prizes Practice Guide Is

Nesta's "Challenge Prizes: A Practice Guide" (2019) was produced when Nesta operated the Challenge Prize Centre, which has since become the independent organization Challenge Works. The guide consolidates practice from Nesta's work designing and running challenge prizes for the UK government, the Rockefeller Foundation, the Robert Wood Johnson Foundation, and other major funders. It covers the full challenge prize lifecycle: problem definition, prize design, success criteria development, baseline analysis, participant recruitment, evaluation, and societal outcome assessment.

Challenge prizes are a distinct funding mechanism: rather than selecting grantees and funding their work toward a known solution, a prize defines the result to be achieved and awards prizes to anyone who achieves it. This result-first structure means that success criteria must be defined with enough precision to be falsifiable before any participant begins work. A success criterion that depends on reviewer judgment at assessment time is not a prize criterion; it is a grant review criterion. The guide addresses this distinction extensively and provides frameworks for developing criteria that are measurable, unambiguous, and assessable by an independent evaluator.

The guide is used by challenge prize designers in government innovation units, philanthropic foundations, and development finance institutions. Challenge Works continues to use and update its principles in ongoing prize design practice.

---

## Build Obligation Mode: The Natural Fit

CROSS's three obligation modes are Build (deliverable specification), Change (behavior or state change), and Retroactive (retrospective recognition of completed work). Challenge prizes are structurally Build obligations: they specify a deliverable or result to be achieved and award prizes to participants who achieve it by the specified criteria.

The Build mode in CROSS is designed for obligation records where gate passage depends on falsifiable completion criteria applied to a delivered artifact or demonstrated result. The entry specification gate in Build mode locks the completion criteria before any work begins. This is the structural equivalent of the guide's "success criteria defined upfront" requirement: in CROSS Build mode, success criteria are gate-locked at entry and cannot be changed without a formal gate record. A prize that changes its success criteria after launch without a documented rationale is a CROSS gate violation; the gate architecture makes this failure mode visible and formally recorded.

CROSS's four-gate sequence in Build mode maps to the challenge prize lifecycle: the entry specification gate corresponds to prize launch (criteria locked); the progress gate corresponds to mid-competition check-ins (evidence of participant progress); the output gate corresponds to submission review (does the submission meet the completion criteria); and the outcome gate corresponds to post-award evaluation (did the prize achieve the societal outcomes intended). Not all challenge prizes run all four gates; a short-cycle prize may use only entry and output gates. CROSS allows gate configuration per program.

---

## Entry Specification Gate: Measurable Success Criteria Defined Upfront

The guide's most operationally specific requirement is that success criteria must be defined before the prize launches. This requirement has a structural implication: criteria defined before launch cannot depend on comparative assessment of submissions (since submissions do not yet exist) and must be expressed as absolute standards against which any submission can be assessed independently. Criteria that are expressed comparatively ("the best solution submitted") are not measurable upfront criteria; they are selection criteria, which are a different design choice.

CROSS's entry specification gate is the gate that locks the eleven-field indicator specification before any applicant submits. In a challenge prize context, Fields 1 through 5 (name, definition, unit, baseline, target) define what must be demonstrated and at what level. Field 11 (compliance threshold) is the pass/fail criterion: it specifies the level of attainment that constitutes prize qualification, expressed as an absolute standard. The compliance threshold field is the CROSS instrument-layer expression of the guide's falsifiable success criterion requirement.

WALKRI strengthens the entry specification gate for challenge prizes by requiring criterion intent to be stated explicitly before the evaluation fields are published. A prize evaluation rubric is a collection instrument; it collects assessors' judgments about submissions. WALKRI's criterion intent requirement forces the prize designer to state what each evaluation field is measuring and why, before assessors are trained and before submissions are reviewed. This requirement prevents the common prize design failure where evaluation rubrics accumulate criteria that reflect what assessors find interesting rather than what the success criteria require.

---

## Evaluation Fields as Measurement Instruments: WALKRI Application

Prize evaluation involves structured assessment of submissions against defined criteria. The evaluation rubric or scoring framework is a collection instrument; assessors are the collectors. WALKRI's five field requirements apply to prize evaluation rubrics as they apply to any other collection instrument.

The response form requirement is particularly important in the prize context: it specifies what form assessors' responses take (binary pass/fail, scored rubric, ranked ordering) and requires justification for the choice. A rubric that mixes binary criteria with scored criteria without explanation produces data that cannot be aggregated cleanly across assessors. WALKRI's response form requirement makes this design choice explicit before assessors are trained.

The evidence form requirement specifies what independent verification pathway exists for each evaluation field. For challenge prizes, this means: what artifact does the submission provide that allows an independent reviewer to verify the assessor's judgment? Prize submissions that cannot be independently verified after assessment cannot satisfy WALKRI's evidence form requirement without additional specification of the verification pathway.

---

## Structural Mapping Table

| Guide Requirement | CROSS Provision | WALKRI Provision | Coverage |
| :-- | :-- | :-- | :-- |
| Measurable success criteria defined upfront | Entry specification gate; Build obligation mode; compliance threshold (Field 11) as absolute pass/fail standard | Criterion intent requirement for evaluation fields | Structural: gate architecture enforces pre-specification and locks criteria |
| Baseline analysis | Field 4 (baseline) in eleven-field specification | No direct provision | Structural: baseline documented in indicator specification |
| Independent evaluation of submissions | Gate evidence submission structure; evidence form (Field 10) | Evidence form requirement: independent verification pathway required | Structural: gate evidence and WALKRI evidence form together |
| Societal outcome evaluation | Outcome gate; ToC causal architecture linking deliverable to societal effect | No direct provision | Structural: outcome gate is post-award evaluation moment |
| Participant outcome evaluation | Output gate; Field 6 (population scope) | No direct provision | Structural: participant scope documented in indicator specification |

---

## Further Information

CROSS: github.com/cross-walkri/CROSS

WALKRI: github.com/cross-walkri/WALKRI

Nesta Challenge Prizes Practice Guide: https://media.nesta.org.uk/documents/Nesta_Challenges_Practice_Guide_2019.pdf

Challenge Works: challenge.works

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. Build obligation mode, entry specification gate, and WALKRI evaluation field requirements analyzed against Nesta guide requirements. Societal and participant outcome gate mappings documented. |
