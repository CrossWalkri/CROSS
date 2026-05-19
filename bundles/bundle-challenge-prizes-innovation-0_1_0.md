---
title: CROSS+WALKRI Program Bundle - Challenge Prizes and Innovation Grants
version: 0.1.0
date: 2026-05-19
license: CC0
standards: CROSS v0.4.7 (github.com/cross-walkri/CROSS), WALKRI v0.1.7 (github.com/cross-walkri/WALKRI)
bundle_type: challenge-prizes-innovation
---

# CROSS+WALKRI Program Bundle: Challenge Prizes and Innovation Grants

---

## Overview

This bundle covers programs that fund the creation of novel solutions to defined problems through competitive mechanisms: challenge prizes with a specified problem and winner structure, milestone-based innovation grants funded by advanced research agencies, staged innovation funding programs with escalating evidence requirements at each phase transition, and open innovation competitions that accept public solution submissions.

Four program sub-types operate in this space with materially different obligation structures. This bundle addresses all four and notes where provisions diverge.

**Sub-type A: Challenge prizes** post an open competition against a specified problem, with a prize amount (or tiered prize structure) awarded to the solver or team that best satisfies the stated criteria. The prize is the incentive; completion of the challenge is the obligation. Prize criteria, evaluation rubric, and prize amount must all be committed to before any solver begins work.

**Sub-type B: Milestone-based innovation grants** fund performers against a sequence of pre-specified milestones, with payment contingent on confirmed achievement of each milestone. The ARPA-H Payable Milestones structure is the canonical implementation: completion criteria specified before work begins, payment triggered by the Program Manager's confirmation of achievement, non-achievement triggering termination rather than remediation. ARPA-E and SBIR/STTR Phase II programs follow related but distinct structures.

**Sub-type C: Staged innovation funding** allocates grants in phases, with each phase requiring a higher level of evidence than the prior phase before the next allocation is made. The Education Innovation Research (EIR) program's Early-Phase, Mid-Phase, and Expansion tiers are the canonical implementation, using ESSA/WWC evidence tiers as the gating standard. Wellcome Leap programs follow a related staged structure.

**Sub-type D: Open innovation and crowdsourced solutions** accept solution submissions from the public, often through a platform intermediary (the InnoCentive model). The problem statement, submission requirements, evaluation criteria, and prize or licensing terms are specified before any submission is made.

---

## Part 1: CROSS Runbook

### Obligation Mode Selection

**Sub-types A, B, and D:** Use Build obligation mode. Challenge prizes, milestone-based grants, and open innovation competitions all fund the creation of a specific solution, prototype, demonstration, or technology. The obligation is to build something that achieves the specified performance threshold. The completion gate confirms that the built thing achieves the stated criteria.

**Sub-type C (staged innovation funding):** Use Build obligation mode for the early phases (where a prototype or proof of concept is the deliverable). Transition to Change obligation mode at phases where the grant funds a scaled program and the required evidence is demonstration of measurable outcomes in a real population (EIR Mid-Phase and Expansion require outcome data from independent evaluation, not just proof of concept).

**Portfolio-level continuation benchmark (Sub-types B and C):** The SBIR/STTR program introduces a new primitive: a portfolio-level continuation benchmark applied to the funder, not the individual grantee. The SBIR portfolio is expected to maintain a Phase I-to-Phase II transition rate benchmark and a commercialization revenue benchmark per Phase II award. This benchmark is applied to the funder's full portfolio, not to individual performers. CROSS's continuation gate applies at the funder level as well as the grantee level for programs using this structure.

### Entry Specification Gate

Before any competition opens, any solver begins work, or any performer commences a milestone, the following must be committed to in writing and published in a verifiable location (a public Federal Register notice, a program website with a stable URL and publication timestamp, or an on-chain governance record):

**Competition or program specification:**
- Obligation mode (Build, transitioning to Change for staged programs)
- Total prize pool or funding allocation, and whether the prize is winner-takes-all, tiered, or divided
- Problem statement at operational precision (see Problem Statement field specification below)
- Eligibility criteria (who may submit: individuals, teams, small businesses, academic institutions, international entities)
- Evaluation rubric with scoring weights (not just criteria names; weights must be stated before submissions open)
- Milestone sequence and completion criteria for each milestone (Sub-type B)
- Phase transition evidence requirements for each phase (Sub-type C)
- IP and commercialization terms (who owns the solution; what licensing applies to submissions; revenue sharing if any)
- Prize payment or funding disbursement mechanism and timeline

**Pre-specification as the central gate requirement:** Pre-specification is the most critical primitive for this program type. Challenge prizes and innovation grants fail their core purpose if criteria shift after solvers have invested resources in developing solutions. Any change to the problem statement, evaluation rubric, scoring weights, prize amount, or eligibility criteria after the competition opens constitutes a material change requiring disclosure to all enrolled participants and re-opening the entry window if the change disadvantages solvers who made design decisions based on the original specification.

**Completeness requirement for completion criteria:** "A solution that achieves X" is not a complete completion criterion. The completion criterion must specify: what demonstration constitutes evidence of a viable solution, what measurement protocol or test will be applied, what performance threshold must be met, who will administer the test, and under what conditions. Completion criteria that cannot be confirmed by an independent assessor who did not participate in the program design do not satisfy this field.

**Human-in-the-loop override with published conditions (Sub-type A, referenced from Optimism Retro Funding 2025):** Programs that use a formula-based or rubric-based determination of winners may pre-specify conditions under which a human committee can override the formula result. If an override mechanism exists, the conditions triggering the override, the composition of the override committee, and the decision process must be published before the competition opens. Override conditions that are not pre-published cannot be invoked without disclosing a change from the original specification.

**SBIR/STTR portfolio-level entry specification (Sub-type B):** The SBIR/STTR program specification must include the portfolio-level benchmarks the funder commits to at the program level: the Phase I-to-Phase II transition rate benchmark and the commercialization revenue benchmark per Phase II award. These are funder commitments, not individual grantee commitments, and must appear in the program specification before individual applications are solicited.

### Application Gate

**Problem alignment declaration:** Each applicant must declare how their proposed approach addresses the stated problem, at sufficient specificity that reviewers can assess alignment with the problem statement without relying on vague assertions of relevance.

**Technical approach specification:** The applicant's proposed technical approach must describe: the core mechanism by which the solution achieves the stated performance threshold, the key technical risks and proposed mitigation, and the expected demonstration pathway (how the applicant plans to show that the solution works). Approaches that cannot be described at this level of specificity indicate insufficient readiness to enter a milestone-based program.

**Team identity and qualification:** All named contributors and key personnel must be identified. For Sub-type B programs (ARPA-H, SBIR/STTR): key personnel by name and role; subcontractor relationships; facilities and resources. For Sub-type A and D programs: team identification at the level required by the competition rules, including pseudonymous participation if the competition permits it (in which case the prize payment mechanism must accommodate pseudonymous payees).

**IP status declaration:** The applicant must declare the IP status of any prior work the proposed solution builds upon: whether prior IP is owned by the applicant, licensed from a third party, in the public domain, or subject to a government-use license from prior Federal funding. Solutions that build on third-party IP without a declared license or permission do not satisfy this field.

**Commercialization plan (Sub-type B, SBIR/STTR):** SBIR/STTR Phase II applications must include a commercialization plan specifying: the target market, the anticipated revenue model, the pathway from Phase II prototype to commercial product, and evidence of private sector interest (letters of intent, commitments to Phase III investment, or equivalent). The commercialization plan is not a deliverable; it is an entry specification for the Phase II application gate.

### Completion Gate

**Sub-types A and D (challenge prizes, open innovation):** Completion evidence is the submitted solution assessed against the pre-specified evaluation rubric. Assessment must be conducted by the evaluation panel named at the entry gate, using the rubric with the weights committed to at the entry gate. A solution assessed by a different panel, or against criteria modified after the competition opened, has not passed the CROSS completion gate.

**Sub-type B (milestone-based, ARPA-H model):** Completion evidence for each milestone is the Program Manager's confirmed achievement determination. The determination must confirm that the deliverable meets the completion criteria stated in the milestone specification, not a general judgment that the performer made good progress. Non-achievement of a milestone triggers termination of the program, not a remediation plan; this is an ARPA design principle that CROSS's completion gate structure accommodates but does not require other programs to adopt.

**Sub-type C (staged programs, EIR model):** Completion evidence for each phase is the evidence package required by the phase transition criteria. For EIR Early-Phase: a completed feasibility study or pilot demonstrating ESSA Tier 3 promising evidence (well-designed study with positive findings). For EIR Mid-Phase: results from a rigorous independent evaluation demonstrating ESSA Tier 2 moderate evidence (quasi-experimental design with significant positive impact). For EIR Expansion: results from prior Mid-Phase demonstrating sizable, significant impacts replicable at scale.

**SBIR/STTR portfolio-level completion (Sub-type B):** In addition to individual performer completion gates, the SBIR program tracks portfolio-level benchmarks. Portfolio-level non-performance (transition rate below benchmark, commercialization revenue below benchmark) triggers a program-level review, not individual performer sanctions. CROSS accommodates this by applying the continuation gate to the funder's portfolio as well as to individual grantees.

**Formula and rubric integrity check:** For any program using a formula or scoring rubric to determine winners or rankings, the completion gate must include a formula integrity check: confirmation that the formula or rubric committed to at the entry gate was applied without modification to the data or submissions collected. Any deviation from the committed formula must be disclosed and, if it materially affects rankings, treated as a specification change.

### Attestation Gate and Corpus

The Attestation Corpus for challenge prizes and innovation grants should be structured to preserve the pre-specification record and the completion determination in a form that can be independently audited:

- Competition or program specification: published with a stable URL and timestamp before submissions open; for Federal programs, the Federal Register notice number serves as the primary reference
- Application record: for challenge prizes, application metadata at minimum (applicant identity, submission date, submission identifier); for milestone-based grants, the full milestone specification document and the applicant's accepted proposal
- Evaluation record: for challenge prizes, the scoring rubric applied, the scores assigned, and the panel members who assessed; for milestone-based grants, the Program Manager's milestone achievement determinations with dates
- Prize or disbursement record: payment amount, date, and payee identity for each award
- Portfolio-level benchmarks record (Sub-type B, SBIR/STTR): the funder's portfolio performance data at the end of each program year, confirming whether the portfolio-level benchmarks were met

### Continuation Gate

For staged programs (Sub-type C) and multi-phase programs (Sub-type B):

A continuing performer must demonstrate: confirmed achievement of all prior phase milestones, a current technical approach and team composition consistent with the accepted proposal (or disclosed changes), and an updated IP status declaration.

A continuing program operator must demonstrate: the entry specification gate for the next phase is published before the prior phase closes, the attestation corpus for the prior phase is complete and publicly accessible, and the portfolio-level benchmarks (if applicable) are being tracked and are within range of the committed targets.

---

## Part 2: WALKRI Field Specifications

The following field specifications cover the intake fields most commonly required in challenge prize and innovation grant programs. Each specification satisfies WALKRI's five pre-publication requirements: criterion intent, operational definition, response form, evidence form, compliance threshold.

---

### Field: Problem Statement and Success Criteria

**Criterion intent:** Defines the problem the competition or grant is designed to solve at sufficient operational precision that solvers can design solutions that meet the stated requirements, and evaluators can confirm whether a submitted solution achieves the stated success criteria. The problem statement is the contract between the funder and all participants; vague problem statements produce vague solutions and make the completion gate unenforceable.

**Operational definition:** A problem statement is operationally specified when it includes: the phenomenon or condition to be addressed (what exists now that the solution must change), the target context (what environment or population the solution must work in), the performance threshold (what level of achievement constitutes success, stated in measurable units), and the constraints (what the solution may not do or require in order to be eligible). A success criterion is operationally specified when it names the measurement protocol or test that will be applied, the instrument or measurement tool, the conditions under which the test will be administered, and the numerical threshold that constitutes passing.

**Response form:** A structured problem statement covering: context description (2-4 sentences identifying the phenomenon, the target context, and why existing solutions are insufficient), a primary success criterion (one or more measurable thresholds the solution must achieve, each stated with a unit, a target value, and a measurement method), secondary criteria (if multiple criteria apply, the rubric weights assigned to each), and constraints (explicit exclusions: what the solution must not require, cost, or do).

**Evidence form:** The problem statement is itself the evidence form for this field; it is published before the competition opens. At completion: the test protocol used to assess each submitted solution against the primary success criterion, with the results for each submission scored against the stated threshold. The test protocol must be the one described in the problem statement; deviation requires disclosure.

**Compliance threshold:** A primary success criterion stated with a unit, a target value, and a named measurement method. A problem statement without a measurable threshold (for example, "the best solution to X" without a definition of "best" in measurable terms) does not satisfy this field. Rubric weights for secondary criteria must be stated as percentages or point allocations summing to 100% of the total evaluation score. Unstated weights, or weights stated as ranges rather than fixed values, do not satisfy this field.

---

### Field: Proof of Concept Requirements

**Criterion intent:** Specifies what demonstration constitutes evidence that a proposed solution is viable, distinguishing between a claim that a solution will work and confirmation that a working solution exists or has been produced, at a defined level of technical readiness appropriate to the program phase.

**Operational definition:** A proof of concept is a demonstration that the core mechanism of a proposed solution functions at a defined level of technical readiness (TRL). The TRL level required must be stated before the competition or program phase opens. A proof of concept requirement is operationally specified when it names: the TRL level required, the demonstration environment (laboratory bench, simulated field conditions, real-world field conditions), the measurement protocol used to confirm the mechanism functions, and the documentation format for the demonstration (video, test report, sample submission, working prototype available for independent testing).

**Response form:** For each required demonstration: TRL level required (using the NASA TRL scale or the program's equivalent), demonstration environment, what must be shown (the mechanism, the performance threshold, or both), the documentation format in which the demonstration will be provided, and whether independent testing by the evaluator is required or whether applicant-provided documentation is sufficient. Programs that require laboratory bench demonstration at TRL 3-4 must state this explicitly; programs that require field demonstration at TRL 6-7 must state this explicitly. The TRL level is a completion criterion, not a target aspiration.

**Evidence form:** At submission or at the milestone confirmation stage: the demonstration documentation in the stated format. For programs requiring independent testing: the independent test report signed by the testing entity named in the program specification. For programs accepting applicant-provided documentation: the documentation with sufficient technical detail that an independent expert reviewer can assess the claimed mechanism. Self-assertions that a solution "works" without supporting documentation do not satisfy this field.

**Compliance threshold:** A named TRL level with a named demonstration environment. A proof of concept requirement that accepts "early-stage" or "promising concept" without a TRL level does not satisfy this field. Programs with staged TRL requirements (e.g., TRL 3 at phase one, TRL 6 at phase two) must state the TRL requirement for each phase in the relevant phase's entry specification gate.

---

### Field: Evaluation Rubric with Scoring Weights

**Criterion intent:** Commits the funder to the criteria and relative weights that will determine winners or rankings before any solver invests resources in developing a solution, so that solvers can design their approaches to the stated priorities and so that the completion gate determination is auditable against the committed rubric.

**Operational definition:** An evaluation rubric is the full set of criteria used to assess submissions, with each criterion's definition, the scoring method applied to it, and the weight it carries in the final determination. A rubric is fully specified when: every criterion is named and defined, the scoring method for each criterion is stated (binary pass/fail, a numerical scale with defined anchor points, or a formula), the weight of each criterion in the final score is stated as a percentage or point value, the total weight sums to 100% or the stated maximum score, and the minimum passing threshold (if any) is stated for each criterion individually and for the total score. Rubric specifications published after submissions open do not satisfy CROSS's pre-specification primitive regardless of their quality.

**Response form:** A rubric table with columns for: criterion name, criterion definition (what counts as strong performance on this criterion), scoring method (scale, formula, or pass/fail with definitions), weight (percentage of total score), and minimum passing threshold if applicable. A narrative explanation of how the criteria collectively assess the competition's success criteria. For programs with a multi-stage evaluation process (a technical review panel followed by a program leadership review): the rubric for each stage must be separately specified, with the relationship between stages (e.g., the technical panel advances finalists; program leadership selects from finalists) stated before submissions open.

**Evidence form:** The published rubric document with a timestamp predating the submission window opening. At completion: the score sheet for each submission assessed, showing scores by criterion, the weight applied, and the total score. For challenge prizes: the ranking of all assessed submissions with scores. For milestone-based grants: the milestone achievement determination with the completion criterion it is assessed against.

**Compliance threshold:** Every criterion must have a stated weight summing to 100% of the total. Rubrics with unstated weights, relative weights (e.g., "technical feasibility is the most important criterion"), or criteria described but not weighted do not satisfy this field. Weights that change after submissions open constitute a material change requiring the human-in-the-loop override mechanism (if pre-specified) or full redisclosure and re-opening of the submission window.

---

### Field: IP and Commercialization Terms

**Criterion intent:** Establishes who owns the solution produced through the competition or grant, what rights the funder retains, and what commercialization pathway is expected or required, so that participants can make informed decisions about whether to enter before investing resources.

**Operational definition:** IP terms are the rights assignments and licensing conditions that apply to solutions submitted to or developed under the competition or grant. Commercialization terms are the conditions under which the solution may be used, licensed, or brought to market after the competition or grant period ends. Both must be stated before the competition opens or the grant is awarded. The relevant IP categories are: copyright (in written, software, or documentation outputs), patent (in novel inventions produced during the program), trade secret (in undisclosed technical know-how that the solution depends on), and data rights (in data produced or used during development).

**Response form:** For each IP category relevant to the program: who owns IP created during the program (applicant, funder, shared), what license the funder receives in applicant-owned IP (none, a government-use license, a non-exclusive commercial license, or an exclusive license), the duration and geographic scope of the license. For commercialization terms: the post-award commercialization requirement if any (SBIR/STTR Phase II commercialization plan requirement), revenue sharing terms if any, the period after which the funder's license lapses if not exercised, and any open source or public domain requirements for software outputs. For Federal programs: Bayh-Dole Act applicability and the Government's march-in rights, if applicable.

**Evidence form:** The IP and commercialization terms document published as part of the program specification before submissions open. For Federal programs: the relevant FAR or DFARS clauses governing IP rights, cited by clause number. At completion (for commercialization-required programs): the commercialization progress report from the grantee covering the period specified in the program documentation.

**Compliance threshold:** A named owner for each IP category, a named license grant to the funder (or an explicit statement that the funder receives no license), and commercialization terms stated at sufficient specificity that a participant could obtain legal counsel on the terms before deciding to enter. Terms stating only that "IP ownership will be negotiated" after award do not satisfy this field. The IP terms must be final and non-negotiable before the competition opens; post-award negotiation of IP terms is a material change requiring the specification change disclosure process.

---

### Field: Milestone Completion Criteria

**Criterion intent:** For Sub-type B (milestone-based innovation grants), specifies the conditions that must be confirmed for each milestone to be deemed achieved, at sufficient operational precision that the confirming authority (the Program Manager or equivalent) can make a binary determination without exercising discretion about what "achievement" means.

**Operational definition:** A milestone completion criterion is the specific, measurable condition that must be met for a milestone to be confirmed as achieved. The criterion is operationally specified when it includes: what must exist or be demonstrated (the deliverable, the performance result, or the condition), who confirms it (the named confirming authority), the method of confirmation (independent test, review of submitted documentation, on-site demonstration), the standard against which it is confirmed (the performance threshold from the problem statement, the specification document, or the test protocol), and the timeline for confirmation after submission. A milestone criterion that relies on the confirming authority's judgment about quality, promise, or trajectory does not satisfy this field; the criterion must be confirmable by binary observation.

**Response form:** For each milestone: milestone name and sequence number, due date or duration from program start, deliverable or demonstration required, performance threshold to be achieved, confirmation method (independent test, document review, or demonstration with named confirming party), confirmation timeline (how many days after submission the confirming authority will issue a determination), and consequence of non-achievement (program termination, re-scoping agreement, or other specified consequence). For ARPA-H Payable Milestones: the payment amount triggered by confirmation of each milestone, stated as a dollar amount and as a percentage of the total program value.

**Evidence form:** The milestone completion specification document, published before the performer begins work on the milestone. At completion: the confirming authority's written determination that the milestone was or was not achieved, with the specific completion criterion it is assessed against, the test results or documentation reviewed, and the date of determination. A determination that is not written, or that does not reference the specific completion criterion, does not constitute a CROSS attestation corpus record for the milestone gate.

**Compliance threshold:** Every milestone must have a named confirming authority, a named confirmation method, and a binary completion criterion. Milestones with criteria stated as "significant progress toward X" or "a promising approach to Y" do not satisfy this field. The confirming authority must be identified by name or role before the performer begins work; changing the confirming authority mid-program requires disclosure.

---

### Field: Independent Verification Mechanism

**Criterion intent:** Establishes who confirms that the claimed achievement of a milestone, competition winner determination, or phase transition is accurate, independent of the performer or funder's internal review, so that the completion gate determination is externally auditable.

**Operational definition:** An independent verification mechanism is the process by which an entity not party to the grant or competition confirms the accuracy of a completion determination. For challenge prizes: an evaluation panel whose members are identified before the competition opens and who are independent of the prize administrator, the performers, and the funding entity. For milestone-based grants: a Program Manager or technical review panel whose determination is based on objective test results rather than judgment, with the test administered by a laboratory or testing facility independent of the performer. For staged programs: the independent evaluation required at each phase transition, conducted by an evaluator who did not assist in designing or implementing the program being evaluated.

**Response form:** The names or roles of the independent verifying entity or entities (individual panel members do not need to be named before the competition opens, but the selection process, qualification criteria, and conflict of interest policy must be stated). The verification method: what the verifier does, what data or demonstrations the verifier is given access to, and what the verifier produces (a signed test report, a panel determination memo, an independent evaluation report). The verifier's independence criteria: what relationships would disqualify a potential verifier. The timeline for verification relative to the completion gate determination.

**Evidence form:** For challenge prizes: the evaluation panel members' names and affiliations, disclosed at or before the winner announcement, with a statement of any conflicts reviewed. For milestone-based grants: the test report or determination memo from the confirming authority, with the tester's or laboratory's name and accreditation. For staged programs (EIR): the independent evaluation report with the evaluator's name, institutional affiliation, and the evaluation methodology used.

**Compliance threshold:** A named verification entity or a specified selection process for identifying the verification entity. Programs that state "an independent panel will review submissions" without specifying the selection process, qualification criteria, or conflict of interest policy do not satisfy this field. For programs requiring ESSA or WWC-equivalent evidence standards: the independent evaluator must be unaffiliated with the program developer and must use a study design meeting the specified tier (ESSA Tier 1, 2, or 3) as declared in the program specification.

---

### Field: Phase Transition Evidence Requirements

**Criterion intent:** For Sub-type C (staged innovation funding), specifies the evidence standard that must be met before a grantee advances from one phase to the next, ensuring that the escalating evidence requirement is pre-specified rather than applied retrospectively at the discretion of program officers.

**Operational definition:** A phase transition evidence requirement is the minimum evidence standard a grantee must demonstrate to be eligible for the next phase of funding. The evidence standard is stated in terms of a named evidence framework (ESSA/WWC evidence tiers, IES What Works Clearinghouse standards, or the program's own evidence hierarchy) and a specific tier or level within that framework. The standard must specify: the study design required (randomized controlled trial, quasi-experimental design, or pre-post with comparison group), the effect size requirement if any, the statistical significance threshold, the sample size and demographic representativeness requirements, and whether the evaluation must be conducted by an independent evaluator or may be conducted by the grantee.

**Response form:** For each phase transition: the evidence tier required (stated as the specific tier in the named framework, e.g., ESSA Tier 2: Moderate Evidence), the minimum study design (RCT, quasi-experimental, or equivalent), the statistical significance threshold, any minimum effect size requirement, the sample requirement (minimum n, demographic representativeness criteria), whether the evaluation must be independent (as in EIR Mid-Phase and Expansion), and the documentation format in which the evidence must be submitted. For programs that allow a portfolio of evidence rather than a single study: the rules for how multiple pieces of evidence are combined to meet the tier requirement.

**Evidence form:** At each phase transition application: the evaluation report or evidence portfolio submitted by the grantee, with the evaluator's name and methodology. The program's phase transition determination record, confirming that the evidence meets the stated tier requirement. For EIR: the IES-aligned assessment of the submitted evidence against the ESSA tier criteria.

**Compliance threshold:** Every phase transition must have a named evidence framework and a named tier within that framework. Phase transition requirements stated only as "strong evidence of effectiveness" or "promising results" without a named framework and tier do not satisfy this field. The evidence standard must be the same framework and tier for all grantees in the same program cohort; applying different standards to different grantees in the same phase cohort without disclosure constitutes a specification change.

---

## Part 3: Compatibility Map

This section maps the challenge prizes and innovation grants program type to the frameworks in the CROSS+WALKRI compatibility corpus that are most directly applicable. The map is organized by primitive.

---

### Pre-specification Primitive

The pre-specification primitive is the central requirement for this program type: prize criteria, evaluation rubric, prize amount, and completion criteria must all be committed to before any solver begins work. Frameworks that implement this primitive most rigorously:

- **ARPA-H Payable Milestones**: milestone completion criteria specified for each milestone before any performer begins work; payment contingent on confirmed achievement; the most rigorous implementation of pre-specification in the Federal grant ecosystem
- **Optimism Retro Funding 2025**: the metrics formula and all input weights published before the assessment period opens; the human-in-the-loop override conditions published before the round opens; this is a retroactive-mode implementation of the same pre-specification principle
- **Nesta Challenge Prizes Practice Guide**: the Nesta guide's first principle is that the prize problem, criteria, and prize amount must be set before the competition opens; the guide's case studies document failures caused by mid-competition criterion changes
- **EIR Program (IES)**: phase transition evidence requirements published in the program announcement before the first cohort's Early-Phase applications are accepted

Compatibility statements: ARPA-H-Payable-Milestones, Optimism-Retro-Funding-2025, Nesta-Challenge-Prizes, EIR-IES-Program.

---

### Build Obligation Mode

Challenge prizes, ARPA-H milestone programs, SBIR/STTR Phase I and II, EIR Early-Phase, and all open innovation competitions operate in Build obligation mode. The obligation is to create a specific solution, prototype, or demonstration. Frameworks that define the Build obligation most precisely:

- **ARPA-H Payable Milestones**: the clearest operationalization of Build obligation mode in Federal funding; each milestone is a discrete deliverable with a binary completion determination
- **SBIR/STTR Phase I**: the prototype or proof of feasibility produced at Phase I is the Build deliverable; Phase I-to-Phase II transition rate is a portfolio-level Build completion benchmark
- **EIR Early-Phase**: the feasibility study or pilot is the Build deliverable; the ESSA Tier 3 evidence standard is the minimum completion criterion
- **Nesta Challenge Prize design**: the prize winner's solution is the Build deliverable; evaluation rubric determines which solution meets the Build criterion most completely

Compatibility statements: ARPA-H-Payable-Milestones, SBIR-STTR, EIR-IES-Program, Nesta-Challenge-Prizes.

---

### Independent Verification Primitive

The independent verification primitive requires pre-specification of who confirms achievement and by what method. Innovation program implementations:

- **ARPA-H Program Manager milestone confirmation**: the Program Manager's written achievement determination is the verification record; the PM's role and authority are defined in the program agreement before work begins
- **SBIR/STTR commercialization database**: the Small Business Administration's commercialization tracking database provides an independently maintained record of Phase II awardees' commercial outcomes; used for portfolio-level benchmark verification
- **EIR/WWC independent evaluation requirement**: EIR Mid-Phase and Expansion require independent evaluation by an evaluator unaffiliated with the program developer; the WWC Review Standards define the independence requirement
- **Nesta evaluation design**: Nesta's challenge prize practice recommends an independent evaluation of prize winner implementation, separate from the competition judging panel

Compatibility statements: ARPA-H-Payable-Milestones, SBIR-STTR-Commercialization-Database, EIR-IES-Program, WWC-Review-Standards.

---

### Portfolio Benchmarks Primitive

The portfolio benchmarks primitive is a new primitive identified in the SBIR/STTR structure: a benchmark applied to the funder's full portfolio, not to individual grantees. This is distinct from individual grantee completion gates. Implementations:

- **SBIR/STTR Phase I-to-Phase II transition rate benchmark**: the SBA applies a 0.25 transition rate benchmark to the full SBIR program portfolio; agencies below benchmark are subject to program review
- **SBIR/STTR commercialization revenue benchmark**: the USD 100,000 per Phase II award average is a portfolio-level target applied to the funder's program, not a requirement of any individual grantee
- **EIR cohort continuation rate**: IES tracks what percentage of EIR Early-Phase awardees advance to Mid-Phase as a program health indicator; this is an emergent portfolio benchmark

This primitive has no direct external precedent in non-Federal frameworks. CROSS is the first standards corpus to name it explicitly.

Compatibility statements: SBIR-STTR-Commercialization-Benchmarks, EIR-IES-Program (cohort tracking).

---

### Causality Stance Primitive (via Evidence Tiers)

Innovation programs address causality through evidence tier frameworks rather than through an explicit causality stance declaration. The evidence tier system is a graded series of causality claims:

- **ESSA Tier 1 (Strong Evidence)**: randomized controlled trial with significant positive impact; the strongest attribution claim the framework supports
- **ESSA Tier 2 (Moderate Evidence)**: quasi-experimental design with significant positive impact; a contribution claim with rigorous comparison group
- **ESSA Tier 3 (Promising Evidence)**: a well-designed correlational study with statistical controls; an association claim with documented co-variation
- **ESSA Tier 4 (Demonstrates a Rationale)**: a logic model or conceptual framework; a narrative causality claim without empirical confirmation

CROSS's causality stance declaration maps to the ESSA tier system: Tier 1 corresponds to attribution; Tiers 2-3 correspond to contribution at different levels of rigor; Tier 4 corresponds to association. Programs using EIR-style escalating evidence requirements should map their phase transition evidence requirements to the CROSS causality stance taxonomy.

Compatibility statements: ESSA-Evidence-Framework, WWC-Review-Standards, EIR-IES-Program.

---

### Escalating Evidence Primitive

The escalating evidence primitive requires that each successive phase of a staged program requires stronger evidence than the prior phase. The EIR program is the canonical implementation:

- **EIR Early-Phase**: ESSA Tier 3 promising evidence (feasibility study with positive findings); minimum evidence threshold for the initial grant
- **EIR Mid-Phase**: ESSA Tier 2 moderate evidence from a rigorous independent evaluation; required for phase transition from Early to Mid
- **EIR Expansion**: sizable, significant impacts from prior Mid-Phase evaluation demonstrating scalability; required for the largest grant tier
- **Wellcome Leap programs**: Wellcome uses a stage-gate model with escalating technical readiness requirements (TRL-based rather than evidence-tier-based) for health innovation programs; the TRL and ESSA approaches are parallel implementations of the same escalating evidence primitive

Compatibility statements: EIR-IES-Program, ESSA-Evidence-Framework, Wellcome-Trust-Grant-Conditions.

---

### Human-in-the-Loop Override with Published Conditions

The human-in-the-loop override primitive, first identified in the Optimism Retro Funding 2025 structure, applies in challenge prize contexts when a formula-based or rubric-based determination is subject to human review under pre-specified conditions:

- **Optimism Retro Funding 2025**: the canonical implementation; override conditions (categories of outcome that would trigger committee review) published before the assessment period opens
- **ARPA-H Payable Milestones**: the Program Manager's determination is itself the human-in-the-loop mechanism; the PM's authority to deviate from the stated completion criterion is constrained by the program agreement, not entirely eliminated; deviation triggers a contract modification process rather than an informal override

This pattern is new in the corpus and not yet addressed by any external framework at the specificity level CROSS requires.

Compatibility statements: Optimism-Retro-Funding-2025, ARPA-H-Payable-Milestones (deviation process).

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
