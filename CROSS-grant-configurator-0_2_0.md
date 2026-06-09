---
title: CROSS Grant Configurator
version: 0.3.1
date: 2026-06-08
license: CC0
status: Working draft. Companion implementation specification synced to CROSS-common-reporting-outcome-standards-schema-0_5_0.md. Inherits all field definitions, tier logic, and gate requirements from that standard. Supersedes version 0.2.0.
related_documents:
  - standards/CROSS-common-reporting-outcome-standards-schema-0_5_0.md
  - standards/CROSS-runbooks-0_1_0.md
  - standards/CROSS-grantee-dashboard-0_1_0.md
changelog:
  - version: 0.3.1
    date: 2026-06-08
    summary: >
      Frame Language own-voice pass. Own-voice watchlist terms were replaced with
      the structural act each names (the govern family became covers, applies to,
      or subject to; mandatory and the "become mandatory" field-clustering language
      became required; the concurrent-funding field governance rights became
      decision rights; own-voice beneficiary populations became affected
      populations). Framework names, the Procurement Integrity dimension name,
      the Continuity Capacity and Collective names already in place, and the
      changelog rows were preserved. Em-dash sweep clean. No configuration step,
      question, or requirement changed; vocabulary and naming only.
  - version: 0.3.0
    date: 2026-06-05
    summary: >
      Synced to the 0.5.0 standard. Added the entry-gate declarations a funder must
      collect (organizational identity, sufficiency architecture, public benefit
      mechanism, development stage, continuity resilience, obligation
      fulfillment record) as configuration steps in Q3A. Added reviewer calibration
      (Q11.6), the round specification pre-commitment (Q13), structured dataset
      publication and the funder-side Attestation Corpus query procedure (Q14),
      measurement framework declarations (Q3B), the continuation gate causality
      stance and counterfactual reference option (Q5 and Q11), and the
      infrastructure declaration requirement extended to reviewer calibration at
      independent-review level or above. Added a CRAFT-inheritance note recording
      that CROSS is a domain application of CRAFT (standard Part XIII receipt).
  - version: 0.2.0
    date: 2026-05-14
    summary: Runbook selection, per-stage obligation mode, program-level continuation gates, four-gate configuration sequence.
---

# CROSS Grant Configurator

Version 0.3.1 | 2026-06-08 | CC0

---

## Section 1: Purpose and Scope

The CROSS Grant Configurator is the pre-award instrument through which funders generate a round-specific obligation specification from their eligibility criteria. It is the operational entry point into the CROSS (Common Reporting Outcome Standards Schema) ecosystem for funders opening a new grants round or a new program stage.

The Configurator serves funders, not applicants. A program officer, grants committee, or foundation staff member uses the Configurator before a round opens to translate the funder's natural language eligibility criteria into a structured obligation schema. The output, the round specification, is published and becomes the authoritative coordinating instrument for that round. Applicants interact with the round specification; they do not interact with the CROSS standard directly.

The Configurator does not evaluate applications. It does not score, rank, filter, or recommend funding decisions. Those functions belong to reviewers applying the assessment rubric (CROSS-common-reporting-outcome-standards-schema-rubric-0_2_0.md). The Configurator's job is to establish, before any application arrives, exactly what applicants must demonstrate, which obligation dimensions are active, what gates are in effect, and what the reviewer rubric will look like for this round.

Version 0.2.0 of the Configurator extended version 0.1.0 in four structural ways. First, the Configurator supports runbook selection as a starting configuration: funders may select one of the standard runbook configurations (CROSS-runbooks-0_1_0.md) and customize from there. Second, the Configurator explicitly asks funders to declare the obligation mode (build, change, or retroactive) for each round or stage. Third, the Configurator supports program-level configuration: multi-stage programs configure continuation gates separately from round-level gates, and mode assignments are configurable per stage. Fourth, the disbursement structure question sequence was replaced with an explicit gate configuration sequence covering all four gate types from the CROSS standard: entry specification, progress verification, completion verification, and continuation specification.

This version (0.3.0) syncs the Configurator to the 0.5.0 standard. It adds configuration steps for the entry-gate declarations a funder must collect from every applicant (organizational identity, sufficiency architecture, public benefit mechanism, development stage, continuity resilience, and the obligation fulfillment record); for measurement framework declarations; for reviewer calibration at gates set to independent review or above; for the round specification pre-commitment; for structured dataset publication and the funder-side Attestation Corpus query procedure; and for the causality stance (attribution versus contribution) and its counterfactual reference option at outcome-bearing gates. These additions do not restructure the existing question sequence; they extend it. Each new step names the CROSS standard Part it encodes so the inheritance is traceable.

The Configurator produces one kind of output: a round specification. A round specification is a complete, self-contained obligation schema that instantiates the CROSS standard for a specific funder, round, and set of eligibility criteria.

**CRAFT inheritance.** CROSS is a domain application of CRAFT (Chains Reveal Attested Falsifiable Truth), the meta-standard for evaluation chain legibility. The Configurator is the funder-facing instrument through which several of CRAFT's six conditions are realized for a grants round: pre-specifying the decision before any application is received, publishing the criteria before the round opens, and recording the verification infrastructure the funder will operate. An implementer does not configure CRAFT separately. A round specification produced by a conformant Configurator satisfies CRAFT's conditions for that round's evaluations through the CROSS requirements encoded here. The full inheritance is declared in the CROSS standard's CRAFT inheritance receipt (Part XIII); this companion document does not restate it.

---

## Section 2: Two Modes of Operation

The Configurator operates in two modes that are sequentially dependent. Funder configuration mode runs before the round opens and produces the round specification. Applicant specification mode is embedded within the round specification and structures what applicants encounter when they submit.

**Funder configuration mode.** The funder answers the structured question sequence in Section 4 of this document. The Configurator takes those answers and generates the round specification: a complete obligation schema covering the obligation mode, gate configuration, active dimensions, required fields, conflict of interest configuration, common indicators if any, reviewer rubric calibration, reporting frequency, and disbursement structure. The round specification is then reviewed by the funder and published. Once published, it becomes the authoritative obligation commitment for the round. No field defined in the published round specification may be removed or relaxed without re-opening the configuration process and re-publishing.

**Applicant specification mode.** The round specification contains a structured application form pre-built from the funder's configuration choices. This form is what applicants see and complete. Within the form, applicants self-specify their outcome indicators using the fields defined in Part V of the CROSS standard: indicator name, rationale for indicator, measurement form and evidence classification, operational definition, construction and aggregation methodology, cumulative or non-cumulative designation, disaggregation categories, data source and collection method, data cost estimation, baseline or FROM state, and target or TO state. For build-obligation rounds, the entry specification form asks instead for a deliverable specification and completion criteria. For retroactive rounds, the form asks for prior contribution evidence and evidence of use. The Configurator's configuration choices determine which entry specification form applicants receive, which optional fields appear, which dimensions are active, and which common indicators (if any) are pre-populated and locked.

The boundary between the two modes is the act of publishing the round specification. Before publication, the funder is in configuration mode and can revise any choice. After publication, the round specification is fixed for that round, and any change to a material field requires re-publication with a documented revision reason.

---

## Section 3: Base Configuration

A base configuration is the persistent, round-independent record of what a funder always requires. It is established once, at the time the funder first adopts CROSS, and updated after each round closes through the lessons-learned register described in Section 7. It is not reconstructed each round. When a new round opens, the Configurator loads the base configuration and surfaces the delta: what this round's stated criteria add or emphasize relative to the base.

**Contents of a base configuration.** A base configuration contains the following elements.

The funder's standing eligibility criteria. These are the requirements that apply to every round regardless of topic or funding amount: open source requirement, ecosystem requirement, organizational type restrictions, and funding amount range. The funding amount range feeds the Coordination Scaling Standard tier calibration.

The funder's default obligation mode. For funders who operate a single program type consistently (for example, always build-obligation rounds), the default mode is recorded here. For funders who run different program types, the mode is set per round in the question sequence rather than in the base configuration.

The funder's default obligation tier calibration. This specifies which obligation dimensions are always active regardless of round-specific criteria. Dimensions that require per-round activation are not included in the base.

The funder's conflict of interest configuration. Two options are available. Permit Tier 2 waivers: Tier 1 relationships are categorical bars with no waiver; Tier 2 relationships require written disclosure and a qualified waiver process with a named receiving authority. Treat all Tier 2 as categorical bars: both Tier 1 and Tier 2 relationships are absolute bars. Either option inherits all tier definitions from Part VII of the CROSS standard; the base configuration specifies which treatment applies.

The funder's default token holdings materiality threshold. The CROSS standard default is greater than 1% of circulating supply or greater than \$5,000 in value at time of review, whichever is lower. The base configuration accepts this default or overrides it. Any override must be documented with a rationale. The threshold may be made more restrictive but not less restrictive than the CROSS default through configuration.

Any standing common indicators required across all rounds.

**Default rubric template.** The base configuration stores the funder's default rubric template: the rubric text the Configurator loads as the starting point for every new round before round-specific calibration is applied. The template is established from the first round's confirmed rubric and updated through the lessons-learned register after each subsequent round. A funder who has run three rounds will have a rubric template that reflects three cycles of calibration. A funder opening their first round has no template; the Configurator starts from the CROSS assessment rubric baseline plus any runbook-recommended emphasis.

**Rubric history log.** The base configuration maintains a chronological log of every confirmed rubric from every prior round this funder has run. Each entry contains: the round identifier, the obligation mode, the runbook used (if any), the full confirmed rubric text, the confirmation timestamp, and a brief summary of any reviewer feedback on rubric clarity or scoring consistency from the lessons-learned register for that round. When a funder opens a new round, the Configurator offers the rubric history log as an alternative starting point to the generated preview.

**Program-level continuation gate configuration.** For funders operating multi-stage programs, the base configuration also records the program-level continuation gate structure: the evidence scope and strength required for progression from one stage to the next, and the infrastructure declaration for any gate at independent review level or above. Program-level continuation gates are set once for the program and apply across all rounds in the program. They are distinct from round-level gates, which cover progress within a single round.

**Base configuration onboarding (for new funders).** When a funder adopts CROSS for the first time, the Configurator runs a one-time base configuration setup step before any round is opened. This step establishes the base configuration that all subsequent rounds inherit from. The funder selects a starting profile from the following options, or selects Custom to build the base configuration from scratch.

*Community and ecosystem funder.* Default obligation mode: build obligation. Default conflict of interest treatment: Tier 2 waivers permitted. Default documentation tier: Small Team scale for grants below a named threshold, Standard scale above. Rubric template: pre-populated from the Community Allocation with Build Obligation runbook emphasis. Appropriate for: Octant-style rounds, Gitcoin-style quadratic funding, ecosystem grant programs where many small teams apply and light-touch obligation is the right calibration.

*Institutional and foundation funder.* Default obligation mode: change obligation. Default conflict of interest treatment: all Tier 2 as categorical bars (or Tier 2 waivers permitted with named conformance staff). Default documentation tier: Standard to full institutional scale. Rubric template: pre-populated from the Institutional Conformance runbook emphasis, with optional environmental and social impact and gender equity dimensions available. Appropriate for: foundations, development agencies, and any funder that must satisfy external obligation requirements or that funds at a scale requiring formal outcome documentation.

*Retroactive and recognition funder.* Default obligation mode: retroactive. Default conflict of interest treatment: Tier 2 waivers permitted with named panel conflict of interest process. Rubric template: the retroactive contribution template from the Retroactive Impact runbook, which the funder customizes per round. Appropriate for: programs that fund demonstrated past contribution, protocol recognition grants, sustained infrastructure maintenance awards.

*Staged and ladder funder.* Default obligation mode: build obligation at Stage 1, configurable per stage thereafter. Program-level continuation gate pre-configured with usage evidence requirement at the Stage 1-to-Stage 2 transition. Rubric template: pre-populated from the Graduated Evidence runbook with per-stage calibration. Appropriate for: multi-stage programs, funded programs with escalating evidence requirements, programs modeled on Development Innovation Ventures-style staging.

*Custom.* No profile is pre-loaded. The funder completes every base configuration field manually. This option is appropriate for funders whose program structure does not match any of the four profiles, for funders who want precise control over every default, or for organizations that are adopting CROSS as part of a broader obligation infrastructure and have their own established defaults they want to encode. Custom configuration takes longer to complete but produces a base configuration that is precisely tailored to the funder's actual practice rather than an approximation from a profile.

After profile selection (or after completing Custom configuration), the funder reviews the full base configuration before confirming it. The confirmed base configuration is version-stamped and stored. It may be updated through the lessons-learned register after each round closes but may not be changed mid-round.

**The inheritance rule.** A new round begins with the base configuration fully loaded. Round-specific criteria layer on top of the base. The round configuration can tighten requirements relative to the base but cannot loosen them. The round configuration cannot lower the conflict of interest tier, cannot raise the token holdings materiality threshold above the base configuration value, cannot deactivate dimensions that are active in the base configuration, and cannot remove or weaken any CROSS minimum standard.

---

## Section 4: Question Sequence for Funder Configuration

The following question sequence is the core of the Configurator. It is the structured interview a program officer completes to generate a round specification. Questions are ordered to allow later questions to depend on earlier answers. The Configurator presents each question, records the answer, maps the answer to CROSS fields and dimensions, and applies field clustering structural conditions (Section 5) before generating the round specification.

An implementer building the Configurator must implement each question as a discrete input with validation logic. All questions are required unless marked optional.

---

**Q0. Program type and runbook selection.**

0.1 Is this a new program configuration or an update to an existing program?

0.2 If new: does this program match any of the standard runbook configurations? Review the runbook library (CROSS-runbooks-0_1_0.md) and select the closest match, or select "Custom configuration."

- [ ] Runbook 1: Discovery Sprint
- [ ] Runbook 2: Staged Development
- [ ] Runbook 3: Community Allocation with Build Obligation
- [ ] Runbook 4: Retroactive Impact
- [ ] Runbook 5: Graduated Evidence
- [ ] Runbook 6: Institutional Conformance
- [ ] Custom configuration (no runbook selected; proceed through the full question sequence)

0.3 If a runbook is selected: the Configurator loads the runbook as the starting gate configuration. Display a summary of the runbook's default gate configuration to the funder. Ask: which fields in the runbook configuration, if any, does this program need to adjust? Note that runbook fields labeled "minimum" may only be tightened, not loosened. Fields labeled "configurable" may be adjusted in either direction within the bounds of the CROSS standard.

0.4 Record the runbook selection (or "Custom") and any adjustments in the round specification under the "Program configuration basis" block.

0.5 Note that the selected runbook also calibrates the rubric preview generated in Q12. Each runbook carries a recommended rubric emphasis: the CROSS rubric criteria that are most load-bearing for that program type, and which are less applicable. The Configurator uses this to pre-weight the Q12 rubric preview before the funder reviews it. A funder selecting a runbook does not commit to its rubric emphasis; they may adjust the rubric in Q12 as with any other configuration step.

---

**Q1. Round identification.**

1.1 What is the name of this round?

1.2 What is the name of the funding organization?

1.3 What is the round opening date?

1.4 What is the round closing date?

1.5 If this is a multi-stage program: what is the stage number of this round (Stage 1, Stage 2, etc.)?

1.6 Who is the named receiving authority for conflict of interest declarations? (Name and role required; this person must be different from any decision-maker in this round.)

---

**Q2. Obligation mode and program structure.**

2.1 What obligation mode does this round operate in?

- [ ] Build obligation: the funded work must produce a specified deliverable
- [ ] Change obligation: the funded work must produce a measurable change in a defined population
- [ ] Retroactive obligation: the application presents evidence of prior demonstrated contribution
- [ ] Multi-stage program with different modes per stage (proceed to Q2.3)

2.2 If a single mode is selected: confirm whether this is the same mode as the program's prior rounds, or whether this round represents a mode transition. Mode transitions in a multi-stage program must be subject to a configured continuation gate (see Q5 below).

2.3 If multi-stage: for each stage in the program, specify:
- Stage number
- Obligation mode for this stage
- Whether this stage is active in the current round or configured for future rounds

The mode assignment per stage is recorded in the program-level configuration and applies to every round at that stage.

2.4 For retroactive obligation rounds: does the program configure a forward commitment requirement? If yes, the forward commitment is assessed under build-obligation criteria (falsifiable deliverable with verifiable completion criteria) and is included in the application form.

---

**Q3. Eligibility domain.**

3.1 What type of work qualifies for this round? Select all that apply: Ethereum ecosystem development, Digital Public Good classification, open source software, open source research or data, protocol infrastructure, public goods infrastructure, civic technology, social impact research, other (specify).

3.2 Is the funder's standing open source requirement in effect? If yes: is open source a hard gate (applicants not releasing under a qualifying open source license are ineligible) or a soft requirement (open source is preferred but not disqualifying)?

3.3 If open source is required: which license or license categories qualify?

3.4 Is Digital Public Good classification required, preferred, or neither?

3.5 Are there organizational type restrictions? Options: incorporated entity only, decentralized autonomous organization only, any organizational form, individual contributors eligible, or specify restrictions.

---

**Q3A. Entry-gate applicant declarations (always collected).**

The CROSS standard (Part IV and Part II) requires that every entry specification gate, in every obligation mode, collect a fixed set of applicant declarations before gate assessment proceeds. These are pre-conditions for assessment, not scored criteria: an entry submission missing any required declaration is incomplete and is not assessed until the declaration is provided. The Configurator does not let a funder switch these declarations off. This question block configures how each declaration appears in the application form and at what evidence strength the funder will hold it. The declarations themselves become locked sections of every application form generated for this round.

3A.1 Organizational identity declaration (required of all applicants, all modes; Part IV). Confirm that the application form collects the six required fields: legal entity name and jurisdiction; parent organization declaration; affiliated entity disclosure; prior round history; disbursement authority (individual, collective, or delegated, with the named holder or mechanism); and on-chain identity anchor (the canonical wallet address used for cross-program identity matching and the Attestation Corpus query in Q14). This declaration is not configurable off. Confirm only the form labels and help text the funder wishes to show.

3A.2 Sufficiency architecture declaration (required of all applicants, all modes; Part IV). Confirm that the form collects the scope declaration, the sufficiency position (one of: critical gap, partial, approaching, surplus, declared at the stated scope), the portfolio context statement, the grant contribution statement, and the revenue architecture declaration (one of: grant-only, fee-for-service, commercial, hybrid; Part II). Set the evidence strength for the sufficiency position: self-report (corroborating evidence accepted but not required) or independent review or above (at least one piece of corroborating evidence from a source outside the applicant's control is required before gate assessment proceeds). Acceptable corroborating sources to name: publicly accessible treasury data, grant history records from a named external database (KarmaGAP, Gitcoin Explorer, RPGF recipient lists, or equivalent), or disclosed revenue figures from a named independent source.

3A.3 Public benefit mechanism and access condition declaration (required wherever eligibility includes any public goods claim; Part II and Part IV). Where Q3 admits any public goods basis, this declaration is active and cannot be configured off. Confirm that the form collects the mechanism type statement (one of: output production, access provision, condition change, ecosystem shift) and the access condition statement, whose required content follows the mechanism type: for output production, the SPDX license identifier and license file location; for access provision, the access mechanism, cost structure, and non-excludability mechanism; for condition change, a FROM state and population definition; for ecosystem shift, a named causal pathway and co-factor list. Specify which mechanism types this round accepts and the evidence scope each requires. The declared mechanism type constrains the evidence scope required at the completion gate (output production commits to output evidence at minimum, access provision to usage evidence, condition change to outcome evidence, ecosystem shift to a documented contribution argument).

3A.4 Development stage declaration (required of all applicants, all modes; Part II and Part IV). Confirm that the form collects the declared stage number (1 through 5), the applicant's account of why their work is at that stage rather than adjacent stages, and at least one piece of evidence from a source outside the applicant's control confirming the declared stage. Declare which stages are within scope for this round. A round that accepts all stages must state this explicitly; a round targeting specific stages must name them and state why other stages are excluded. Stage targeting is published before any applicant submits. The declared stage constrains the coherent obligation mode selections (Part IV).

3A.5 Continuity Capacity declaration (Part II). Confirm the trigger: grants above a funder-defined size threshold, grants producing ongoing infrastructure with continuing operational requirements, and any application where the applying entity has a single named primary contributor with no documented backup capacity. For programs that fund infrastructure maintenance or sustained service delivery, this declaration is always active regardless of threshold. The applicant declares one of three states (single, partial, or resilient) with supporting evidence; a single-point-of-continuity declaration must name the person on whom continuation depends and state what would happen to active grants and funded deliverables if that person became unavailable. Specify whether the completion gate for this round requires evidence of partial or resilient continuity as a condition of final disbursement above the threshold.

3A.6 Obligation fulfillment record (Part IV). Confirm that the form requires an obligation fulfillment record where any of the following hold: the applicant has received prior grants from this funder in any prior round; the applicant cites prior work as evidence of capability at the entry gate; or the applicant's prior round history includes unresolved KarmaGAP milestones or open gate conditions. For each prior grant from this funder, the record documents what was committed at that round's entry gate, what was produced (with a publicly accessible link), and whether the commitment was fulfilled, partially fulfilled, or unfulfilled, with the applicant's explanation where fulfillment was not complete. An undisclosed prior obligation that research surfaces is a material discrepancy under Block J. The funder verifies this record against the Attestation Corpus query configured in Q14.

3A.7 Prior work attribution statement (Part IV). Confirm that the form requires a prior work attribution statement wherever an applicant cites prior work as evidence of capability, track record, or past contribution in any mode. For each cited piece of prior work it asks: the entity of performance (under which legal entity or organizational context the work was performed); the applicant's relationship at the time and its current status; and current ownership and access (who holds the intellectual property rights, who controls the deployment or codebase, and who holds the relationship with any users cited as evidence). This is an adverse signal disclosure requirement, not a scored field.

---

**Q3B. Measurement framework declaration (optional; Part IX).**

3B.1 Does this round declare alignment with an institutional measurement framework? Options: no; yes (select one or more). Recognized declarations: IRIS+ Core Metrics Set (with sub-selection of thematic set), OECD DAC criteria (DCD/DAC(2019)58/FINAL), Logic Model (W.K. Kellogg Foundation), Grant Maturity Index (Biedermann and Gibrel, arXiv:2410.19828), DAOIP-5 (DAOstar/Metagov), and custom.

3B.2 If a framework is declared: the Configurator publishes the framework name and version alongside the gate configuration and pre-populates the external standards section with the framework's canonical reference and a template conformance threshold. A measurement framework declaration does not modify the gate or indicator requirements; it adds a named vocabulary expectation the Configurator exposes to applicants and reviewers. Where OECD DAC alignment is declared, coherence disclosure (Part IX-A) is required at both the entry gate and the progress gate; confirm that the application form carries the coherence disclosure field naming known interventions in the same problem area and characterizing their relationship as complementary, parallel without coordination, duplicative, or in tension.

---

**Q4. Funding amount range for this round.**

4.1 What is the minimum award amount for this round?

4.2 What is the maximum award amount for this round?

4.3 Does this round include tiered award categories? If yes, specify the tiers and their amount ranges.

The Configurator uses Q4 answers to calibrate the Coordination Scaling Standard tier. A round with a maximum award below the small grant threshold may configure all gates at self-report with documentation level. A round with awards above the threshold must configure the completion verification gate at no lower than third-party verifiable level. The Configurator surfaces the applicable tier calibration in the round specification.

---

**Q5. Program-level continuation gate configuration (for multi-stage programs).**

This question block applies only to programs with more than one stage. It configures the continuation gates that apply to progression between stages. These gates are set at the program level, not the round level, and must be published before any round in the program opens.

5.1 Does this program have a program-level continuation gate? Options: yes (multi-stage program with defined progression requirements); no (single-stage or no continuation requirement).

5.2 If yes: for each stage transition in the program (Stage 1 to Stage 2, Stage 2 to Stage 3, etc.), specify the continuation gate configuration:

For each stage transition:
- Evidence scope required: output / usage / outcome / impact
- Evidence strength required: self-report with documentation / third-party verifiable / independent review / independent evaluation
- Obligation mode of the next stage (may differ from the current stage; see Q2.3)
- Infrastructure declaration: if the continuation gate is at independent review level or above, name the reviewer or review body, state their qualifications, describe the review process, and specify the timeline

5.3 For programs configuring Stage 3 or above using the Graduated Evidence runbook: confirm that the cost-effectiveness consideration is active at the Stage 2 to Stage 3 continuation gate. Options: required (the review panel must assess cost-effectiveness before committing Stage 3 funding); advisory (the review panel may consider cost-effectiveness).

5.3a Sustainability assessment at continuation (Part IV). The cost-effectiveness question (whether further investment is worthwhile) and the sustainability question (whether outcomes from prior rounds persist without continued intervention) are different questions and must not be collapsed into one. Confirm that, where a continuation gate is configured, the grantee's continuation submission includes a sustainability stance on outcomes produced in prior rounds, declared as one of three positions: sustained (self-sustaining, no additional intervention required), conditional (persists under specified conditions independent of this program's funding), or dependent (will not persist without continued intervention). A dependent stance is a disclosure, not a disqualifier; a funder continuing a program with a dependent stance is choosing to sustain outcomes rather than only to advance them, and that choice is recorded in the continuation record.

5.3b Causality stance for each continuation pathway (Part IV). For change-obligation continuation gates, declare the causality stance the gate requires: attribution stance (evidence that the intervention caused the observed change; counterfactual reference, configured in Q11, is the standard methodology) or contribution stance (evidence that the intervention plausibly contributed, with a named causal pathway, a list of co-factors, and a written account of why the contribution was material rather than incidental). Contribution stance is appropriate for most public goods and Web3 contexts where multiple funders and community actors contribute to the same ecosystem outcomes. Attribution stance is appropriate where the funder must defend a causal claim to an institutional body, where the intervention is the primary or only active change effort in the target population, or where future funding depends on causal proof. The causality stance is a gate-level configuration: a program may set progress gates at contribution stance and continuation gates at attribution stance as evidence accumulates.

5.4 Record all continuation gate configurations in the program-level configuration block of the round specification. This block is separate from the round-level gate configuration in Q9.

---

**Q6. Public impact claim scope.**

6.1 What is the geographic or network scope of the public impact claims expected in this round? Select one: local (a specific city, region, or named community), regional (multi-country or continental), global, protocol-level (impact claimed at the level of a named protocol or network).

6.2 For change-obligation rounds: does this round require that affected populations be explicitly named and validated? Options: yes, required; yes, required only above a named funding threshold; no, not required for all applicant types.

6.3 For build-obligation rounds: does this round activate the coordinating party engagement dimension? If yes, applicants must document the current absence or inadequacy of the deliverable with named independent evidence, and name at least one external coordinating party who has confirmed the need.

---

**Q7. Track record requirement.**

7.1 What evidence of prior work is required for this round? Select one or more: no minimum track record required; at least one prior funded project in a related domain; verifiable public output from the prior 24 months; prior funding from a named set of programs; other (specify).

7.2 If a track record is required: must prior work be independently verifiable? Options: yes, all claimed prior work must be independently verifiable; yes for work above a named amount; no minimum verification requirement.

7.3 Does this round permit first-time applicants with no prior grants history? If yes, are there compensating requirements (stronger coordinating-party validation, reduced award ceiling, milestone-gated disbursement)?

---

**Q8. Conflict of interest configuration for this round.**

8.1 Does this round override the base configuration conflict of interest treatment? Options: no, apply the base configuration treatment; yes, tighten conflict of interest treatment for this round (permitted); yes, loosen conflict of interest treatment for this round (not permitted; Configurator rejects this option and applies the base configuration).

8.2 Confirm the token holdings materiality threshold for this round. Options: apply the CROSS standard default; apply the base configuration override if one exists; apply a more restrictive threshold for this round (specify).

8.3 Does this round involve any reviewer or committee member from an organization with known token holdings in applicant projects? If yes, the Configurator flags this as requiring pre-round conflict of interest declaration from named individuals before the round opens.

---

**Q9. Optional dimensions.**

9.1 Activate environmental and social impact assessment dimension? If yes: who is the named party with reviewer standing responsible for reviewing classifications submitted by applicants?

9.2 Activate gender equity dimension?

9.3 Activate procurement integrity dimension? Note: if the base configuration has this dimension active, it cannot be deactivated at the round level.

9.4 Activate value for money dimension? (Optional; not a CROSS standard requirement.) If yes: specify the cost-effectiveness methodology the funder will use, or indicate that this is left to reviewer judgment with no specified methodology.

---

**Q10. Round-level common indicators.**

10.1 Are there any outcome indicators required of all applicants in this round, in addition to their self-specified indicators?

10.2 If yes: for each common indicator, provide the following fields (these become fixed entries in every application form for this round):
- Indicator name
- Rationale for selecting this indicator as common to the round
- Measurement form description in plain language (see Part V of the CROSS standard; this replaces the prior constrained data type list)
- Source type classification: on-chain verifiable / off-chain verifiable / qualitative or narrative
- Measurement form classification: quantitative / ordinal / binary / qualitative
- Aggregation type: cumulative / non-cumulative
- Operational definition (inclusion criteria, exclusion criteria, unit of analysis, edge case determination)
- Construction and aggregation methodology
- Disaggregation categories required
- Named data source

Applicants complete the baseline and target fields for each common indicator; the indicator definition itself is locked.

---

**Q11. Round-level gate configuration.**

This question block configures the four gate types for this round. If a runbook was selected in Q0, the Configurator pre-fills this block from the runbook and asks the funder to confirm or adjust. Gate configurations inherited from a runbook must be confirmed before the round specification is generated.

11.1 Entry specification gate.

Confirm that the entry specification gate is active (it is always present). The gate question and acceptance criteria are determined by the obligation mode selected in Q2:
- Build obligation: can the applicant name a falsifiable deliverable with independently verifiable completion criteria?
- Change obligation: can the applicant name the FROM state as a specific measurable condition in a defined population?
- Retroactive obligation: does the applicant present evidence of prior contribution meeting the program's published threshold criteria?

For retroactive obligation rounds: specify the contribution threshold the program will use. This threshold must be published in the round specification before the round opens. The review panel rubric (required for retroactive obligation rounds) is configured in Q12.

11.2 Progress verification gates.

Are there progress verification gates for this round (mid-funding disbursement tranches contingent on demonstrated progress)?

If yes, for each progress verification gate:
- Which tranche does this gate cover (tranche 1, tranche 2, etc.)?
- Evidence scope: output / usage / outcome / impact
- Evidence strength: self-report with documentation / third-party verifiable / independent review / independent evaluation
- Infrastructure declaration: if independent review or above, name the reviewer, their qualifications, the review process, and the timeline
- Milestone or progress description: what must the grantee demonstrate?

11.3 Completion verification gate.

The completion verification gate is always active. Configure:
- Evidence scope: output / usage / outcome / impact
- Evidence strength: self-report with documentation / third-party verifiable / independent review / independent evaluation
- Infrastructure declaration: if independent review or above, provide the full declaration (who reviews, their qualifications, process, timeline)

For build-obligation rounds: confirm that the completion gate requires verification that the specified deliverable is publicly accessible before final payment is released. This requirement is not configurable; it is a CROSS standard minimum.

For completion gates at self-report with documentation level: name the staff member who will review the submission and the timeline for review before final payment.

For all completion gates: confirm that the gate cannot be satisfied by grantee self-report alone at any evidence strength level (Part IV). The funder must review the submission against the published completion criteria and make a documented determination. Confirm that the completion submission requires an unintended outcomes disclosure alongside the primary outcome evidence: any effects, positive or negative, that occurred during the grant period that were not specified at entry and are plausibly connected to the funded work. A grantee who states that no unintended outcomes occurred must state this explicitly; silence does not satisfy the field. An unintended negative outcome is recorded as an adverse signal and triggers the Adverse-Signal Engagement Principle path at the continuation gate.

11.3a Causality stance and counterfactual reference (change-obligation rounds; Part IV).

For change-obligation completion gates, declare the causality stance the gate requires (the same two options as Q5.3b): attribution stance or contribution stance. CROSS requires the stance to be declared explicitly; a gate that leaves it undeclared is operating somewhere between the two positions without saying which.

A gate set to contribution stance requires the grantee to supply a named causal pathway from the funded activity to the observed change, a list of other interventions or actors that also contributed, and a written account of why the funded intervention's contribution was material. It does not require a counterfactual.

A gate set to attribution stance may additionally be configured at counterfactual reference level. Where so configured, name the acceptable counterfactual methods before the round opens (historical trend extrapolation from pre-intervention data, a matched comparison group not exposed to the intervention, or a modeled counterfactual with stated assumptions and sensitivity ranges). A grantee submitting at counterfactual reference level must include a counterfactual baseline, an attribution argument naming the main alternative explanations and why they are insufficient, a defined comparison period or group, and an independent attestation that the method and comparison group are reasonable given the context. Counterfactual reference applies only when explicitly configured here and declared in the infrastructure declaration; it is not implied by selecting outcome evidence scope.

11.4 Continuation specification gate for this round (if applicable).

For rounds that are the final round in a program stage: does a continuation specification gate cover whether the grantee may apply to the next stage? If yes, reference the program-level continuation gate configuration set in Q5 (the program-level gate applies; this question confirms the linkage).

For rounds not at a stage boundary: this gate is not active; record "Not applicable."

11.5 Reporting frequency.

How often must grantees report during the grant period? Options: monthly, quarterly, semi-annually, at milestone completion only, at grant end only, or a named custom schedule.

11.6 Reviewer calibration (required for any gate configured at independent review level or above; Part IV).

For any gate set in this question block to independent review or independent evaluation, the funder must conduct a reviewer calibration exercise before the review window opens, completed before any reviewer assesses any live application. Reviewer calibration is part of the infrastructure declaration for those gates: a gate assessment conducted by a reviewer who did not complete calibration does not satisfy the infrastructure declaration.

Configure the calibration exercise. It must present reviewers with the published gate criteria, their criterion intents, and the conformance threshold for each criterion, and must include at least two worked examples: one application that clearly satisfies the gate criteria and one that clearly does not, each with a documented assessment. Where the review panel includes reviewers from multiple institutions or contexts, the exercise must include a check for inter-rater consistency on the worked examples before live applications are assessed.

Record the calibration plan in the round specification: the gate criteria to be reviewed, the two worked examples, and the named reviewers expected to participate. The calibration record produced at run time (reviewers present, date, gate criteria reviewed, confirmation that calibration was completed) is retained as part of the gate's evidence record.

---

**Q12. Rubric review and confirmation (required for all rounds).**

The rubric is the instrument reviewers use to assess applications against the round's obligation standard. It is a first-class configuration output of the Configurator, not a derived consequence of other choices. The funder must review, customize if needed, and explicitly confirm the rubric before the round specification is generated. The confirmed rubric is locked on publication; it cannot be changed after applications open without re-publishing the round specification with a documented revision reason and a version increment.

12.0 Starting point selection. Before generating the rubric preview, the Configurator asks: where should this round's rubric start from?

- Option A: Generate from current configuration. The Configurator builds the rubric from the obligation mode (Q2), active dimensions (Q9), common indicators (Q10), and runbook-recommended emphasis (Q0) for this round. This is the default for a funder's first round.
- Option B: Start from a prior confirmed rubric. The Configurator displays the rubric history log from the base configuration. The funder selects a prior round's confirmed rubric as the starting point. The selected rubric is then updated to reflect any differences in the current round's mode, dimensions, and common indicators.
- Option C: Start from the funder's default rubric template. If a default template is stored in the base configuration, the funder may select it as the starting point and apply round-specific calibration from there.

The selected starting point is recorded in the "Program configuration basis" block of the round specification so the rubric's origin is traceable.

12.1 Rubric preview generation. The Configurator generates a rubric preview from the starting point selected in 12.0, calibrated to the obligation mode, active dimensions, common indicators, and runbook emphasis for this round. The funder reviews this preview before confirming.

For build-obligation rounds: the pre-generated rubric contains the entry specification gate criteria (deliverable specification and completion criteria assessment), indicator field scoring adapted for build-obligation (Fields 3, 10, and 11 in build-obligation mode), data quality standards assessment, and all three conformance checks.

For change-obligation rounds: the pre-generated rubric contains the entry specification gate criteria (FROM state classification with D1/D2 failure vocabulary), all eleven indicator field scoring criteria, the rigor tier calibration from the Coordination Scaling Standard, data quality standards assessment, and all three conformance checks.

For retroactive obligation rounds: the pre-generated rubric is a framework placeholder that the funder must complete in full in 12.4 below. The Configurator does not pre-populate the substantive scoring criteria for retroactive obligation rounds because the assessment is program-specific.

12.2 Round-specific scoring guidance. Does the funder want to add guidance to any rubric section? If yes, for each addition: name the section, provide the guidance text, and specify whether it is advisory (reviewers read it before scoring but it does not change the scoring scale) or required (reviewers must address it explicitly in their finding). Funder additions may supplement CROSS rubric criteria; they may not lower minimum evidence requirements or waive conformance checks.

12.3 Common indicator rubric criteria. If round-level common indicators were designated in Q10, assessment criteria for each common indicator appear in the rubric automatically. The funder may add specific guidance for how reviewers should score each common indicator against the round's stated goals. If no guidance is added, reviewers apply the standard indicator field rubric to the common indicators.

12.4 Retroactive round rubric (required if obligation mode = retroactive). The funder writes the full assessment rubric. Required elements: what kinds of contribution qualify (eligibility criteria for prior work); how contribution quality is weighted against scale of use; how the review panel resolves disagreements; the minimum threshold for an award; and the minimum evidence strength required (on-chain verifiable, off-chain verifiable, or qualitative/narrative, with independent sources required at a minimum).

12.5 Review panel declaration (required if obligation mode = retroactive). Name the review panel: member names, their qualifications relevant to the contribution area, and the process for handling panel conflicts of interest. A retroactive obligation round with a named panel constitutes independent review at the entry specification gate; all infrastructure declaration requirements from Part IV of the CROSS standard apply.

12.6 Funder confirmation. The funder explicitly confirms the rubric as displayed, including any additions made in 12.2 and 12.3. This confirmation is recorded in the round specification with a timestamp. The Reviewers Dashboard loads the confirmed rubric directly from the published round specification and applies it as the sole scoring criteria instrument for all reviewer assessments in this round.

---

**Q13. Round specification pre-commitment (optional; Part IV).**

A round specification pre-commitment is a publicly queryable record, derived from the complete published round specification before any applicant sees the form, that an independent party can use to confirm the specification existed at a specific point in time before submissions were received. It is the evidentiary basis for applicant redress: an applicant asserting that criteria changed after submission can demonstrate the discrepancy by comparing the committed specification to the criteria as applied. Without a pre-commitment, such a claim is an assertion; with one, it is a documentable discrepancy. Programs whose gate architecture includes summative completion gates with declared redress rights are strongly advised to publish a pre-commitment.

13.1 Does this round publish a pre-commitment to the round specification? Options: yes; no.

13.2 If yes: select the mechanism. The pre-commitment must satisfy two conditions: it must be derivable from the specification document so that any party can verify the match between the commitment and the specification in force, and it must carry a timestamp from a source outside the program's own control. On-chain transactions, signed timestamps from recognized timestamping authorities, and equivalent mechanisms all satisfy these conditions. The Configurator does not require any specific mechanism; it records which one the funder uses.

13.3 Record the commitment reference in the published round specification so that any party can verify the match between the committed document and the specification applied.

---

**Q14. Structured dataset publication and Attestation Corpus query (Part IV and Part IX).**

14.1 Funder-side Attestation Corpus query. The CROSS standard requires that, for each application providing an on-chain identity anchor (collected in Q3A.1), the reviewing program query the Attestation Corpus for that address across named public sources before gate assessment is complete. This is a funder-side procedure, not an applicant submission requirement. Confirm the query is part of this round's evaluation process and configure its sources. Required query sources: on-chain attestation registries (EAS deployments on Ethereum mainnet, Optimism, Base, and Arbitrum at minimum), the KarmaGAP grants and milestone API, and any program-specific grant databases this round names. The query returns total non-revoked attestations, attestations by known schema (KarmaGAP, RPGF, Gitcoin, and other named programs), and endorsement count and endorser identities where resolvable.

14.2 Reconciliation with the obligation fulfillment record. Confirm that the query result is recorded in the evaluation record alongside the obligation fulfillment record collected in Q3A.6. Where the Attestation Corpus reveals prior grants, milestones, or obligations not disclosed in the applicant's obligation fulfillment record, this is non-disclosure of a prior obligation and is treated as a material discrepancy under the adverse signal provisions of Part IV.

14.3 Structured dataset publication. The conformant configuration records and publishes, before the round opens, the round-level data the standard requires be legible (Part IX): whether concurrent funding is present and the resulting additionality requirements; external standard references for each gate, each with an identifier, version anchor, scope, and conformance threshold; the program's funder-side obligation configuration (internal clarification mechanism, structured appeals procedure, and independent redress mechanism status); and the field clarity gate outcome for each application field. Confirm the publication format the program uses (the Configurator does not require a specific one; structured JSON, an on-chain schema record, or any tabular format that carries these elements is conformant). The field clarity gate requires that each application field carry a criterion specification meeting Part IV requirements before the round opens; fields that do not are flagged and must be resolved or overridden with documented justification before publication.

---

## Section 5: Field Clustering Structural Conditions

Field clustering structural conditions specify when a particular answer to the question sequence triggers additional required fields automatically. Clustering is deterministic: if the trigger condition is met, the additional fields become required in the round specification. Funders cannot override clustering structural conditions; they are inherited from the CROSS standard.

**Condition 1.** If measurement form classification = quantitative with composite construction (multiple weighted components) for any common indicator: the component specification, weighting, and aggregation rule fields for that indicator become required. A composite indicator without these three fields is unverifiable and does not satisfy the CROSS data quality standard.

**Condition 2.** If any applicant invokes the privacy-sensitive accommodation: the specific harm field and the alternative methodology field both become required. The accommodation is not an exemption from obligation; it substitutes an appropriate methodology.

**Condition 3.** If any venture capital or institutional investment is disclosed in the concurrent funding disclosure: the expanded concurrent funding fields become required for that applicant: investor name, approximate investment amount, decision rights held by the investor, and the documented relationship between the commercial investment scope and the public goods scope of this application.

**Condition 4.** If the environmental and social impact dimension is activated (Q9.1): the classification field (Category A, B, or C under the International Finance Corporation Performance Standards derived classification) becomes required for all applicants within scope. Applicants self-classify; the named party with funder standing reviews and may reclassify.

**Condition 5.** If round-level common indicators are designated (Q10.1 = yes): those indicators are pre-populated in all application forms with their measurement form descriptions, operational definitions, construction methodologies, and disaggregation categories. These fields are locked for applicants; applicants complete the baseline and target fields only.

**Condition 6.** If progress verification gates are configured (Q11.2): milestone or progress specification fields become required for every application in the round. Required fields for each milestone: milestone name, description, evidence type (artifact, deployed system, published report, outcome data, or other), verification method, expected completion date, and disbursement amount contingent on this milestone. At least one milestone must be designated as a verification milestone where an independent party confirms the deliverable.

**Condition 7.** If the procurement integrity dimension is activated (Q9.3) and an applicant's proposed budget includes sub-contracting, sub-granting, or re-granting exceeding 20% of the total award: sub-contractor disclosure fields become required for that applicant.

**Condition 8.** If the adverse signal disclosure field reveals a prior rejection from a program with substantially similar eligibility criteria: the applicant must complete the adverse signal response field naming the program, the stated rejection reason, and what has changed since that is material to this application.

**Condition 9.** If the track record requirement in Q7.2 requires independent verification and an applicant claims prior funded work: all claimed prior work must include a verifiable public link or named third-party source.

**Condition 10.** If the gender equity dimension is activated (Q9.2) and an applicant claims population-level impact: gender-disaggregated reporting fields become required for all impact indicators measured at the individual or household unit of analysis.

**Condition 11.** If obligation mode = retroactive (Q2.1): the prior award disclosure field becomes required for all applicants. All prior awards for the same or substantially overlapping contribution must be disclosed. This disclosure is in addition to the standard concurrent funding disclosure (Template 4).

**Condition 12.** If a program-level continuation gate is configured (Q5.1 = yes) and this round is at a stage boundary: the continuation gate evidence requirements are surfaced in the application form as a forward-looking section.

**Condition 13.** If round-level common indicators are designated (Q10.1 = yes): the rubric confirmation step (Q12) must include explicit assessment criteria for each common indicator. The Configurator surfaces these criteria automatically in the rubric preview at Q12.1. If the funder skips Q12 without addressing the common indicator criteria, the round specification cannot be generated. The confirmed rubric must cover every indicator applicants are required to report. Applicants must acknowledge the continuation gate requirements before submitting, and the Grantee Dashboard will track the evidence required for the continuation gate alongside the round completion verification evidence.

---

## Section 6: Round Specification Output Format

The round specification is the output of the Configurator. An implementer must generate a round specification containing all of the following elements.

**Round identification block.** Round name, funder name, round opening date, round closing date, stage number (if multi-stage), version number of the round specification, and the named conflict of interest receiving authority.

**Program configuration basis.** The runbook selected in Q0 (or "Custom configuration") and any adjustments made to the runbook default values. This block creates a traceable record of how the program's configuration relates to the standard starting configurations.

**Obligation mode declaration.** The declared obligation mode for this round (build, change, or retroactive). For multi-stage programs: the mode assignment for each stage, displayed in a stage-by-stage table.

**Eligibility criteria in structured form.** The eligibility domain answers from Q3, rendered as a list of qualifying and disqualifying binary conditions.

**Active obligation dimensions.** An enumeration of all obligation dimensions active for this round. For each active dimension: the dimension name, the triggering condition, and a brief statement of what the dimension requires applicants to demonstrate.

**Gate configuration block.** For each of the four gate types: entry specification, progress verification (one sub-block per tranche), completion verification, and continuation specification. Each sub-block contains: the evidence scope, the evidence strength, and the infrastructure declaration. For gates at independent review level or above: the named reviewer or review body, their qualifications, the review process, and the timeline.

**Program-level continuation gate block.** For multi-stage programs: the continuation gate configuration for each stage transition, including evidence scope, evidence strength, mode of the next stage, and infrastructure declaration. This block is separate from the round-level gate configuration block and is reproduced from the program-level base configuration.

**Required application fields.** A complete list of all fields applicants must complete, including: core CROSS fields, entry specification fields (mode-specific: deliverable specification form for build-obligation, FROM/TO specification for change-obligation, prior contribution form for retroactive), dimension-specific fields, clustering-condition-triggered fields, and common indicator fields if any.

**Entry-gate applicant declaration blocks.** The locked declaration sections every application form carries, configured in Q3A: the organizational identity declaration (six fields), the sufficiency architecture declaration (five elements with the configured evidence strength for the sufficiency position), the public benefit mechanism and access condition declaration where a public goods claim is in scope (mechanism type and access condition, with the accepted mechanism types named), the development stage declaration with the round's in-scope stages and the published exclusion rationale, the Continuity Capacity declaration with its trigger and any completion-gate continuity condition, the obligation fulfillment record with its triggering conditions, and the prior work attribution statement. Each block names the field set and the evidence strength at which the funder holds it.

**Measurement framework declaration.** If declared in Q3B: the framework name and version, the pre-populated external standards reference and template conformance threshold, and, where OECD DAC alignment is declared, the coherence disclosure field at both the entry and progress gates.

**Causality stance block.** For change-obligation rounds: the declared causality stance (attribution or contribution) for each outcome-bearing gate, and, where attribution stance is configured at counterfactual reference level, the acceptable counterfactual methods named before the round opens.

**Reviewer calibration plan.** For any gate configured at independent review level or above: the calibration plan from Q11.6, comprising the gate criteria to be reviewed, the two worked examples, and the named reviewers expected to participate. This plan is part of the infrastructure declaration for those gates.

**Round specification pre-commitment reference.** If a pre-commitment is published (Q13): the commitment reference and the mechanism used, recorded so any party can verify the match between the committed document and the specification applied.

**Structured dataset and Attestation Corpus query configuration.** The published round-level dataset elements from Q14.3 (concurrent funding presence and additionality requirements, external standard references, funder-side obligation configuration, and field clarity gate outcomes), the configured Attestation Corpus query sources from Q14.1, and the reconciliation procedure from Q14.2.

**Conflict of interest configuration for this round.** Which tier treatment applies, the token holdings materiality threshold, the named receiving authority, the pre-round declaration requirement and deadline, and the post-participation certification requirement.

**Round-level common indicators.** If common indicators were designated in Q10: the fully specified common indicator block for each one, reproduced verbatim in every application form.

**Confirmed rubric block.** The rubric as confirmed by the funder in Q12. This is not a reference to the companion rubric document; it is the full rubric text, generated from the CROSS assessment rubric (CROSS-common-reporting-outcome-standards-schema-rubric-0_2_0.md) as the base, calibrated to this round's obligation mode and active dimensions, supplemented by any funder additions from Q12.2, and extended with common indicator criteria from Q12.3 if applicable. For retroactive obligation rounds: the rubric is the funder-authored text from Q12.4. The rubric confirmation timestamp and the confirming funder standing are recorded alongside the rubric text. The Reviewers Dashboard loads this block directly; it does not re-derive the rubric from the companion document at runtime. The rubric is included in the published round specification so reviewers and applicants read the same confirmed instrument.

**For retroactive obligation rounds: review panel block.** The named panel members, their qualifications, and the conflict of interest handling process for panel members.

**Reporting frequency and disbursement schedule.** The reporting frequency selected in Q11.5, expressed as a schedule with named reporting periods and due dates. The disbursement schedule expressed as disbursement amounts, gate trigger conditions, and the verification contact responsible for confirming each trigger condition.

**Verification contacts.** A named contact for each gate verification requirement. Each contact entry includes name, role, and the specific gate or condition they are responsible for verifying. Where an independent third party is the verification contact, their organizational affiliation is included.

---

## Section 7: Configuration Inheritance Across Rounds

Each round closes with a structured post-round review. The purpose is to identify gaps, failures, and unanticipated patterns from the closed round and absorb fixes into the base configuration.

The Configurator supports this through a lessons-learned register attached to the base configuration. Each entry contains: the round in which the issue was identified, a description of the issue, the remediation taken within that round, and the base configuration change made to prevent recurrence.

The following categories of findings should prompt base configuration updates.

If a concurrent funding non-disclosure was discovered post-award: review the disclosure field for completeness and tighten the definition in the base configuration if the non-disclosure exploited an ambiguity.

If a conflict of interest relationship was discovered post-award that was not captured by the existing tier definitions: document the relationship type and update the base configuration to cover it.

If an outcome indicator proved unmeasurable, unverifiable, or structurally flawed: document the failure mode. If likely to recur, the base configuration can add round-level guidance flagging that indicator category and its specific failure pattern.

If a field clustering structural condition failed to trigger in a case where it should have triggered: document the missed trigger and update the Configurator's clustering structural condition implementation.

If a gate was configured at a level the funder could not operationally support (for example, independent review was committed but no reviewer was arranged in time): document the infrastructure gap and update the base configuration or runbook guidance to flag the operational requirement.

If reviewer assessments showed inconsistent interpretation of a rubric criterion (for example, two reviewers gave materially different scores to the same application on the same field): document the criterion, describe the interpretive gap, and either add funder guidance to the criterion in the default rubric template or propose an update to the CROSS rubric companion document if the ambiguity is structural. The rubric history log entry for that round should include a brief note on which criteria produced scoring inconsistency. This note is available to the funder when selecting that round's rubric as a starting point for a future round.

**Funder maturation tracking.** A funder operating within a CROSS-conformant program records their gate configuration for each round. In programs operating within the Proof of Coordination protocol, gate configurations are tracked across rounds, making funder maturation visible over time. The lessons-learned register and the sequence of round specifications are the primary record of this maturation. The Configurator supports this by maintaining a versioned history of base configuration changes with their associated rationales.

The lessons-learned register is reviewed at the start of each new round configuration session. Open items from a prior round that have not been absorbed into the base configuration are surfaced as required decisions before the new round specification is generated.

---

## Section 8: Forward-Looking Considerations

**Cross-funder interoperability.** When multiple funders each operate the Configurator with different base configurations, their round specifications are structurally compatible. Field names are drawn from the CROSS standard and are identical across funders. A grantee's CROSS obligation record from one round is readable and directly comparable by a reviewer at a different funder assessing a subsequent application from the same grantee. Cross-funder portability does not require funders to coordinate their eligibility criteria or conflict of interest configurations; it requires only that each funder's Configurator implementation conforms to the field definitions in the CROSS standard.

**Onchain publication of round specifications.** A round specification generated by the Configurator can be published as an onchain schema definition. The schema hash recorded onchain provides a reference point against which application forms, grantee reports, and disbursement records can be verified. Retroactive modification of a round specification after applications have been received is detectable because the published schema hash would not match the modified document. The mechanism for onchain publication is an implementation decision for the organization deploying the Configurator; the round specification output format defined in Section 6 is structured to be compatible with this.

**Connection to the Grantee Dashboard.** The Grantee Dashboard (CROSS-grantee-dashboard-0_2_0.md) is the post-award tool that converts the round specification into a live obligation record for each funded project. The Grantee Dashboard ingests the round specification as its input. From it, the Dashboard derives the indicator schema, the entry specification form type (build, change, or retroactive), the gate configuration, the disaggregation ratchet, the reporting schedule, and the disbursement conditions for each grantee. The Configurator and the Grantee Dashboard are designed as a pair: the Configurator defines the schema; the Grantee Dashboard populates it. A round specification generated by a conformant Configurator should be directly ingestible by a conformant Grantee Dashboard without requiring schema translation or manual field mapping.

**Connection to the Reviewers Dashboard.** The Reviewers Dashboard (specification forthcoming) is the stage-gated review interface for evaluators. It ingests the round specification to load the correct rubric for the round's obligation mode, configure the conflict of interest declaration gates, and assign applications to reviewers. The Configurator's mode declaration (Q2) and gate configuration (Q11) are the primary inputs the Reviewers Dashboard uses to configure its evaluation stage. A well-formed round specification produced by the Configurator eliminates the need for manual rubric configuration in the Reviewers Dashboard.

**Versioning and amendment.** The round specification carries a version number. The initial published version is 1.0. Material amendments increment the version number and require a documented revision reason. Minor amendments may be issued as patch versions with a changelog entry. All versions of a round specification are retained in the funder's configuration history.
