---
title: CROSS - Common Reporting Outcome Standards Schema - Assessment Rubric
version: 0.3.1
date: 2026-06-08
license: CC0
status: Working draft. Companion rubric synced to CROSS-common-reporting-outcome-standards-schema-0_5_0.md. Supersedes version 0.2.0.
---

# CROSS: Common Reporting Outcome Standards Schema - Assessment Rubric

Version 0.3.1 | 2026-06-08 | CC0

---

## How to Use This Document

This rubric is the reviewer-facing evaluation tool for applications assessed against the Common Reporting Outcome Standards Schema (CROSS). It is designed to be used during an active review without cross-referencing the full standard. Reviewers who have not read the standard should still be able to complete a well-grounded evaluation using this document alone. This version of the rubric is synced to CROSS version 0.5.0, in which CROSS is declared a domain application of CRAFT (Chains Reveal Attested Falsifiable Truth), the meta-standard for evaluation chain legibility (spec Part XIII receipt). A program that uses this rubric to assess applications against CROSS thereby satisfies CRAFT's conditions for those grant evaluations; the reviewer does not separately apply CRAFT. Where a check below realizes a specific CRAFT requirement, that connection is noted; the note is orientation for a researcher, not an additional step the reviewer performs.

This rubric covers three obligation modes: build obligation, change obligation, and retroactive obligation. Before applying any scored criteria, a reviewer must determine which mode the round operates in and navigate to the correct entry specification gate in Section 2. The mode is declared in the published round specification; it is not determined by the reviewer and is not open to interpretation during review.

The rubric is organized into six sections. Section 1 is a pre-assessment configuration step: the reviewer confirms the mode, the active gates, and the assessment preconditions (including reviewer calibration). Section 2 contains the entry specification gate. Section 2 opens with the entry-gate preconditions (the declarations that must be present before any gate assessment proceeds) and then the mode-specific gate, which is binary. Sections 3 and 4 contain the scored rubric criteria: indicator specification (11 fields) and data quality standards (5 standards). Section 5 covers binary conformance checks that run parallel to scoring. Section 6 specifies the recommendation vocabulary.

All three recommendation categories (Fund, Fund with conditions, Do not fund) depend on the complete evaluation record. A strong indicator score does not override a conformance check failure. A gate failure in Section 2 terminates evaluation before scoring begins.

---

## Section 1: Round Configuration

Before beginning evaluation, confirm the following from the published round specification. Record the findings; they shape which sections of this rubric apply.

**1. Obligation mode.** Which mode does this round operate in?

- [ ] Build obligation: the funded work must produce a specified deliverable
- [ ] Change obligation: the funded work must produce a measurable change in a defined population
- [ ] Retroactive obligation: the application presents evidence of prior demonstrated contribution

**2. Active gates.** Which gates are active in this round's published configuration?

- [ ] Entry specification gate (always active)
- [ ] Progress verification gate(s): how many? ___
- [ ] Completion verification gate
- [ ] Continuation specification gate

**3. Evidence scope and strength at the completion verification gate.** Record the published configuration. This determines the minimum threshold for a Fund recommendation.

Evidence scope: _______________ (output / usage / outcome / impact)

Evidence strength: _______________ (self-report with documentation / third-party verifiable / independent review / independent evaluation)

**4. Infrastructure declaration.** If any gate is configured at independent review level or above, confirm that the infrastructure declaration is present in the round specification before proceeding. A gate at independent review level without a named reviewer, stated qualifications, and published process does not satisfy the conformance requirement. Record any gap here.

> [Note any missing infrastructure declarations, or write "Not applicable" if no gates require independent review]

**5. Reviewer calibration (assessment precondition).** For any gate configured at independent review level or above, confirm that a reviewer calibration exercise was completed before the review window opened and before you, the reviewer, assess any live application. The calibration must have presented the published gate criteria, their criterion intents, and the conformance threshold for each criterion, and must have included at least two worked examples: one application that clearly satisfies the gate criteria and one that clearly does not, each with a documented assessment. Where the panel includes reviewers from more than one institution or context, confirm that calibration included an inter-rater consistency check on the worked examples. Confirm that a calibration record exists naming the reviewers present, the date, and the gate criteria reviewed.

This is a precondition, not a scored criterion. A gate assessment conducted by a reviewer who did not complete calibration does not satisfy the infrastructure declaration for that gate, and the assessment should not proceed until calibration is complete. (This realizes the pre-specified-criteria condition of CRAFT, by keeping the criteria from collapsing into reviewer judgment.)

> [Confirm calibration completed for each gate at independent review level or above, or write "Not applicable" if no gates require independent review]

---

## Section 2: Entry Specification Gate

### Section 2-0: Entry-Gate Preconditions

Before navigating to the mode-specific gate, confirm that the entry-gate preconditions are present. A precondition is not a scored criterion. An entry gate submission that is missing a required declaration is incomplete and is not assessed until the declaration is provided. Where a precondition assessment surfaces a discrepancy (a declared fact that contradicts other evidence in the submission), record it; the spec routes such discrepancies to a structured discrepancy investigation (the spec calls this Block J under a conformant evaluation process).

These preconditions are the declarations the entry specification gate requires of every applicant regardless of mode, plus the conditional declarations that activate for some applicants. Confirm each that applies before proceeding to the mode-specific gate.

**Precondition A: Organizational identity completeness.**

**Reviewer Question:** Are all six required fields of the organizational identity declaration present and complete? The six fields are: legal entity name and jurisdiction; parent organization declaration; affiliated entity disclosure; prior round history; disbursement authority; on-chain identity anchor.

Confirm each field as follows.

- *Legal entity name and jurisdiction:* the name of the natural person or registered organization exactly as it appears in the jurisdiction of registration, plus that jurisdiction. A project name, display name, or code-repository organization name does not satisfy this field unless it is also the legal name. Where no legal entity exists, confirm the applicant states this explicitly and names the individual who assumes personal responsibility for the obligation.
- *Parent organization declaration:* whether the applicant operates under or is affiliated with a larger organization, network, or chapter structure, with the parent named where one exists, and the relationship described. Silence is not acceptable where an affiliation is publicly documented or where the applicant's name, brand, or personnel overlaps a known larger organization.
- *Affiliated entity disclosure:* any other organization, project, or entity sharing the applicant's name, brand, domain, key personnel, or codebase. Non-disclosure of a publicly documentable affiliation is a conformance failure; disclosure is not.
- *Prior round history:* whether the applicant or any substantially overlapping entity has applied to this program in prior rounds, under what name, and with what outcome. This field catches serial rebranding after a prior rejection.
- *Disbursement authority:* see Precondition B.
- *On-chain identity anchor:* the canonical wallet address by which the applying entity is identifiable across blockchain programs and grant databases. Non-disclosure of an on-chain address publicly associated with the applicant's identity in any grant database is a conformance failure equivalent to non-disclosure in the affiliated entity field.

| Finding | Action |
|---|---|
| All six fields present and complete | Precondition met. Proceed. |
| One or more required fields absent | Submission incomplete. Do not assess. Record which fields are missing. |
| A declared field is contradicted by other evidence in the submission or by independent evidence (for example, an undisclosed affiliation that is publicly documented) | Record as a material discrepancy and route to structured discrepancy investigation. Non-disclosure of a publicly documentable fact is treated more seriously than the fact itself. |

**Precondition B: Disbursement authority.**

**Reviewer Question:** Does the organizational identity declaration name the person or persons with legal authority to receive grant funds on behalf of the applying entity and approve their deployment, in one of the three recognized states?

The three states are: individual (one named person with full authority); collective (shared authority through a named mechanism, with current key holders named and the quorum threshold stated); and delegated (authority by role, with the current holder named and the transfer mechanism stated). For a decentralized autonomous organization applicant without a legal wrapper, confirm that the declaration names the controlling wallet address and the decision-standing mechanism, with current token holders above the materiality threshold named where possible.

| Finding | Action |
|---|---|
| Disbursement authority declared in one of the three states with the required supporting detail | Precondition met. |
| Declaration absent | Entry gate submission is incomplete. Do not assess until provided. |
| State declared but required detail absent (for example, "collective" without named key holders or quorum threshold) | Record the gap. The declaration is incomplete until the detail is provided. |

**Precondition C: Sufficiency architecture coherence.**

**Reviewer Question:** Are all five elements of the sufficiency architecture declaration present, and do they form a coherent account of where this grant fits in the applicant's resource position? The five elements are: scope declaration, sufficiency position, portfolio context statement, grant contribution statement, and revenue architecture declaration.

Confirm each.

- *Scope declaration:* the specific program, sub-entity, or aspect of the applicant's work this application covers, stated clearly enough that a reviewer could determine what falls within it and what falls outside. Where the application covers the entire operation, confirm this is stated explicitly.
- *Sufficiency position:* one of four declared positions at the declared scope (not at the entity level overall): critical gap, partial, approaching, or surplus.
- *Portfolio context statement:* how other funding sources address other scopes of the entity's work. This is not concurrent funding disclosure (which covers other funding for the same scope). Silence about other funding sources in an entity with multiple programs requires explicit explanation.
- *Grant contribution statement:* what specific gap at the declared scope this grant would close, and the sufficiency position at that scope after the grant.
- *Revenue architecture declaration:* one of four types (grant-only, fee-for-service, commercial, or hybrid). For grant-only, the declaration confirms no commercial revenue model exists. For fee-for-service, commercial, and hybrid, the declaration activates the additionality delineation requirement assessed in Check 1-A: the applicant must identify which portion of the work or budget commercial revenue does not cover.

**Corroborating evidence.** The sufficiency position declaration requires at least one piece of corroborating evidence from a source outside the applicant's control (publicly accessible treasury data, grant history from a named external database, or disclosed revenue figures from a named independent source). A declaration with no corroborating evidence is accepted at self-report evidence strength only. Where the program configures the sufficiency architecture declaration at independent review evidence strength or above, corroborating evidence is required before assessment proceeds. Where no public corroborating evidence exists (for example, a recently formed entity with no funding history), confirm the applicant states this explicitly and explains why the declared position is reasonable.

| Finding | Action |
|---|---|
| All five elements present; coherent; corroborating evidence present where required | Precondition met. The declaration supports additionality, attribution, and the assessment of how this grant fits the broader funding architecture. |
| One or more elements absent | Submission incomplete. Do not assess until provided. |
| Elements present but internally incoherent (for example, a surplus sufficiency position paired with a critical-gap grant contribution statement) | Record the incoherence; request clarification before proceeding to scoring. |
| Sufficiency position declared but no corroborating evidence where the program requires it at independent review strength or above | Assessment does not proceed until corroborating evidence is provided. |

**Precondition D: Public benefit mechanism and access condition.**

This precondition applies in every program where the eligibility criteria include any public goods basis. Where a public goods claim appears in the eligibility section but no public benefit mechanism and access condition declaration is present, the submission is incomplete and is not assessed until the declaration is provided.

**Reviewer Question:** Does the applicant declare (1) which of the four mechanism types the public benefit claim rests on, (2) the access conditions under which that mechanism delivers benefit to the stated population, specified precisely enough that an independent reviewer could confirm them without contacting the applicant, and (3) whether the access conditions are current at application, will be achieved at the completion gate, or both?

The four mechanism types and their required access-condition content are:

- *Output production:* an SPDX license identifier and the location of the license file. A copyright notice that permits free viewing without granting modification or redistribution rights does not satisfy this access condition. A "source available" or "fair code" license restricting commercial use does not satisfy it unless the program's published round configuration explicitly accepts such licenses and states the accepted SPDX identifiers. A future licensing commitment without a current license does not satisfy the access condition at the entry gate; the applicant must specify when the license will be applied and confirm this at the completion gate.
- *Access provision:* an access mechanism, a cost structure, and a non-excludability mechanism.
- *Condition change:* a FROM state and a population definition.
- *Ecosystem shift:* a named causal pathway and a co-factor list.

The mechanism type declared at entry constrains the evidence scope required at the completion gate: output production commits to output evidence at minimum; access provision commits to usage evidence; condition change commits to outcome evidence; ecosystem shift commits to a documented impact contribution argument. A declared mechanism that the evidence scope available at the completion gate cannot support is a misrepresentation in the entry specification.

| Finding | Action |
|---|---|
| Mechanism type, access condition content (matching the type), and currency status all present | Precondition met. |
| Public goods claim present in eligibility but declaration absent | Submission incomplete. Do not assess until provided. |
| Mechanism type declared but the access condition content does not match the type (for example, output production declared with no SPDX identifier) | Record the gap; the declaration is incomplete until corrected. |
| Mechanism type contradicts the applicant's own description of the work (most commonly: output production claimed while the work is described as standard all-rights-reserved copyright) | Material discrepancy. Route to structured discrepancy investigation. This contradiction cannot be resolved by reviewer judgment; the applicant must address it before assessment proceeds. |

**Precondition E: Development stage consistency.**

The development stage dimension is active in all rounds. Confirm the development stage declaration is present and consistent with the evidence elsewhere in the submission.

**Reviewer Question:** Does the applicant declare one of five development stages, explain why the work is at that stage rather than an adjacent one, and provide at least one piece of evidence from a source outside their control confirming the declared stage? Is the declared stage consistent with the evidence provided and with the round's stage-targeting configuration?

Stage evidence expectations: Stage 1 (proof of concept) provides output evidence of the existing artifact; Stage 2 (early adoption) provides usage evidence from at least one named external user; Stage 3 (growth) provides independently verifiable adoption data with a trend; Stage 4 (established infrastructure) provides 12 months of sustained usage data from sources outside the team; Stage 5 (retroactive recognition) provides prior contribution evidence in the entry submission.

Confirm two consistency relationships. First, the declared stage must match the evidence: a Stage 1 declaration paired with independent usage evidence is either a misrepresentation of stage or an understatement to investigate; a Stage 3 or higher declaration with no independently verifiable adoption data is a discrepancy to investigate. Second, the declared stage constrains the obligation mode: a Stage 1 applicant committing to a change obligation must provide a FROM state and a population baseline at entry, coherent only if the Stage 1 artifact is specifically designed to measure against an existing condition; a Stage 4 applicant selecting a build obligation must specify what new functionality is added beyond sustained operation, and declaring Stage 4 with a build obligation for what amounts to continued maintenance is a framing misrepresentation.

| Finding | Action |
|---|---|
| Stage declared, justified, evidenced from outside the applicant's control, consistent with both the provided evidence and the obligation mode; within the round's stage-targeting scope | Precondition met. |
| Declaration absent | Submission incomplete. Do not assess until provided. |
| Declared stage not supported by the provided evidence, or inconsistent with the obligation mode | Material discrepancy. Route to structured discrepancy investigation. |
| Declared stage outside the round's published stage-targeting scope | Record; stage targeting is a published program design decision, so a stage outside scope is an eligibility matter for the program, not a reviewer judgment. |

**Precondition F: Decision-standing structure and Continuity Capacity.**

This precondition is active for grants above a funder-defined size threshold, grants producing ongoing infrastructure with continuing operational requirements, and any application where the applying entity has a single named primary contributor with no documented backup capacity. For programs funding infrastructure maintenance or sustained service delivery, it is always active.

**Reviewer Question:** Where this precondition is active, does the applicant declare one of three continuity-resilience states (single, partial, or resilient) with supporting evidence? For a single-point-of-failure (single) state, does the declaration name the person on whom continuation depends and state what would happen to active grants and funded deliverables if that person became unavailable?

| Finding | Action |
|---|---|
| Resilience state declared with supporting evidence; single-point-of-failure declarations name the person and state the continuity consequence | Precondition met. A single-point-of-failure disclosure is not a disqualifier; it is a material fact affecting the sustainability assessment at the continuation gate and the funder's configuration of completion gate conditions. |
| Precondition active but declaration absent | Submission incomplete for this dimension. Record. |
| Single state declared but the person is not named or the continuity consequence is not stated | Declaration incomplete until provided. |

**Precondition G: Obligation fulfillment record.**

This precondition activates where any of the following apply: the applicant has received prior grants from this funder in any prior round; the applicant cites prior work as evidence of capability at the entry gate; or the applicant's prior round history includes unresolved external milestones or open gate conditions.

**Reviewer Question:** Where this precondition is active, does the obligation fulfillment record document, for each prior grant from this funder: what was committed at the entry gate of that prior round (the deliverable specification, the FROM-TO state, or the contribution evidence, as appropriate to that round's mode); what was produced during the grant period (the artifact, the measured change, or the verified contribution, with a publicly accessible link); and whether the commitment was fulfilled, partially fulfilled, or unfulfilled, with the applicant's explanation where fulfillment was not complete?

| Finding | Action |
|---|---|
| Record present and complete for each prior grant from this funder | Precondition met. An unfulfilled prior obligation is not automatically disqualifying; it is a disclosed fact affecting the track record assessment at the continuation gate and may be addressed by a written explanation. |
| Precondition active but record absent | Submission incomplete. Do not assess until provided. |
| A prior grant, milestone, or unresolved obligation is discovered through research (including the funder-side query of public attestation sources) but is not disclosed in the record | Material discrepancy. Non-disclosure of a prior failure is treated more seriously than the failure itself. |

**Precondition H: Prior work attribution.**

This precondition activates for any applicant in any mode who cites prior work as evidence of capability, track record, or past contribution: build-obligation applicants citing prior deliverables, change-obligation applicants citing prior outcomes as a baseline or established methodology, and retroactive-obligation applicants whose entire submission consists of prior work.

**Reviewer Question:** For each piece of prior work cited, does the prior work attribution statement address all three questions?

- *Entity of performance:* under which legal entity or organizational context was the cited work performed? If performed as an employee, contractor, or contributor to an organization that is not the applying entity, that organization must be named. If performed under the applying entity's own resources, that must be stated explicitly.
- *Applicant's relationship at the time:* what was the applicant's role in the entity under which the work was performed, and what is the current status of that relationship? Both the relationship at the time of creation and the relationship at the time of application must be stated.
- *Current ownership and access:* who currently holds the intellectual property rights, who controls the deployment or codebase, and who has the relationship with any users cited as evidence of impact? If the applying entity does not hold the rights, control the deployment, or have the user relationship, this must be stated.

The prior work attribution statement is an adverse signal disclosure requirement. An applicant who cannot truthfully complete it for cited prior work has surfaced a misrepresentation in the core evidential basis of the application.

| Finding | Action |
|---|---|
| Statement present and addresses all three questions for each piece of cited prior work | Precondition met. |
| Prior work cited but no attribution statement, or the statement omits one of the three questions for any cited work | Submission incomplete for this evidence. Do not rely on the cited work as track record until the statement is complete. |
| The completed statement reveals that the track record rests on work performed under a different entity without that entity's knowledge or endorsement of the application | Adverse signal. The applicant is claiming responsibility for outcomes they did not control. Record and route to the adverse signal provisions (Check 2). |

---

### Section 2-1: Mode-Specific Entry Specification Gate

Confirm the entry-gate preconditions in Section 2-0 are met, then navigate to the sub-section that matches the obligation mode confirmed in Section 1. Complete the gate assessment before opening any scored rubric sections. A gate failure terminates evaluation; do not apply the indicator rubric to a gate failure.

The mode-specific gate also incorporates the served-population check below, which applies wherever the round's eligibility rests on serving a defined population.

**Served-population risk-bearer floor (apply at this gate and at every subsequent gate where the round's eligibility rests on serving a defined population).**

The parties who bear loss when a round's evaluation misjudges are the applicant whose work may be misclassified, the funder whose resources may be misdirected, and the served population: the people a funded intervention is meant to serve, who bear loss when the round funds work that does not reach them or excludes work that would have served them. The spec names the served population a risk-bearer carried through every gate, not validated only at entry (spec Part II beneficiary dimension; this realizes CRAFT Condition 1 risk-bearer identification as a carried requirement).

**Reviewer Question:** Where the round's eligibility rests on serving a defined population, does the gate determination record show that the served population's exposure was considered, not only that the population was named at entry?

At the entry gate, the beneficiary engagement and beneficiary validation dimension performs part of this: in change-obligation rounds the claimed FROM state must be validated by parties outside the applicant's control, and in build-obligation rounds the claimed need for the deliverable must be validated by at least one party outside the applicant's organization who would use or benefit from it. Confirm that this outside-the-applicant validation is present where the dimension is active.

At the completion verification gate, confirm that the determination and the unintended outcomes disclosure additionally consider whether the served population bears exposure the round has not surfaced: work recorded as delivered that does not reach them, or effects on them that the declared indicators do not capture.

| Finding | Action |
|---|---|
| The gate determination record shows the served population's exposure was applied as a consideration (the claimed need validated from outside the applicant at entry; at completion, exposure beyond what the declared indicators capture considered) | Floor met. Record the consideration in the determination. |
| The served population was named at entry but the determination record does not show its exposure was considered | Floor not met. The determination record must show the consideration was applied, not merely that the population was named. Return the determination for the consideration to be applied and recorded. |

Note: this floor is a named consideration each gate is checked against. It does not, on its own, require a standing channel through which the served population raises concerns during the grant period; such a channel is a separate configuration a funder may add.

---

### Section 2A: Entry Specification Gate - Build Obligation

**What the gate is asking.** Can the applicant name a falsifiable deliverable with independently verifiable completion criteria?

A falsifiable deliverable is an artifact, product, or documented output whose existence and quality can be confirmed by a reviewer who did not commission the work. Completion criteria are independently verifiable when a reviewer with access to the submitted artifact, and no additional information from the applicant, could determine whether those criteria are met.

This gate does not ask whether the applicant has already started building, whether the deliverable will be widely adopted, or whether the applicant's approach is the best available. It asks only whether the commitment is specific enough to evaluate at the end of the grant period.

**Direction specification without deliverable.** The primary failure mode in build-obligation rounds is offering a direction or vision in place of a deliverable specification. "Making DeFi more transparent" is a direction. "A reporting module that produces a human-readable summary of fees collected by any ERC-4626 vault, published as an open-source library under the MIT license, with at least one deployed instance on Ethereum mainnet, documented with a usage example and test suite" is a deliverable. The difference is testability: a reviewer at grant end can confirm whether the second was delivered; the first cannot be verified or falsified.

**Underspecified completion criteria.** A deliverable is named but the completion criteria are too vague for independent verification. "A working prototype" specifies a form but not a standard. "A prototype that successfully executes the three functions listed in the specification document, as demonstrated in a public recording or live session, with accompanying test results from the specified test suite" specifies a verifiable standard. The rubric can be applied to an application that passes the gate but has underspecified criteria; it will score 2 or lower on Fields 10 and 11.

**Gate finding options.**

Gate passes: document "Gate passes: applicant names [deliverable, paraphrased] with completion criteria sufficient for independent verification: [describe what verification would look like]." Proceed to Section 3.

Gate fails: document "Gate fails: [describe what was offered instead of a falsifiable deliverable or verifiable completion criteria]." Close the evaluation record. Distinguish which failure type applied so the applicant receives the correct corrective signal.

---

### Section 2B: Entry Specification Gate - Change Obligation

**What the gate is asking.** Can the applicant name the FROM state as a specific measurable condition in a defined population?

A FROM state is specific when it names a condition. A condition describes an observable state that exists in the world and can be measured. A category describes a type of problem without grounding it in an observable measurement.

A FROM state that passes the gate: "96 to 99 percent network reachability drops for users in Iran during government-imposed shutdowns, as measured by Open Observatory of Network Interference probe data from 2023 to 2025." This names a measurable quantity, a defined population, a triggering condition, a data source, and a time period. A reviewer can verify that this condition exists.

A FROM state that fails the gate: "There is a lack of privacy tools for people in repressive contexts." This names a category and a vague population. Neither is measurable. A reviewer cannot verify whether this condition exists or how severe it is.

**Two gate failure types in change-obligation rounds.** These are the Frame Language diagnostic categories D2 and D1. They look superficially similar during review but have different implications for the applicant.

Class D2 (values aspiration without conditions): the application offers values language, community commitments, or a mission statement in place of a diagnosis. When asked for a specific FROM state, a D2 application produces more values language because no diagnostic work preceded the application. D2 applications cannot produce a plausible FROM state on request. Gate failure is immediate. The applicant has not performed a problem diagnosis; the path to resubmission is to do the diagnostic work before applying again.

Class D1 (canonical vocabulary without structural grounding): the application uses technically correct vocabulary and names something that resembles a problem diagnosis. A specific FROM state can be articulated. The gate passes. The failure appears at the rigor tier: the indicators claimed are not supported by a sourced data methodology, the baseline is undocumented, or the construction methodology cannot be replicated. A D1 application may score 2s and 1s across the indicator rubric after passing the gate. Treating a D1 failure as a gate failure produces false negatives; the applicant has done diagnostic work and deserves a specific rigor-tier finding about what specification is missing.

**Application timing is not the diagnostic.** A team that built something before the grant round opened is not automatically exhibiting a gate failure. They can name the FROM state precisely because they built the solution to address it. Application timing tells the reviewer when the applicant sought funding; it does not reveal whether a diagnosis was performed.

**Build nested inside change is valid.** An application that describes what it will build while also naming a qualifying FROM state has not failed the change-obligation gate. The build is the mechanism; the change specification is intact. The gate question is whether a FROM state can be named, not whether the applicant also commits to producing an artifact. Build becomes the failure mode when it has replaced the change specification: the applicant names a deliverable but cannot produce a FROM state because the problem was never diagnosed.

**Gate finding options.**

Gate passes: document "Gate passes: applicant names [specific condition, verbatim or paraphrased] in [specific population] with [named source or evidence]." Proceed to Section 3.

Gate fails: document "Gate fails: [describe what was offered instead of a FROM state specification, and note whether the failure type is D2 or D1-equivalent]." Close the evaluation record. Do not apply the indicator rubric.

---

### Section 2C: Entry Specification Gate - Retroactive Obligation

**What the gate is asking.** Does the applicant present evidence of prior contribution meeting the program's published threshold criteria?

In retroactive rounds, the gate question is not about diagnosis or deliverable specification. It is about whether the evidence presented clears the program's published minimum threshold for what constitutes a qualifying prior contribution. The published rubric from the round specification is the instrument; the gate confirms whether the application contains the required evidence in the required form.

**What the reviewer is assessing.** The application must contain: a description of what contribution was produced, the period during which it was produced, evidence of who is using or has benefited from it that is accessible from sources outside the applicant's control, and a concurrent funding disclosure covering any prior awards for the same or overlapping work. If any of these is absent, the entry specification gate fails.

**The rubric dependency.** Unlike build and change obligation, retroactive applications are assessed primarily against the program's published rubric rather than the CROSS indicator specification rubric in Section 3. The Section 3 rubric applies if the program has configured additional indicator-based reporting for retroactive applications (for example, a forward commitment combined with an indicator specification). If no indicator specification is required, proceed from this gate to Section 5 (conformance checks) and Section 6 (recommendation framework), using the program's published rubric for the substantive scoring.

**Gate finding options.**

Gate passes: document "Gate passes: applicant presents evidence of prior contribution in [described form] covering [described period], with evidence of external use [describe source]." Proceed to applicable scoring (program rubric, Section 5, Section 6).

Gate fails: document "Gate fails: [describe what is absent from the application: no contribution description, no period, no independently accessible evidence of use, or no concurrent funding disclosure]." Close the evaluation record.

---

## Section 3: Indicator Specification Rubric

### Overview

CROSS requires applicants to self-specify their outcome indicators. The rubric in this section assesses the quality of the applicant's self-specified indicators across 11 required fields. Each field is scored on a 1-4 scale using the definitions below.

**Score 4 (meets Standard):** The field is complete, specific, and independently verifiable. An independent reviewer with access to the stated sources could confirm the field content without contacting the applicant.

**Score 3 (minor Gap):** The field is substantially complete. One specific, addressable gap is present. The gap is resolvable without structural redesign of the indicator. A score of 3 does not trigger a condition; reviewers note it in the evaluation record.

**Score 2 (conditional):** The field has a significant gap that must be resolved before disbursement. A score of 2 generates a condition. The condition must be specific, verifiable, and time-bounded. An application with one or more 2s cannot receive a Fund recommendation; it receives Fund with conditions if all other criteria are met.

**Score 1 (fails Standard):** The field is absent, generic, or unverifiable. An application with any indicator field scored 1 is ineligible for funding without resubmission. A score of 1 on the primary indicator produces a Do not fund recommendation.

Where multiple indicators are specified, each indicator is scored independently. The recommendation reflects the weakest primary indicator.

In retroactive obligation rounds where no indicator specification is required by the program configuration, Sections 3 and 4 do not apply. See Section 2C.

---

### Field 1: Indicator Name

**Reviewer Question:** Is a short, descriptive label present? Is it distinguishable from generic category labels?

| Score | Criterion |
|---|---|
| 4 | Name is present and distinguishable from generic category labels. It would be recognizable as referring to this specific indicator in a cross-funder comparison. |
| 3 | Name is present but is a category label that could apply to materially different operational definitions. The operational definition field compensates. |
| 2 | Name is absent or is a copy of the program area eligibility criterion rather than an indicator label. |
| 1 | No indicator name is present. |

---

### Field 2: Rationale for Indicator

**Reviewer Question:** Does the applicant explain why this indicator was chosen over available alternatives? Is the diagnostic reasoning that preceded tool selection visible?

Rationale is required. An applicant who cannot articulate why they selected a particular indicator over obvious alternatives has not engaged seriously with whether the measurement instrument is valid.

| Score | Criterion |
|---|---|
| 4 | Rationale names at least one alternative indicator considered and explains why the chosen indicator better matches the intervention's claim. The reasoning demonstrates that selection was a deliberate decision. |
| 3 | Rationale explains why the chosen indicator is appropriate but does not name alternatives considered. The reasoning is plausible and specific, not generic. |
| 2 | Rationale is present but circular (e.g., "we chose transaction volume because we measure transactions"). No diagnostic reasoning is visible. |
| 1 | Rationale is absent. |

---

### Field 3: Measurement Form and Evidence Classification

**Reviewer Question:** Has the applicant named the measurement form in plain language, with enough specificity to classify it against the three evidence classification axes? Is the stated measurement form consistent with the construction methodology in Field 5?

This field replaces the constrained four-option data type list from version 0.1.0. The applicant now names the measurement form in plain language rather than selecting from a list. Reviewers classify the stated form against three axes for data quality assessment purposes. The applicant is not required to use the axis vocabulary; the reviewer applies the classification.

**Axis 1: Source type.** Where does the evidence originate?
- On-chain verifiable: accessible from public blockchain data with a named contract or address
- Off-chain verifiable: accessible from public sources outside the blockchain (public code repository, published report, named application programming interface)
- Qualitative/narrative: documented through structured narrative, interview data, or artifact review requiring a human evaluator

**Axis 2: Measurement form.** How is the result expressed?
- Quantitative: expressed as a number, proportion, rate, currency amount, or duration
- Ordinal: expressed as a position on a defined ordered scale
- Binary: expressed as met or not met against named completion criteria
- Qualitative: expressed as a documented condition, verified artifact, or narrative record assessed against named criteria

**Axis 3: Aggregation type.** How do period values relate to each other?
- Cumulative: values sum correctly across reporting periods; see Field 6 for the applicant's explicit designation
- Non-cumulative: values describe a state at a point in time; summing across periods is a construction error

**For Build-obligation Indicators:** the measurement form is typically binary or qualitative. The measurement form declaration specifies what done looks like with enough precision that a reviewer who did not commission the work could verify it independently.

**For Change-obligation Indicators:** the measurement form is typically quantitative or ordinal. The declaration must include the unit of measurement and the direction of desirable change.

| Score | Criterion |
|---|---|
| 4 | The applicant names the measurement form in plain language with enough specificity to classify against all three axes without inference. The classification is internally consistent with the construction methodology in Field 5. |
| 3 | The measurement form is named but requires modest inference to classify. The classification is possible; the applicant has not made one or two axes explicit. Internally consistent with Field 5. |
| 2 | The measurement form is named but the classification along at least one axis conflicts with the construction methodology (e.g., described as quantitative but the methodology produces only binary results), OR the description is so general that axis classification cannot be determined. |
| 1 | No measurement form description is present. |

**On-chain verification check (apply when the primary deliverable is a smart contract, protocol, or on-chain system).** Before applying the Field 3 scores above, confirm whether the obligation object is a contract's behavioral properties rather than discrete outputs or a published artifact. If yes, the indicator must additionally contain four named sub-fields: invariant specification, verification method, verification artifact, and failure surface. Assess these as follows.

**Reviewer Question:** Is an invariant specification present? Is the verification method named? Is the verification artifact a type that an independent reviewer can access without contacting the applicant (a public audit report, a public proof artifact, or a named contract address and query against public chain data)?

| Finding | Action |
|---|---|
| All four sub-fields present; verification artifact is independently accessible | Apply Field 3 score normally. No additional condition. |
| Invariant specification present but verification method or artifact is absent | Score Field 3 at 2. Generate a condition: applicant must name an independent verification instrument before disbursement. |
| Sole verification instrument is an applicant-controlled test suite with no independent instrument | Score Field 3 at 1. This is an integrity standard failure. The integrity standard (Standard 2, Section 4) requires at least one evidence source independent of the applicant. |
| No on-chain behavioral indicator is present despite the primary deliverable being a contract or protocol | Score Field 3 at 1 on the behavioral indicator. This is a construction error, not a missing field. The applicant has specified an output indicator where a behavioral indicator is required. |

Note: applicant-controlled test suites and private monitoring dashboards may appear as supplementary evidence. They do not satisfy the minimum verification requirement as the sole instrument for any indicator where the obligation object is a contract's behavioral properties.

---

### Field 4: Operational Definition

**Reviewer Question:** Are all four required sub-components present: inclusion criteria, exclusion criteria, unit of analysis, and at least one edge case determination?

| Score | Criterion |
|---|---|
| 4 | All four sub-components are present and specific: inclusion criteria state what qualifies as one instance; exclusion criteria state what the indicator explicitly does not count; unit of analysis names the entity being counted or assessed; at least one edge case shows how an ambiguous instance is resolved. |
| 3 | Three of four sub-components are present. The missing sub-component is restorable without redesigning the indicator. Edge case determination is most commonly absent. |
| 2 | Two of four sub-components are present. The indicator can be understood in principle but cannot be replicated without applicant clarification. |
| 1 | Operational definition is absent or consists entirely of the indicator name restated. No sub-components are identifiable. |

---

### Field 5: Construction and Aggregation Methodology

**Reviewer Question:** Is the construction methodology detailed enough that an independent reviewer with access to the stated data source could replicate the result, without contacting the applicant?

For build-obligation indicators: the construction methodology specifies how completion is determined, who performs the verification, and by what process.

For change-obligation indicators: the standard data construction methodology applies (formula or counting rule, partial data handling, sub-unit aggregation).

| Score | Criterion |
|---|---|
| 4 | The formula or counting rule (or, for build indicators, the completion determination process) is stated explicitly. Partial data handling is specified. Aggregation from sub-units to project level is described. An independent reviewer could execute the methodology given the stated source. |
| 3 | The formula or completion process is stated but one secondary element (partial data handling or aggregation) is absent. Replication is possible with minor inference. |
| 2 | The methodology names the data source and describes the result category but does not specify a counting rule or completion determination process. Replication requires significant applicant clarification. |
| 1 | No construction methodology is present. The result is asserted without any described production process. |

---

### Field 6: Cumulative or Non-Cumulative

**Reviewer Question:** Has the applicant designated the indicator as cumulative or non-cumulative? Does the target calculation match the designation?

Note: this field is primarily relevant for change-obligation and build-obligation indicators that involve counting over time. Binary completion criteria (did or did not ship the deliverable) are not subject to the cumulative/non-cumulative distinction; mark as not applicable and score 4 for build-obligation binary indicators.

| Score | Criterion |
|---|---|
| 4 | Designation is present and correct. The target is expressed consistently: a cumulative indicator has a life-of-grant total target; a non-cumulative indicator has a target status at grant end, not a sum of period targets. |
| 3 | Designation is present and correct. The target is expressed in the right form but lacks a per-period breakdown expected given the reporting frequency. Minor gap only. |
| 2 | Designation is present but the target calculation is internally inconsistent with it (treating a non-cumulative indicator as cumulative, or vice versa). |
| 1 | Designation is absent. |

---

### Field 7: Disaggregation

**Reviewer Question:** Are disaggregation categories named? Is the applicant aware that committed categories may be supplemented but not removed without committee approval?

| Score | Criterion |
|---|---|
| 4 | Disaggregation categories are named. The applicant acknowledges that committed categories may be supplemented but not removed without committee approval. |
| 3 | Disaggregation categories are named but no acknowledgment of the ratchet constraint is present. The categories are clear and applicable. |
| 2 | Disaggregation categories are stated at a level of generality that does not permit actual disaggregation (e.g., "by region" without specifying which regions). |
| 1 | No disaggregation categories are named. |

---

### Field 8: Data Source and Collection Method

**Reviewer Question:** Is the named source independently accessible? Is the collection method described? Does any evidence source independent of the applicant appear?

For build-obligation indicators: the data source for completion verification is the named artifact itself plus the named party who will confirm it meets the completion criteria.

| Score | Criterion |
|---|---|
| 4 | The data source is named specifically (contract address, named public application programming interface endpoint, named third-party platform, named institutional partner, named survey instrument, or named artifact with named verifying party). The collection method is stated. The source is independently accessible. |
| 3 | The source is named but access requires a process not described (e.g., "data from our partner organization" without naming the organization or the access method). |
| 2 | The source is a category rather than a named source. |
| 1 | No data source is named. |

---

### Field 9: Data Cost Estimation

**Reviewer Question:** Has the applicant attested that data collection is feasible within the project budget?

| Score | Criterion |
|---|---|
| 4 | Applicant attests to feasibility. Approximate cost is stated (or confirmed as zero with source named). The source of funding for collection within the project budget is identified. |
| 3 | Applicant attests to feasibility and confirms free access to the data source, but no budget line or cost estimate is provided. Adequate for free sources; minor gap for paid sources. |
| 2 | Applicant names a data source but makes no attestation of feasibility or cost. |
| 1 | No data cost estimation or feasibility attestation is present. |

---

### Field 10: Baseline (FROM State)

**Reviewer question and mode-specific assessment.**

**For Change-obligation Indicators:** Is the FROM state specific, measurable, and sourced? Does it express the same unit and type as the indicator's operational definition?

| Score | Criterion |
|---|---|
| 4 | Baseline is specific (a named value or condition), measurable (expressed in the units of the operational definition), and sourced (the source is named and independently accessible). |
| 3 | Baseline is specific and measurable but the source is named at a category level rather than a specific source. |
| 2 | Baseline is directional rather than specific (e.g., "currently low adoption"), or the baseline and target are expressed in different units, or the baseline is asserted without any source. |
| 1 | Baseline is absent. The TO state target appears without any FROM state reference. |

**For Build-obligation Indicators Where The Coordinating Party Engagement Dimension Is Activated:** Is the documented current absence or inadequacy of the deliverable present, with named evidence?

| Score | Criterion |
|---|---|
| 4 | The gap the deliverable addresses is documented with specific evidence: a named party outside the applicant's organization who has confirmed the need, a named existing tool's limitation, or a named data source confirming the gap. |
| 3 | The gap is described with reference to a named source or party but the evidence is indirect. |
| 2 | The gap is asserted by the applicant without independent evidence. |
| 1 | No evidence of the need for the deliverable is present. |

**For Build-obligation Indicators Where The Coordinating Party Engagement Dimension Is Not Activated:** Score 4 for any reasonable plain-language statement of what problem or gap the deliverable addresses. This dimension is advisory at this level.

**For Retroactive Obligation Indicators:** Is the documented state of the prior contribution at the time the award period begins present, with named evidence of use?

Apply the change-obligation scoring logic to the evidence of prior contribution: is it specific, does it name a period and source, and is the source independently accessible?

---

### Field 11: Target (TO State)

**Reviewer question and mode-specific assessment.**

**For Change-obligation Indicators:** Is the target expressed in the same units as the baseline? Is it consistent with the cumulative/non-cumulative designation? Is it specific enough to be verifiable?

| Score | Criterion |
|---|---|
| 4 | Target is expressed in the same units as the baseline and operational definition. It is expressed correctly for the cumulative/non-cumulative designation. It is a specific value or condition, not a directional aspiration. |
| 3 | Target is specific and in the correct units but does not account for all reporting periods where sub-targets are expected. Minor gap only. |
| 2 | Target is directional rather than specific ("increase user adoption"), or units differ from the baseline, or the designation mismatch noted in Field 6 causes internal inconsistency. |
| 1 | Target is absent. |

**For Build-obligation Indicators:** Is the completion criteria clear enough that a reviewer who did not commission the work could verify whether it was met? Do the criteria correspond to the measurement form stated in Field 3?

| Score | Criterion |
|---|---|
| 4 | Completion criteria are stated with enough specificity that an independent reviewer could verify them. The criteria name what must be true (not just what will be built). The criteria correspond to the measurement form in Field 3 (binary criteria for binary form; artifact description for qualitative form). |
| 3 | Completion criteria are present and verifiable in principle but one element of specificity is missing (e.g., "deployed on mainnet" without naming the contract or confirming public accessibility). |
| 2 | Completion criteria are present but too vague for independent verification (e.g., "a working prototype" without specifying what working means or how it will be demonstrated). |
| 1 | No completion criteria are present. |

**For Retroactive Obligation With A Forward Commitment Configured:** Is the forward commitment specific enough to verify at the close of the commitment period?

Apply the build-obligation scoring logic to the forward commitment criteria.

---

## Section 4: Data Quality Standards Assessment

The five data quality standards apply to all evidence claims in the application across all obligation modes. They are assessed as pass/conditional/fail for each standard, separately from the 1-4 indicator field scores. A conditional finding generates a condition equivalent to a score of 2 on an indicator field. A fail finding produces a Do not fund finding for that standard.

In retroactive obligation rounds where the program has not configured indicator-based reporting, assess the data quality standards against the contribution evidence presented in the entry specification. Sections 4's standards still apply to the quality of that evidence.

---

### Standard 1: Validity

**Assessment Question:** Could I, with access to the stated data source and the stated construction methodology, confirm that this indicator measures what the applicant claims it measures?

For build-obligation rounds: is there a documented logical chain from the stated completion criteria to the deliverable being what the applicant says it is?

**Common Failure Mode:** A macro-level adoption metric (ecosystem-wide transaction volume, protocol total value locked) is claimed as evidence of a specific project's contribution. The validity failure is the undocumented causal claim connecting the project's work to the metric's movement.

**Finding Options:** Pass, Conditional (a specific gap in the causal documentation can be resolved before disbursement), or Fail (the indicator is structurally disconnected from the claimed result and the problem is not correctable without redesigning the indicator).

---

### Standard 2: Integrity

**Assessment Question:** Does any evidence for this application's claims originate from a source independent of the applicant?

For all modes: data collection and reporting must be separated from the actor who benefits from the results. Applicant-controlled dashboards, internal databases, and self-reported results without named independent corroboration do not satisfy this standard on their own.

For build-obligation rounds: the named verifying party in Field 8 (who will confirm the deliverable meets the completion criteria) must be independent of the applicant.

**Finding Options:** Pass, Conditional (a specific independent source can be added before disbursement), or Fail (all evidence is applicant-controlled and no independent source is available for the primary outcome claim).

---

### Standard 3: Precision

**Assessment Question:** Is the claimed change larger than the variance of the measurement method, or are the completion criteria specific enough to distinguish done from not done?

For change-obligation rounds: the measurement instrument must be capable of detecting changes at the magnitude the project claims to produce.

For build-obligation rounds: the completion criteria must be specific enough to distinguish a passing deliverable from a failing one. Criteria that accept any output ("a working prototype," "some documentation") fail this standard.

**Finding Options:** Pass, Conditional (the instrument can be refined to achieve the required precision), or Fail (the instrument is structurally incapable of detecting the claimed effect size or distinguishing completion).

---

### Standard 4: Reliability

**Assessment Question:** Has the applicant used different metrics or methodologies for the same indicator in prior reporting, and if so, is the change documented with a rationale?

For first-time applicants: does the methodology specify enough precision that it could be applied consistently across reporting periods?

For continuation grants in any obligation mode: compare the indicator specification in this application against any prior reports on file. Methodology changes are not automatically disqualifying when documented; they are disqualifying when undocumented.

**Finding Options:** Pass, Conditional (a specific prior discrepancy can be documented and resolved before disbursement), or Fail (multiple undocumented methodology changes make prior periods incomparable and the baseline is unreliable).

---

### Standard 5: Timeliness

**Assessment Question:** Will the data be current at each disbursement decision point given the collection frequency?

For all obligation modes: data must be current to the reporting period. Annual data collection cannot support quarterly disbursement decisions. A completion claim based on work from a prior period not covered by the current gate does not satisfy timeliness.

**Finding Options:** Pass, Conditional (a secondary indicator or interim collection method can bridge the frequency gap), or Fail (no feasible collection method can satisfy the timeliness requirement for the proposed disbursement structure).

---

### Causality Stance and Counterfactual Reference (apply at gates configured at usage, outcome, or impact evidence scope)

This assessment applies where outcome or usage evidence is required and the round's gate configuration declares a causality stance. It is not part of the 1-4 indicator scoring; it confirms that the evidence presented matches the stance the funder declared. The reviewer does not choose the stance; the funder declares it in the published gate configuration. The reviewer confirms the evidence corresponds to it.

**The two stances.** CROSS requires the causality stance to be declared explicitly in the gate configuration. There are two positions on a causality spectrum.

*Attribution stance.* The gate requires evidence that the intervention caused the observed change. Counterfactual reference (below) is the standard methodology for attribution stance claims. Attribution stance is appropriate where the funder must defend a causal claim to an institutional body, where the intervention is the primary or only active change effort in the target population, or where future funding depends on causal proof rather than plausible contribution.

*Contribution stance.* The gate requires evidence that the intervention plausibly contributed to the observed outcome, with co-factors named and the contribution mechanism stated. Contribution stance does not require a counterfactual. It requires a named causal pathway from the funded activity to the observed change; a list of other interventions, conditions, or actors that also contributed; and a written account of why the funded intervention's contribution was material rather than incidental. Contribution stance is appropriate for most public goods and Web3 grants contexts, where multiple funders, tools, and community actors contribute to the same ecosystem outcomes and exclusive attribution is neither verifiable nor necessary.

**Reviewer Question (stance match):** Does the evidence presented match the stance the funder declared for this gate? Evidence that asserts exclusive causation where contribution stance was declared overstates; evidence that offers only plausible contribution where attribution stance was declared understates.

**Finding Options:** Pass (the evidence form matches the declared stance), Conditional (the evidence is close to the declared stance but a specific element is missing, for example a contribution-stance submission that names the pathway but omits the co-factor list), or Fail (the evidence form is structurally mismatched to the declared stance and cannot be corrected without redoing the outcome analysis).

**Counterfactual reference (apply only where the funder has configured the gate at counterfactual reference level).** This is an additional layer activated explicitly; it is not implied by selecting outcome evidence scope. Where it is configured, the funder must have specified the acceptable counterfactual methods before the round opened.

**Reviewer Question:** Does the submission include all four required contract elements?

- *Counterfactual baseline:* a documented estimate of what the indicator value would have been during the grant period without the intervention, derived from historical trend extrapolation from pre-intervention data, a matched comparison group not exposed to the intervention, or a modeled counterfactual with stated assumptions and sensitivity ranges.
- *Attribution argument:* a written account of why the observed change is attributable to the intervention rather than to confounding factors, naming the main alternative explanations and explaining why they are insufficient.
- *Comparison period or group:* a defined period or population serving as the counterfactual reference, described specifically enough that a reviewer can assess whether it is an appropriate comparison for the intervention context.
- *Independent attestation:* confirmation from a party outside the grantee organization that the counterfactual method and comparison group are reasonable given the intervention context and available data.

Where a comparison group cannot be defined because the intervention affects an entire ecosystem or operates at a protocol level with universal effects, confirm the grantee documents why a comparison group approach is not feasible and provides a modeled counterfactual with stated assumptions. Absence of a comparison group is not itself a gate failure; absence of a counterfactual estimate and attribution argument is.

**Finding Options:** Pass (all four elements present, or the comparison-group exception is documented with a modeled counterfactual), Conditional (a specific element can be completed before disbursement), or Fail (the counterfactual estimate and attribution argument are absent and cannot be supplied from the available data).

---

## Section 5: Conformance Checks

The three conformance checks are binary: each either passes or fails. They are not part of the scored rubric. A conformance check failure is not a rigor-tier finding; it is a disqualifying or process-requiring finding that operates independently of indicator scores. A conformance check failure produces a Do not fund recommendation regardless of indicator scores.

---

### Check 1: Concurrent Funding Disclosure

**Test:** Is the concurrent funding disclosure complete? Are all grants, investments, or revenue sources from the prior 24 months related to the scope of this application disclosed, including approximate amounts, relationship to the application's scope, ongoing reporting obligations, and any coordinating or decision-making rights held by funders?

For retroactive obligation rounds: the disclosure must cover prior awards for the same or overlapping work, as well as active grants and investments related to the application's scope.

**Token generation event disclosure (part of this check).** Token generation events, planned or executed within the prior 24 months, are required disclosure items alongside grants and investments. A token generation event is any mechanism by which the applying entity or its principals generate, allocate, or vest tokens to themselves, investors, or the public in a manner that represents or may represent economic value. This includes initial decentralized exchange offerings, token generation events, initial coin offerings, liquidity bootstrapping pool launches, and continuous founder or contributor vesting schedules releasing tokens during the disclosure window. The disclosed amount is the approximate United States dollar value at the time of the event, or for pending events, the planned allocation value based on the most recent publicly stated or implied valuation. A token that has not yet launched but for which a whitepaper, tokenomics document, or allocation schedule exists is a pending token generation event and must be disclosed. The existence of a token or planned token is not a disqualifier; non-disclosure of a material token event is treated as a concurrent funding omission under the same rules as undisclosed grants or investments, and fails this check.

**Independent Evidence:** If the reviewer has independent evidence of a funding relationship not disclosed in the form (public announcements, on-chain treasury flows, prior evaluations from other funders), the application fails this check. The finding must be documented with the source of the independent evidence.

**Finding Options:** Pass, or Fail (form is incomplete, a required field is absent, or the reviewer has independent evidence of an undisclosed relationship). Disclosed concurrent funding is not a disqualifier; non-disclosure is.

---

### Check 1-A: Scope Attribution and Outcome Credit (apply only when concurrent funding is disclosed)

This check applies in addition to Check 1 wherever the concurrent funding disclosure is present. If Check 1 passes with no concurrent funding disclosed, this check does not apply.

**Rigor tier check at entry.**

**Test (additionality Declaration):** Is an additionality declaration present? Does the scope boundary specify what this grant funds that concurrent sources do not, at a level of specificity that allows a reviewer to determine whether any proposed activity falls inside or outside this grant's scope?

| Finding | Action |
|---|---|
| Additionality declaration present; scope boundary is specific enough to adjudicate | Pass at entry. Proceed to scoring. |
| Additionality declaration present; scope boundary is too vague to adjudicate | Score as conditional (equivalent to a 2 on an indicator field). Condition: applicant must specify the scope boundary at sufficient precision before disbursement. |
| Concurrent funding disclosed; no additionality declaration submitted | Gate failure at entry. Document: "additionality declaration absent despite concurrent funding disclosure." Close evaluation. |

**Attribution fraction check at reporting stage (apply at any gate configured at usage, outcome, or impact evidence scope).**

**Test:** Is an outcome credit attribution statement present? Does it cover all funders that materially contributed to the reported result? Do attribution fractions sum to 100 percent across named funders and any residual category? Is the attribution rationale documented?

| Finding | Action |
|---|---|
| Attribution statement present; rationale documented; fractions sum to 100 percent | Pass. |
| Attribution statement present but rationale is absent or fractions do not sum to 100 percent | Conditional. Generate a condition: applicant must complete the attribution statement before disbursement is confirmed. |
| Outcome evidence submitted; no attribution statement present; concurrent funding was disclosed | Rigor-tier failure. Score equivalent to a 2 on the affected reporting field. |
| Attribution statement assigns 100 percent of outcome credit to this funder where multiple concurrent funders are named for the same scope and period | Flag for committee review. This is an inconsistency with the concurrent funding disclosure. Request a revised attribution statement. |

If attribution fractions change between reporting periods for the same indicator without a documented reason, note the change in the evaluation record and request documentation of the rationale and an assessment of prior-period comparability.

---

### Check 2: Adverse Signal Disclosure

**Test:** Has the applicant disclosed adverse signals relating to this application: prior rejections from similar programs, contradictory technical findings, or negative due diligence results from other funders?

**Standard:** The Adverse-Signal Engagement Principle Core Standard, incorporated by reference in CROSS, requires applicants to surface signals that contradict their self-presentation. Reviewers must not suppress adverse signals discovered during evaluation.

**Finding Options:** Pass (disclosure field is present; signals are disclosed or attested absent; no undisclosed signals discovered by reviewer), or Adverse signal documented (reviewer adds a specific signal to the evaluation record; committee notes it in deliberations). Non-disclosure of a signal the reviewer independently discovers is a process finding the committee weighs in deliberation; it does not automatically disqualify unless the signal also triggers Check 1.

---

### Check 3: Conflict of Interest

**Test:** Has each reviewer completed a conflict of interest declaration covering all three tiers before review began? Was the declaration submitted to a named receiving function separate from the person making the funding decision? Has a post-participation certification been completed confirming no new conflicts arose during review? The conflict of interest framework runs in both directions: reviewers disclose relationships to applicants, and applicants disclose relationships to committee members and reviewers. The applicable test is the reasonable third party standard: would an informed observer with knowledge of the relevant facts conclude that the person cannot maintain independence and is therefore not capable of objective and impartial judgment? The tier lists below illustrate the standard; a novel relationship type not listed that meets the reasonable third party standard still requires disclosure.

**Tier 1: categorical bar, no waiver.** Any Tier 1 conflict discovered after a review has been completed disqualifies the entire evaluation; the review must be restarted with a non-conflicted panel. Tier 1 relationships:

- Direct financial interest in the applicant entity, including equity, revenue share, or token holdings above the materiality threshold (default: greater than 1 percent of circulating supply, or greater than 5,000 United States dollars in value at the time of review)
- Family relationship with any principal, director, officer, or owner of the applicant project
- Prior receipt of funding from this funder in the same program area where the reviewer's funded work is directly related to the applicant's scope
- Being named as a team member, advisor, or contributor on the applicant project's public materials, whether compensated or not

A funder-side consulting arrangement that is the primary mechanism through which the reviewer receives income from the ecosystem being evaluated is also a categorical bar: structural income dependency on the funder's continued operation and on favorable award decisions is itself the conflict, with no need for a direct relationship to any specific applicant.

**Tier 2: disclosure required, qualified waiver possible.** A qualified waiver requires written justification submitted to a named authority other than the conflicted party, approval granted before participation (not after), and documentation in the review record. A waiver is not available where the relationship creates a financial interest. Tier 2 violations discovered during or after review require remediation: retroactive recusal, review restart, or award cancellation, depending on the degree of influence the conflicted party had. Tier 2 relationships include: employment with the applicant organization in the past 36 months; co-authorship or active project collaboration with applicant principals in the past 48 months; mentor or student relationship with applicant principals (no expiration); having received an honorarium, award, or gift from the applicant entity in the past 12 months; active negotiations or arrangements for future employment with the applicant organization; an organizational conflict where the reviewer's employer has a material financial relationship with the applicant; and an organizational role conflict, where the reviewer holds a paid or unpaid leadership, advisory, or operational role in another organization applying to this round or recently funded by this funder in the same program area (disclosure required even where no direct financial relationship exists, because the structural position across multiple funding relationships is itself the conflict). A funder-side consulting arrangement covering the same program area as the applications under review is a Tier 2 conflict with the qualified waiver procedure.

**Tier 3: disclosure encouraged, reasonable third party standard applies.** Social and community relationships (conference co-speakers, forum co-membership, shared group chats); prior interactions across grant rounds in different program areas; informal mentorship or advisory conversations without ongoing engagement.

**Attestation independence.** The conflict tiers apply not only to reviewers but to any party who signs an attestation confirming an applicant's gate evidence at any gate configured at independent review level or above. A party who holds a Tier 1 conflict with an applicant may not serve as the independent reviewer or sign an attestation confirming that applicant's gate evidence, regardless of the attestation format used. A Tier 1-conflicted party who signs an on-chain attestation, issues a signed document, or issues a credential confirming milestone completion has not satisfied the independent review requirement; the attestation does not meet the evidence strength standard regardless of its format. A party who holds a Tier 2 conflict requires a qualified waiver before serving as attestor, using the same procedure as the reviewer waiver requirement. Confirm reviewer and attestor conflict status before accepting any attestation as satisfying independent review evidence strength. (This is the attestation-independence element of CRAFT's non-self-adjudication requirement.)

**Finding Options:** Pass (all declarations on file, submitted before review began, post-participation certifications complete, no Tier 1 or undisclosed Tier 2 conflicts identified among reviewers or attestors), or Violation (document the tier, the relationship, and the remediation determination). Non-disclosure of a Tier 1 conflict is a disqualifying violation; non-disclosure of a Tier 2 conflict is a process violation requiring remediation.

---

### Check 3-A: Cohort Position Assessment (round-level procedure)

This check is performed across all applicants in a round, before final gate determinations are issued, not within a single application's review. It is recorded in the round record. A reviewer assessing one application contributes the data (named personnel, the on-chain identity anchor, the disbursement authority address, and named endorsers) that the program uses to run this assessment.

**Test:** Across all applications in the round, does the program check for three overlap patterns?

- *Personnel overlap:* does any named team member, contact, or key contributor in one application also appear in another application in the same round under a different entity name?
- *Wallet overlap:* does any on-chain identity anchor or disbursement authority address in one application appear as a recipient, controller, or named address in another application in the same round?
- *Endorser concentration:* has the same identifiable party endorsed or attested to a disproportionate share of applicants in the same round using non-standard schemas?

| Finding | Action |
|---|---|
| No overlap across applications | Recorded in the round record. No action. |
| Personnel overlap | Does not disqualify either application; triggers a Tier 2 conflict of interest disclosure requirement for the overlapping individual (handled under Check 3). |
| Wallet overlap | Requires explanation. The same address appearing across multiple distinct legal entities applying separately is a material discrepancy requiring reconciliation before disbursement. |
| Endorser concentration | Informational. Recorded in the round record without disqualifying effect. |

---

### Check 4: Funder-Side Conformance (for program administrators, not for reviewer assessment of individual applications)

Note: the checks in this subsection are performed by program administrators, not by reviewers assessing individual applications. They confirm that the program itself is operating in conformance with Part XI of the standard before any round opens and when any deviation is discovered. Reviewers who discover a potential funder-side conformance gap during individual application review should flag it to the program administrator rather than recording it as a finding against the applicant.

**Pre-round configuration check.**

Before any round opens, confirm the following.

**Test:** Did the funder publish a gate configuration before this round opened? Does the published configuration specify, for each active gate, the evidence scope, evidence strength, and infrastructure declaration (where gates are configured at independent review level or above)?

| Finding | Action |
|---|---|
| Gate configuration published before round opened; all required elements present | Pass. |
| Gate configuration published but infrastructure declaration absent where required | Conformance gap. Round may not open until the infrastructure declaration is completed and published. |
| No gate configuration published before round opened | Conformance violation. Round should not proceed without a published configuration. |

**Mid-round and post-decision deviation check.**

**Test:** Did the gate configuration change between the round opening and the decision point? If yes, was the change documented with a rationale and submitted to a named authority before the gate was reached? Were applicants notified?

| Finding | Action |
|---|---|
| No changes to the published configuration | Pass. |
| Configuration changed; change documented with rationale; applicants notified before the gate | Documented deviation. Record in the round file. No conformance violation if process was followed. |
| Configuration changed; change not documented or applicants not notified | Funder obligation violation. Administrator must determine whether the deviation materially affected any applicant or grantee and initiate remediation where it did. |

**Appeals mechanism check.**

**Test:** Has the program published an appeals procedure specifying what decisions are appealable, on what grounds, within what time window, and designating an appeals body structurally separate from the original decision-making panel?

| Finding | Action |
|---|---|
| Appeals procedure published before round opened; appeals body designated | Pass. |
| No appeals procedure published | Conformance gap. The program must publish an appeals procedure before any gate decisions are made that would be subject to appeal. |

---

## Section 6: Recommendation Framework

CROSS recognizes three recommendation categories. No other categories exist.

---

### Fund

Available when all of the following conditions are met:

The entry specification gate passes (Section 2 finding is "Gate passes"). All indicator fields score 3 or 4 on the indicator specification rubric (no field scores 1 or 2). All five data quality standards pass. All three conformance checks pass. No unresolved conditions of any type are present.

A score of 3 on one or more indicator fields is compatible with a Fund recommendation. It indicates a minor gap and does not generate a condition. Reviewers note 3-score findings in the evaluation record for the grantee's awareness during reporting.

For retroactive obligation rounds where the indicator rubric does not apply: Fund is available when the entry specification gate passes, the program's published rubric assessment meets the award threshold, and all conformance checks pass.

---

### Fund with Conditions

Available when the gate passes and at least one indicator field scores 2, or at least one data quality standard produces a conditional finding, but no indicator field scores 1, no conformance check fails, and no gate failure has been documented.

Conditions must meet all three of the following requirements. Each condition must specify exactly what must be resolved. Each condition must be verifiable by a named method ("committee review" is not a verification method). Each condition must be time-bounded, with a stated deadline before disbursement occurs.

Conditions attach to disbursement, not to the grant period. Resolution is confirmed before funds are released. The evaluation record must list each condition, the verification method, and the deadline.

---

### Do Not Fund

Required when any of the following apply:

The entry specification gate fails. Any primary indicator field scores 1. Any conformance check fails.

The evaluation record must distinguish which type of failure produced the finding. A gate failure and a rigor-tier failure are both Do not fund findings but carry different messages. A gate failure means the applicant has not performed the required diagnostic work for the declared mode; the path to resubmission is to do that work first. A rigor-tier failure means the diagnostic work exists but the indicator specification is incomplete; the path to resubmission is to complete the specified fields.

For build-obligation gate failures: the applicant has not named a falsifiable deliverable or verifiable completion criteria; the corrective signal is to specify the deliverable and the done criteria.

For change-obligation gate failures: distinguish D2 (applicant has not diagnosed a problem; needs to do diagnostic work before applying) from D1-equivalent rigor failures (applicant has a diagnosis but the specification is incomplete; needs specific field completion).

For retroactive obligation gate failures: the applicant has not provided the required categories of contribution evidence; the corrective signal names which categories were absent.

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.3.1 | 2026-06-08 | Frame Language own-voice pass. Own-voice watchlist terms were replaced with the structural act each names (mandatory became required; credible became verifiable; the Governing test became the Applicable test). Two naming updates aligned the rubric with the spec: Precondition F "Governance and continuity resilience" became "Decision-standing structure and Continuity Capacity", and the "Attestation integrity" check became "Attestation independence". The WALKRI Integrity data-quality standard, the canonical beneficiary dimension name, framework names, and the changelog rows were preserved as citation. Em-dash sweep clean. No scoring or recommendation vocabulary changed; vocabulary and naming only. |
| 0.3.0 | 2026-06-05 | Synced to CROSS spec 0.5.0. Added reviewer calibration as an assessment precondition in Section 1. Added Section 2-0 entry-gate preconditions: organizational identity completeness, disbursement authority, sufficiency architecture coherence, public benefit mechanism and access condition, development stage consistency, governance and continuity resilience, obligation fulfillment record, and prior work attribution. Added the served-population risk-bearer floor check to the entry and subsequent gates (spec Part II beneficiary dimension). Added the causality stance distinction (attribution versus contribution) and the counterfactual reference assessment to Section 4. Added token generation event disclosure to Check 1. Expanded Check 3 with the three conflict-of-interest tiers and the attestation-integrity provision, and added Check 3-A Cohort Position assessment. Noted the CRAFT framing where relevant: CROSS is a domain application of CRAFT (spec Part XIII receipt). No change to the 1-4 indicator field scoring or the recommendation vocabulary. |
| 0.2.0 | 2026-05-14 | Companion rubric to CROSS spec 0.2.0. Three obligation modes, mode-specific entry specification gates, eleven-field indicator rubric, five data quality standards, three conformance checks, recommendation framework. |

---

*End of CROSS Assessment Rubric v0.3.0*
