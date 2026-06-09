---
title: CROSS Reviewers Dashboard
version: 0.2.1
date: 2026-06-08
license: CC0
status: Working draft. Companion implementation specification synced to CROSS-common-reporting-outcome-standards-schema-0_5_0.md. Supersedes version 0.1.0.
related_documents:
  - standards/CROSS-common-reporting-outcome-standards-schema-0_5_0.md
  - standards/CROSS-grant-configurator-0_2_0.md
  - standards/CROSS-grantee-dashboard-0_2_0.md
  - standards/CROSS-common-reporting-outcome-standards-schema-rubric-0_2_0.md
changelog:
  - "0.2.1 (2026-06-08): Frame Language own-voice pass. Own-voice watchlist terms were replaced with the structural act each names (enforce and enforces became requires or applies; the Governing standard became the Applicable standard). The Attestation integrity section and its provision references became Attestation independence, matching the spec Part VII rename. Conflict-of-interest category names, governance-token COI categories, framework names, and the changelog rows were preserved. Em-dash sweep clean. No conflict-of-interest tier, gate, or requirement changed; vocabulary and naming only."
  - "0.2.0 (2026-06-05): Synced to the 0.5.0 CROSS specification. Encoded the three-tier conflict of interest declaration (Tier 1 categorical bar with no waiver, Tier 2 disclosure with qualified waiver, Tier 3 disclosure encouraged) as enforced in the application-level declaration gate. Added the attestation-integrity provision: a Tier 1 conflicted party may not sign attestations and a Tier 2 conflicted party requires a qualified waiver before serving as attestor (spec Part VII). Added the round-level Cohort Position assessment for personnel, wallet, and endorser overlap across applicants. Added funder-side consulting conflicts and the organizational role conflict to the declaration form and waiver handling. Added the reviewer calibration gate that must complete before any reviewer assesses a live application (spec Part IV). Added assessment access for the new entry-gate dimensions (organizational identity, sufficiency architecture, public benefit mechanism, development stage, obligation fulfillment record, Attestation Corpus query). Noted CRAFT inheritance where relevant (spec Part XIII). Data model extended for each addition."
  - "0.1.0 (2026-05-14): First draft. Stage-gated evaluation interface with conflict of interest declaration gates, assessment isolation, role differentiation, rubric loading, and three-layer AI assistance."
---

# CROSS Reviewers Dashboard

Version 0.2.1 | 2026-06-08 | CC0

---

## Section 1: Purpose and Scope

The CROSS Reviewers Dashboard is the stage-gated interface through which grant evaluators assess applications against the round's published obligation standard. It is the fourth operational tool in the CROSS implementation architecture, alongside the Grant Configurator, the Grantee Dashboard, and the CROSS skill.

The Reviewers Dashboard serves a distinct set of functions that neither the Grant Configurator nor the Grantee Dashboard can perform. The Configurator defines the round's obligation schema. The Grantee Dashboard tracks post-award performance. The Reviewers Dashboard runs the evaluation stage: the period between applications closing and funding decisions being made. During this stage, the Reviewers Dashboard requires reviewer calibration before any live assessment, requires three-tier conflict of interest declarations as access controls, applies the attestation-independence provision where it records independent-review attestations, runs the round-level Cohort Position assessment across applicants, maintains assessment isolation between reviewers, surfaces the entry-gate declarations for assessment, loads the correct rubric for the round's configured obligation mode, and provides AI-assisted evaluation support.

The Reviewers Dashboard is active only during the evaluation stage. Before applications close, it has no function. After funding decisions are made and communicated, it closes again. This boundary is applied structurally, not by convention: the Dashboard's application content access is gated to the evaluation window as configured in the Grant Configurator, and no reviewer including program administrators can access application content outside that window through the Dashboard interface.

The primary output of the Reviewers Dashboard is the evaluation record: a structured set of per-application assessments that the funder uses to make funding decisions. Each evaluation record contains the reviewer's scored rubric assessment, conformance check findings, and recommendation, alongside the AI assistance outputs that informed it. The evaluation record is the obligation instrument for the review process itself.

---

## Section 2: Evaluation Stage Gating

The evaluation stage opens when the program administrator sets the stage to active in the Grant Configurator or in the Reviewers Dashboard administrative interface. It closes when the program administrator marks it closed, or when the configured evaluation window duration elapses.

While the evaluation stage is open, reviewers with assigned roles can access applications assigned to them, subject to the conflict of interest handling described in Section 3. While the evaluation stage is closed, no reviewer can access application content regardless of their role. This includes lead reviewers and funder administrators: the stage gate is not a role permission; it is a temporal gate that applies universally.

The evaluation window duration and the process for opening and closing the stage are configured in the Grant Configurator (Q1 of the Configurator's question sequence includes the named conflict of interest receiving authority; the Reviewers Dashboard uses the same named authority as the gatekeeper for stage transitions). Funders may configure automated stage opening tied to the round's published close date, or manual stage opening requiring a named administrator action.

The Reviewers Dashboard records the exact timestamp at which the evaluation stage opened and at which it closes. These timestamps become part of the institutional record for the round.

### Reviewer calibration gate

For any gate configured at independent review level or above, the funder must conduct a reviewer calibration exercise before the review window opens, completed before any reviewer assesses any live application (spec Part IV). The Reviewers Dashboard requires this as a precondition gate: a reviewer who has not completed calibration for the round cannot open any live application, regardless of role or conflict of interest status. A gate assessment conducted by a reviewer who did not complete calibration does not satisfy the funder's infrastructure declaration for that gate.

The calibration exercise the Dashboard presents includes the published gate criteria, their criterion intents, and the conformance threshold for each criterion, together with at least two worked examples: one application that clearly satisfies the gate criteria and one that clearly does not, each with a documented assessment. Where the review panel includes reviewers from multiple institutions or contexts, the Dashboard includes a check for inter-rater consistency on the worked examples before live applications are assessed; it records each calibrating reviewer's worked-example assessment so that the program administrator can confirm consistency before opening live access.

The Dashboard records the calibration result as part of the round's evidence record: the reviewers present, the date, the gate criteria reviewed, and confirmation that calibration was completed. The calibration record is retained alongside the evaluation stage timestamps and transfers to the institutional record (see Section 9).

---

## Section 3: Conflict of Interest Handling

Conflict of interest declaration is not a pre-condition the Reviewers Dashboard asks reviewers to confirm at login. It is a gate applied at the application level: a reviewer who has not submitted a valid conflict of interest declaration for a specific application cannot open that application. The gate operates independently for each reviewer-application pair.

The declaration covers all three tiers of the CROSS conflict of interest framework (spec Part VII). The applicable standard the declaration form states to the reviewer is the reasonable third party standard: would an informed observer with knowledge of the relevant facts conclude that the reviewer cannot maintain independence and is therefore not capable of objective and impartial judgment? The checklist the form presents for each tier illustrates the standard; it does not exhaust it. A reviewer who identifies a novel relationship type not on the checklist that meets the reasonable third party standard is required to declare it, and the Dashboard provides a free-text relationship field for this purpose. Tier assignment is determined by relationship type, not by the round's funding amount or obligation mode; the Dashboard applies the same three tiers in a small-grant build-obligation round as in any other.

### Declaration gate behavior

When a reviewer attempts to open an application for which they have not submitted a conflict of interest declaration, the Dashboard presents the declaration form (Template 6 from the CROSS templates document) before allowing access to application content. The reviewer must complete the declaration and submit it to the named receiving function before the application opens. The named receiving function is separate from the person making the funding decision (spec Part VII).

The declaration is application-specific, not round-level. A reviewer who declares no conflicts for Application A and a Tier 2 conflict for Application B cannot open Application B until the Tier 2 conflict has been resolved through the waiver process. The reviewer may continue reviewing Application A while the waiver for Application B is pending.

### Tier 1 named response

Tier 1 is a categorical bar with no waiver. The declaration form surfaces the Tier 1 relationship types from spec Part VII: a direct financial interest in the applicant entity (equity, revenue share, or token holdings above the materiality threshold, which defaults to greater than 1 percent of circulating supply or greater than 5,000 United States dollars in value at the time of review); a family relationship with any principal, director, officer, or owner of the applicant project; prior receipt of funding from this funder in the same program area where the reviewer's funded work is directly related to the applicant's scope; and being named as a team member, advisor, or contributor on the applicant project's public materials, whether compensated or not.

If a reviewer's declaration for a specific application indicates a Tier 1 relationship, the Dashboard blocks access to that application for that reviewer permanently for this round. The block is not reversible by the reviewer; only a program administrator can remove a Tier 1 block, and only for the purpose of reassigning the application to a non-conflicted reviewer. The Tier 1 block and the relationship it identified are recorded in the evaluation record for that application. Non-disclosure of a Tier 1 relationship that is later discovered is a disqualifying violation under spec Part VII; the Dashboard records the discovery and the relationship in the evaluation record.

### Tier 2 named response

Tier 2 is disclosure required with a qualified waiver possible. The declaration form surfaces the Tier 2 relationship types from spec Part VII: employment with the applicant organization in the past 36 months; co-authorship or active project collaboration with applicant principals in the past 48 months; a mentor or student relationship with applicant principals (no expiration); voting power exercised on proposals affecting the applicant project; co-membership in coordinating or committee roles within the same decentralized autonomous organization as the applicant; having received an honorarium, award, or gift from the applicant entity in the past 12 months; active job negotiations or arrangements for future employment with the applicant organization; an organizational conflict where the reviewer's employer has a material financial relationship with the applicant; and the organizational role conflict described below.

If a reviewer's declaration indicates a Tier 2 relationship, the Dashboard blocks access to that application until either: a waiver is approved by the named receiving function and recorded in the Dashboard, or the reviewer elects recusal. A qualified waiver requires, per spec Part VII, a written justification submitted to a named authority other than the conflicted party, approval granted before participation rather than after, and documentation in the review record. The Dashboard requires this sequence: the waiver record must carry the approver's identity, the justification submitted, and the timestamp, and the approver identity must differ from the reviewer requesting the waiver. A waiver is not available where the relationship creates a financial interest; the Dashboard routes any Tier 2 relationship the reviewer flags as financial to the Tier 1 block path. The waiver approval is accessible to the program administrator and is included in the institutional record for the round. Non-disclosure of a Tier 2 relationship that is later discovered is a process violation requiring remediation under spec Part VII; remediation options recorded by the Dashboard are retroactive recusal, review restart with a non-conflicted panel, or award cancellation, depending on the degree of influence the conflicted party had.

### Organizational role conflict

The Tier 2 declaration includes the organizational role conflict (spec Part VII). A reviewer must declare any paid or unpaid leadership, advisory, or operational role they hold in another organization that is applying to this round, or that received awards from this funder in the most recent prior round in the same program area. The declaration form states that this disclosure is required even when no direct financial relationship exists between the reviewer and the applicant under review: the structural position across multiple funding relationships is itself the conflict. The Dashboard handles a declared organizational role conflict through the Tier 2 waiver path.

### Funder-side consulting conflicts

Where a reviewer is under a paid consulting or service contract with the funder at the time of evaluation, the declaration form requires that relationship to be disclosed to the named receiving function regardless of its connection to any specific applicant (spec Part VII). The disclosure is required for any paid engagement covering the same program area as the applications under review, including review contracts, evaluation support, research commissions, and advisory retainers.

The Dashboard routes a funder-side consulting disclosure by its scope. Where the consulting arrangement covers the same program area as the applications under review, a Tier 2 qualified waiver applies, handled through the waiver path above. Where the consulting arrangement constitutes the primary mechanism through which the reviewer receives income from the ecosystem being evaluated, a categorical bar applies and the Dashboard blocks the reviewer from that round's applications with no waiver available. This bar does not require the reviewer to have a direct financial relationship with any specific applicant; structural income dependency on the funder's continued operation and on favorable award decisions is itself the conflict. The Dashboard records the funder-side consulting disclosure and its routing in the conflict of interest record for the round.

### Tier 3 disclosure

Tier 3 is disclosure encouraged, with the reasonable third party standard applying. The declaration form presents the Tier 3 relationship types from spec Part VII: social and community relationships (conference co-speakers, forum co-membership, shared group chats); prior interactions across grant rounds in different program areas; and informal mentorship or advisory conversations without ongoing engagement. A Tier 3 disclosure does not block application access. It is recorded in the conflict of interest record for the application and is available to the program administrator and the lead reviewer, so that a reviewer's pattern of declared social and community relationships is visible when assessment divergences are reconciled.

### Attestation independence

The conflict of interest framework runs in both directions and applies to attestors confirming completion evidence, not only to reviewers assessing applications (spec Part VII). Where the Reviewers Dashboard records or accepts an attestation confirming an applicant's gate evidence at independent review evidence strength or above, it applies the attestation-independence provision.

A party who holds a Tier 1 conflict with an applicant may not serve as the independent reviewer or sign an attestation confirming that applicant's gate evidence, regardless of the attestation format used. The Dashboard treats a Tier 1-conflicted party's signed on-chain attestation, signed document, or issued credential as not satisfying the independent review requirement; the attestation does not meet the evidence strength standard regardless of its format. A party who holds a Tier 2 conflict with an applicant requires a qualified waiver before serving as attestor for that applicant, using the same waiver procedure as the reviewer waiver requirement above. The Dashboard verifies reviewer and attestor conflict status before accepting any attestation as satisfying independent review evidence strength. This provision applies to all mechanisms by which gate evidence is independently confirmed at any gate configured at independent review level or above. (This realizes CRAFT's non-self-adjudication invariant through ex-ante designated attestation, spec Part XIII, Condition 5.)

### Post-participation certification

When a reviewer submits their final assessment for an application, the Dashboard presents the post-participation certification form (Template 8) before the submission is accepted. The reviewer confirms that no new conflicts arose during review and that their pre-review declaration remained accurate. The certification is recorded alongside the assessment.

### Round-level Cohort Position assessment

Before final gate determinations are issued for a round, the Dashboard surfaces a round-level Cohort Position assessment across all applicants (spec Part VII, derived from the Cohort Position primitive, CROSS+WALKRI Primitives Foundation, Layer 7). This is a round-level procedure available to the funder administrator, not a per-reviewer-per-application gate. The assessment checks three forms of overlap across applicants in the same round.

Personnel overlap: whether any named team member, contact, or key contributor in one application also appears in another application in the same round under a different entity name. Where personnel overlap is found, it does not disqualify either application; the Dashboard triggers a Tier 2 conflict of interest disclosure requirement for the overlapping individual, routed through the declaration gate above.

Wallet overlap: whether any on-chain identity anchor or disbursement authority address in one application appears as a recipient, controller, or named address in another application in the same round. Wallet overlap requires explanation. The same address appearing across multiple distinct legal entities applying separately is a material discrepancy that the Dashboard flags for reconciliation before disbursement.

Endorser concentration: whether the same identifiable party has endorsed or attested to a disproportionate share of applicants in the same round using non-standard schemas. Endorser concentration is informational; the Dashboard records it in the round record without disqualifying effect.

The Cohort Position assessment draws on the organizational identity declaration and the Attestation Corpus query for each application (see Section 5A). Its results are recorded in the round-level conflict of interest record and transfer to the institutional record (see Section 9).

### Conflict of interest record in the evaluation output

The evaluation record for each application includes a conflict of interest summary: which reviewers declared which relationships at each tier, which Tier 1 blocks applied, which Tier 2 waivers were granted, which funder-side consulting and organizational role conflicts were declared and how they were routed, and which post-participation certifications were completed. The round-level record additionally carries the Cohort Position assessment results and any attestor conflict status checks. This summary is part of the institutional record that transfers to the PoC vault (see Section 9).

---

## Section 4: Assessment Isolation

Reviewers cannot see other reviewers' assessments for an application until they have submitted their own assessment for that application. This isolation prevents anchoring effects, where an early reviewer's score or finding influences subsequent reviewers toward conformity rather than independent judgment.

Assessment isolation is applied at the data access level, not by convention. A reviewer who has submitted their assessment for an application may see other submitted assessments for that application, subject to the role permissions in Section 5. A reviewer who has not yet submitted cannot see any other assessment for that application regardless of role.

The isolation boundary is the submission act. Saving a draft does not count as submission. The reviewer must explicitly submit their assessment before the isolation lifts.

### Lead reviewer aggregation view

Lead reviewers have access to an aggregate view that shows, for each application, which reviewers have submitted and which have not, without revealing the content of submitted assessments to reviewers who have not yet submitted their own. The aggregate view is available to lead reviewers to manage the review process timeline; it does not enable the lead reviewer to see assessment content before submitting their own.

Once a lead reviewer has submitted their own assessment for an application, they gain access to all submitted assessments for that application. This enables the lead reviewer to identify divergences among guest reviewer assessments and initiate the reconciliation process described in Section 6.

### Isolation configuration

Funders may configure perpetual isolation: submitted assessments remain invisible to all reviewers until the program administrator closes the evaluation stage. This configuration is appropriate for programs where full independence is paramount and there is no deliberative process between individual reviewer submission and the final funding decision. Under perpetual isolation, lead reviewers cannot see individual assessment content until the stage closes.

---

## Section 5: Role Differentiation

The Reviewers Dashboard distinguishes three access roles. Roles are assigned by the program administrator in the Grant Configurator or in the administrative interface of the Dashboard before the evaluation stage opens.

**Guest reviewer.** A guest reviewer sees only the applications assigned to them by the program administrator or lead reviewer. They do not see the full applicant list, other reviewers' identities or assignments, or assessment content from other reviewers (subject to the isolation rules in Section 4). Guest reviewers submit conflict of interest declarations, complete AI-assisted evaluation, and submit their assessments. They do not have administrative access to any round-level configuration.

This role is the appropriate configuration for invited external reviewers, community evaluators, or domain experts who are brought in for a specific round with a specific assignment set. The role isolation ensures that their participation does not expose them to the full applicant pool or to deliberative information that would not be appropriate for an outside evaluator.

**Lead reviewer.** A lead reviewer sees all applications in the round and all submitted assessments (subject to isolation rules until they have submitted their own assessment for each application). They may assign applications to guest reviewers, view the conflict of interest summary for any application, and initiate assessment reconciliation when guest reviewer assessments diverge substantially. Lead reviewers have the same access to AI assistance as guest reviewers. They have no administrative access to round configuration.

**Funder administrator.** A funder administrator holds all lead reviewer permissions plus the ability to: open and close the evaluation stage, approve Tier 2 conflict of interest waivers (as the named receiving function), configure guest reviewer and lead reviewer assignments, access the full conflict of interest record for the round, run the round-level Cohort Position assessment (Section 3), and export the complete evaluation record for institutional archival. Funder administrators may not modify submitted assessments. They may flag an assessment for re-review with a documented reason, which reopens the assessment for the reviewer who submitted it.

---

## Section 5A: Entry-Gate Declaration Access

When a reviewer opens an application that has passed the declaration gate and calibration, the Dashboard surfaces the applicant's entry-gate declarations alongside the application narrative, so that the reviewer can assess them against the entry specification gate (spec Part IV). These declarations are pre-conditions for gate assessment in the standard: an entry gate submission that omits a required declaration is incomplete and is not assessed until the declaration is provided. The Dashboard flags any missing required declaration as an incomplete submission rather than presenting it as a scored finding.

The reviewer interface surfaces the following entry-gate declarations for assessment.

**Organizational identity declaration.** The Dashboard presents the four required fields (spec Part IV): the legal entity name and jurisdiction, the parent organization declaration, the affiliated entity disclosure, and the prior round history, together with the disbursement authority and the on-chain identity anchor. The reviewer assesses these for completeness and for consistency with the Layer 2 independent investigation (Section 7). The interface highlights where a publicly documentable affiliation or a publicly associated on-chain address was not disclosed, since non-disclosure of either is a conformance failure under the standard.

**Sufficiency architecture declaration.** The Dashboard presents the scope declaration, the sufficiency position (critical gap, partial, approaching, or surplus), the portfolio context statement, the grant contribution statement, and the revenue architecture declaration. Where the round configures the sufficiency architecture declaration at independent review evidence strength or above, the interface surfaces the corroborating evidence from a source outside the applicant's control and flags its absence.

**Public benefit mechanism and access condition declaration.** Where the public benefit mechanism dimension is active, the Dashboard surfaces the mechanism type statement and the access condition statement for assessment against the access condition required by the declared mechanism type. The interface flags a declared mechanism type that contradicts the applicant's own description of their work (for example, an output production claim under an all-rights-reserved copyright) as a material discrepancy requiring Block J investigation.

**Development stage declaration.** The Dashboard surfaces the declared stage number (1 through 5), the applicant's reasoning, and the evidence from a source outside the applicant's control, and flags inconsistencies between the declared stage and the rest of the entry submission for the reviewer to investigate.

**Obligation fulfillment record.** Where the applicant has prior grants from this funder, cites prior work as evidence of capability, or has prior round history with unresolved milestones or open conditions, the Dashboard surfaces the obligation fulfillment record for each prior grant: what was committed, what was produced, and whether the commitment was fulfilled, partially fulfilled, or unfulfilled. The interface places this alongside the Attestation Corpus query result.

**Prior work attribution statement.** Where the applicant cites prior work as evidence of capability, track record, or past contribution, the Dashboard surfaces the prior work attribution statement (entity of performance, the applicant's relationship at the time, and current ownership and access) for assessment as an adverse signal disclosure.

**Attestation Corpus query result.** For each application that provides an on-chain identity anchor, the Dashboard runs a funder-side Attestation Corpus query across the required public sources (on-chain attestation registries, the KarmaGAP grants and milestone interface, and any program-specific databases the round configuration names) and surfaces the result: total non-revoked attestations, attestations by known schema, and endorsement count and endorser identities where resolvable (spec Part IV). Where the query reveals prior grants, milestones, or obligations not disclosed in the obligation fulfillment record, the Dashboard records this as a material discrepancy. The Attestation Corpus query result also feeds the round-level Cohort Position assessment (Section 3) and the Layer 2 prior-grants investigation (Section 7).

These declaration fields are surfaced for assessment, not scored on the rubric's indicator scale; the entry specification gate finding (Section 6) records whether the entry submission, including its required declarations, satisfies the gate.

---

## Section 6: Rubric Loading and Scoring

When a reviewer opens an application, the Dashboard loads the confirmed rubric block from the published round specification. The rubric was generated, reviewed, and explicitly confirmed by the funder in Q12 of the Grant Configurator before the round opened. It is not re-derived at runtime from the CROSS assessment rubric companion document; the confirmed text in the round specification is the authoritative instrument. The Dashboard presents this confirmed rubric as the structured scoring interface. Any funder additions or round-specific guidance from Q12.2 appear alongside the standard CROSS criteria. Common indicator rubric criteria from Q12.3 appear as additional scored sections following the indicator specification rubric.

### Rubric structure in the Dashboard

The scoring interface presents the rubric in the sequence specified in the assessment rubric document. For each section, the Dashboard provides: the reviewer question from the rubric, the scoring criteria (the 1-4 table), a text field for the reviewer's finding, and the score selector.

For the entry specification gate (Section 2 of the rubric), the Dashboard requires the reviewer to record a gate finding before the scoring fields become active. A gate failure finding closes the scoring fields and routes the review directly to the recommendation section with a Do not fund pre-selection that the reviewer may not override.

For the conformance checks (Section 5 of the rubric), the Dashboard presents each check as a binary pass/fail with a required text field for findings. A conformance check failure produces a Do not fund pre-selection.

### Score entry and validation

The Dashboard validates that all required rubric fields are completed before the submission workflow begins. An incomplete rubric cannot be submitted. Required fields are: gate finding, all scored indicator fields for the primary indicator, all five data quality standard findings, and all three conformance check findings.

Recommendations are drawn only from the three CROSS recommendation categories: Fund, Fund with conditions, or Do not fund. The Dashboard does not permit any other recommendation vocabulary.

For Fund with conditions recommendations: the Dashboard requires at least one condition to be specified before submission is accepted. Each condition must have: a specific description of what must be resolved, a named verification method, and a stated deadline. The Dashboard validates that all three components are present for each condition.

### Assessment reconciliation

When guest reviewer assessments for the same application diverge substantially (defined as a difference of 2 or more points on any scored indicator field, or divergent gate findings, or divergent conformance check findings), the lead reviewer is notified. The lead reviewer may: add their own assessment to the record, initiate a discussion note visible to all reviewers who assessed the application, or escalate to the program administrator.

Reconciliation does not require reviewers to change their submitted assessments. The institutional record retains all submitted assessments. The lead reviewer's role is to document the divergence and ensure the final funding decision record acknowledges it, not to require consensus.

---

## Section 7: AI Assistance

The Reviewers Dashboard provides AI-assisted evaluation through three layers. The layers are cumulative: Layer 2 builds on Layer 1, and Layer 3 synthesizes both. Each layer produces a discrete output stored alongside the reviewer's assessment in the evaluation record. Layers are invoked sequentially; the reviewer may view each layer's output, supplement or override it, and invoke the next layer.

The AI assistance is a tool for the reviewer, not a substitute for the reviewer. The reviewer's final assessment is the obligation instrument. AI outputs inform it. The reviewer edits, overrides, and supplements AI-generated content before submission. A reviewer who accepts AI outputs without review has not fulfilled their review obligation.

All AI assistance is invoked using the CROSS skill (claude-skills/claude-skill-CROSS-0_2_0.md) as the machine-readable encoding of the standard, combined with the round specification for rubric calibration.

### Layer 1: Submitted evidence verification

Layer 1 checks whether the evidence the applicant submitted with their application matches the claims made in the entry specification. The check covers: does the named data source exist and is it publicly accessible? does the reported baseline value correspond to what the named source shows? for build-obligation applications, is the named deliverable location accessible? for retroactive obligation applications, does the evidence of use cited match independently verifiable records?

This layer is implemented via the evidence verification endpoint (currently at `/api/evidence/verify` in the Octant grant operations dashboard). It returns a structured verification report for each submitted evidence item: verified, verified in substance (with a note on what could not be confirmed), or cannot be verified from any public source (with the reason and what was tried).

The "cannot be verified" output from Layer 1 triggers the extended verification procedure from the document editing guidebook before the finding is recorded as unverifiable: Playwright rendering for JavaScript-dependent pages, direct API query of the data source, on-chain query via named public indexers, and aggregator checks via named third-party data providers.

### Layer 2: Independent investigation

Layer 2 conducts an independent investigation of the applicant's claims against third-party sources, without relying on the materials the applicant submitted. It is the equivalent of the manual evaluation sessions conducted for Epoch 12 evaluations, whose format and depth serve as the calibration baseline for this layer.

Layer 2 investigates the following categories for each applicant:

**Repository activity.** For applicants claiming software or protocol development: GitHub repository commit history, contributor count, open issues count and trend, recent pull request activity, code quality signals, and release history. The investigation notes the date of the last commit relative to the application submission date.

**Package and deployment records.** For applicants with published libraries or deployed contracts: npm download counts and trend (for JavaScript libraries), deployment verification on named chains via public block explorers, contract interaction counts, and unique address counts from named indexers.

**On-chain usage data.** For applicants making on-chain usage claims: independent query of the claimed contract addresses or protocol addresses from named public blockchain data sources. Comparison against the applicant's stated baseline and target.

**Prior grants and funding history.** Search across known grant history databases (Gitcoin grants data, KarmaGAP, on-chain treasury records where accessible) for prior grants to this applicant or this project. Cross-reference against the applicant's concurrent funding disclosure to identify any discrepancy. Prior Octant funding history is checked against the PoC vault records.

**Adverse signal investigation.** Independent search for adverse signals: prior rejections from comparable programs, published technical criticisms, community dispute records, documented coordinating conflicts, or negative due diligence findings that appear in public sources.

**Claim verification.** For specific quantitative claims made in the application that can be independently verified (user counts, transaction counts, download figures, protocol metrics), Layer 2 queries the named or inferable sources and reports whether the claim is confirmed, confirmed in substance, or cannot be verified from public sources.

The Layer 2 output is a structured investigation report organized by category, using the evaluation format from the Epoch 12 evaluation files as the structural template. Each finding uses the three-value taxonomy: Confirmed, Confirmed in substance (with an explicit statement of what could not be verified), or Cannot be verified from any public source (with reason and what was tried). The taxonomy "Plausible but unverified" is not used; it is a placeholder that must be resolved.

### Layer 3: Draft evaluation

Layer 3 applies the CROSS assessment rubric to the combined findings from Layers 1 and 2 and produces a draft evaluation: per-criterion scores with supporting notes, conformance check findings, and a preliminary recommendation. The draft is pre-populated in the scoring interface described in Section 6.

Layer 3 uses the round specification's obligation mode to select the correct rubric variant. For build-obligation rounds it applies the build-obligation gate and completion criteria assessment. For change-obligation rounds it applies the FROM state gate and the eleven-field indicator specification rubric. For retroactive obligation rounds it applies the program's published contribution assessment rubric.

The draft evaluation is clearly labeled as AI-generated in the scoring interface. The reviewer sees each draft score and note with an indication that it was generated by Layer 3. The reviewer edits, overrides, and supplements the draft before submitting. No draft score or note is submitted as the reviewer's assessment without the reviewer having actively confirmed or modified it.

Layer 3 pre-populates the conflict of interest conformance check as "pending" and requires the reviewer to complete it directly. The AI layer does not assess the reviewer's own conflict of interest status; that is the reviewer's declaration, not a matter for AI inference.

---

## Section 8: Reviewer Assessment Submission

When a reviewer has completed their scoring interface (with or without AI assistance) and is ready to submit, the Dashboard presents the submission workflow.

The submission workflow requires in sequence: confirmation that the conflict of interest declaration was submitted to the named receiving function before review began, scoring completion validation (all required rubric fields completed), post-participation certification (Template 8), and final submission.

Once submitted, the assessment is locked for that reviewer. The reviewer cannot edit a submitted assessment. If the program administrator flags an assessment for re-review, the assessment is unlocked for the reviewer who submitted it and they may revise it, with the revision recorded as an amendment to the assessment record.

The submitted assessment record contains: the reviewer's identity (role, not necessarily name, depending on the program's configured anonymization setting), the submission timestamp, the full scored rubric with all findings and notes, the recommendation (Fund, Fund with conditions, or Do not fund), the conditions list if applicable, the conformance check findings, the conflict of interest summary for this reviewer-application pair, the Layer 1, 2, and 3 AI outputs as they existed at submission time, and the post-participation certification.

---

## Section 9: Storage and Institutional Record

### Storage architecture

All evaluation records are stored in Supabase. The current architecture uses Supabase as the primary storage for evaluation data, AI assistance outputs, conflict of interest records, and assessment submissions. This architecture is noted as the current implementation; the data model in Section 10 documents the schema for future migration to alternative storage if the program requirements change.

The following data is stored per evaluation session:

- The complete evaluation record for each reviewer-application pair (rubric scores, findings, recommendation, conditions)
- The Layer 1 evidence verification output for each application
- The Layer 2 independent investigation report for each application
- The Layer 3 draft evaluation as it existed when the reviewer submitted their final assessment
- The reviewer's edits to the Layer 3 draft (stored as a diff between the draft and the submitted assessment)
- The conflict of interest declaration and post-participation certification for each reviewer-application pair
- The evaluation stage open and close timestamps for the round

### Sync to PoC vault

Completed evaluation records are synced to the Proof of Coordination vault as part of the institutional record. The sync occurs when the evaluation stage closes and the program administrator marks the round's evaluation records as ready for archival.

The sync writes each evaluation record to the vault in the format of the existing Epoch 12 evaluation files: markdown documents with frontmatter, organized by epoch or round, containing the investigation summary, rubric assessment, and recommendation. The vault record does not include raw AI outputs; it contains the reviewer's final assessment as submitted, with a metadata note indicating whether AI assistance was used and at which layers.

The sync record includes the Layer 2 investigation as a separate linked document in the vault, preserving the research depth for institutional memory purposes. Future reviewers evaluating the same project in a subsequent round can retrieve the prior investigation record from the vault as context, rather than re-investigating sources that have already been checked.

---

## Section 10: Data Model

```
Evaluation_Record {
  evaluation_id:          string (unique identifier)
  round_id:               string (foreign key to Round in Grantee Dashboard data model)
  application_id:         string (identifier of the application being evaluated)
  reviewer_id:            string
  reviewer_role:          enum (guest_reviewer | lead_reviewer | funder_administrator)
  evaluation_stage_id:    string (foreign key to the evaluation stage session)
  status:                 enum (in_progress | submitted | flagged_for_review)
  submission_timestamp:   timestamp or null

  // Conflict of interest record (all three tiers, spec Part VII)
  coi_declaration: {
    submitted_at:         timestamp
    submitted_to:         string (named receiving function, separate from funding decision-maker)
    tier_1_blocks:        array of {relationship_type: string, application_id: string,
                          discovered_post_hoc: boolean}
    tier_2_disclosures:   array of {relationship_type: string, is_org_role_conflict: boolean,
                          waiver_justification: text or null, waiver_granted: boolean,
                          waiver_approver: string or null, waiver_timestamp: timestamp or null,
                          recused: boolean}
    tier_3_disclosures:   array of {relationship_type: string, notes: text}
    funder_side_consulting: {
      declared:           boolean
      scope:              enum (none | same_program_area | primary_income_source) or null
      routing:            enum (tier_2_waiver | categorical_bar) or null
      waiver_approver:    string or null
      waiver_timestamp:   timestamp or null
    } or null
    novel_relationship:   text or null
  }
  post_participation_certification: {
    completed_at:         timestamp or null
    no_new_conflicts:     boolean or null
  }

  // AI assistance outputs (stored at submission time)
  layer_1_output: {
    generated_at:         timestamp
    evidence_items:       array of {claim: string, status: enum (confirmed | confirmed_in_substance |
                          cannot_verify), notes: text}
  } or null

  layer_2_output: {
    generated_at:         timestamp
    repository_activity:  text
    package_deployment:   text
    on_chain_usage:       text
    prior_grants:         text
    adverse_signals:      text
    claim_verification:   array of {claim: string, status: enum (confirmed | confirmed_in_substance |
                          cannot_verify), notes: text}
    full_report:          text (structured markdown in Epoch 12 evaluation format)
  } or null

  layer_3_draft: {
    generated_at:         timestamp
    draft_scores:         object (keyed by rubric field, values: {score: integer, note: text})
    draft_recommendation: enum (fund | fund_with_conditions | do_not_fund)
    draft_conditions:     array of {description: text, verification_method: text, deadline: date}
  } or null

  // Entry-gate declaration access (surfaced for assessment, not indicator-scored; spec Part IV)
  entry_gate_declarations: {
    organizational_identity: {
      legal_entity:       text
      parent_org:         text
      affiliated_entities: text
      prior_round_history: text
      disbursement_authority: text
      on_chain_anchor:    text
      undisclosed_affiliation_flag: boolean
    } or null
    sufficiency_architecture: {
      scope:              text
      sufficiency_position: enum (critical_gap | partial | approaching | surplus)
      portfolio_context:  text
      grant_contribution: text
      revenue_architecture: text
      corroborating_evidence: text or null
    } or null
    public_benefit_mechanism: {
      mechanism_type:     string
      access_condition:   text
      contradiction_flag: boolean
    } or null
    development_stage: {
      declared_stage:     integer (1 through 5)
      reasoning:          text
      external_evidence:  text
      consistency_flag:   boolean
    } or null
    obligation_fulfillment_record: array of {prior_round: string, committed: text,
                          produced: text, status: enum (fulfilled | partial | unfulfilled)} or null
    prior_work_attribution: array of {work: string, entity_of_performance: text,
                          relationship_at_time: text, current_ownership: text} or null
    attestation_corpus_query: {
      queried_at:         timestamp
      total_non_revoked:  integer
      by_schema:          object (schema name -> count)
      endorsers:          array of string
      undisclosed_obligation_flag: boolean
    } or null
  } or null

  // Reviewer's final assessment
  rubric_assessment: {
    obligation_mode:      enum (build | change | retroactive)
    gate_finding: {
      passed:             boolean
      finding_text:       text
    }
    indicator_scores:     array of {field: string, score: integer, finding: text}
    data_quality_standards: array of {standard: string,
                          status: enum (pass | conditional | fail), finding: text}
    conformance_checks:   array of {check: string, status: enum (pass | fail | signal_documented),
                          finding: text}
    recommendation:       enum (fund | fund_with_conditions | do_not_fund)
    conditions:           array of {description: text, verification_method: text,
                          deadline: date} or null
    primary_reason:       text (single most important reason for the recommendation)
  } or null

  // Diff between Layer 3 draft and submitted assessment (null if no AI assistance used)
  layer_3_edits: {
    score_overrides:      array of {field: string, draft_score: integer, submitted_score: integer}
    note_edits:           array of {field: string, had_edit: boolean}
    recommendation_change: boolean
  } or null
}

Evaluation_Stage {
  stage_id:               string (unique identifier)
  round_id:               string
  opened_at:              timestamp
  closed_at:              timestamp or null
  opened_by:              string (administrator identity)
  closed_by:              string or null
  reviewer_assignments:   array of {reviewer_id: string, role: enum, application_ids: array of string}

  // Reviewer calibration gate (required where any gate is at independent review level or above)
  calibration_record: {
    required:             boolean
    completed_at:         timestamp or null
    gate_criteria_reviewed: text
    worked_examples:      array of {example_id: string, expected: enum (satisfies | fails)}
    reviewers_calibrated: array of {reviewer_id: string, calibrated_at: timestamp,
                          worked_example_assessments: object}
    inter_rater_check:    text or null
  } or null
}

// Round-level Cohort Position assessment (spec Part VII; run before final gate determinations)
Cohort_Position_Assessment {
  round_id:               string
  assessed_at:            timestamp
  assessed_by:            string (administrator identity)
  personnel_overlap:      array of {individual: string, application_ids: array of string,
                          coi_disclosure_triggered: boolean}
  wallet_overlap:         array of {address: string, application_ids: array of string,
                          reconciled: boolean}
  endorser_concentration: array of {endorser: string, application_ids: array of string,
                          schema: string}
}

// Attestor conflict status check (attestation-independence provision, spec Part VII)
Attestor_Conflict_Check {
  round_id:               string
  application_id:         string
  attestor_id:            string
  tier:                   enum (none | tier_1 | tier_2)
  waiver_granted:         boolean or null
  waiver_approver:        string or null
  accepted:               boolean (false where tier_1, or tier_2 without waiver)
}

Vault_Sync_Record {
  sync_id:                string (unique identifier)
  round_id:               string
  synced_at:              timestamp
  synced_by:              string (administrator identity)
  evaluation_ids:         array of string (evaluation records included in this sync)
  vault_paths:            array of {evaluation_id: string, vault_path: string}
  investigation_paths:    array of {application_id: string, vault_path: string}
}
```

---

## Section 11: Forward-Looking Considerations

**Integration with the Grantee Dashboard.** The evaluation record produced by the Reviewers Dashboard is the source of the obligation registry contents in the Grantee Dashboard: conditions recorded in a "Fund with conditions" recommendation become the conditions tracked in the Grantee Dashboard's disbursement condition tracking. The connection between the two dashboards is the obligation registry creation step. Conditions must be exported from the Reviewers Dashboard in the format expected by the Grantee Dashboard's obligation registry schema.

**PoC vault as the longitudinal institutional record.** The Proof of Coordination vault accumulates the investigation records from Layer 2 across rounds. A project that has been evaluated in multiple epochs has a growing investigation history in the vault: prior grant usage, prior repository activity snapshots, prior adverse signal checks. Future Layer 2 investigations for the same project can retrieve this history as context, making each successive evaluation more efficient and the investigation more longitudinally coherent. This is one of the concrete expressions of the funder maturation tracking capability noted in the CROSS standard's purpose section.

**Supabase migration path.** The current Supabase storage architecture is documented as the present implementation, not the permanent one. The data model in Section 10 is designed to be portable: field names and types are specified independently of Supabase's internal representation, and the vault sync mechanism provides a durable copy in the PoC vault. A migration to alternative storage requires only implementing the same data model in the target store and updating the sync logic; no structural changes to the evaluation workflow are required.

**AI assistance maturation.** The three-layer AI assistance model is specified at a level of capability available at the time of this document. Layer 2 in particular is calibrated to the current manual investigation practice for Epoch 12 evaluations. As investigation tooling improves (deeper on-chain data access, improved cross-program grant history databases, better adverse signal corpora), the Layer 2 specification should be updated to reflect the expanded investigation capability. The calibration baseline is always the most recent cycle of completed manual evaluations in the PoC vault.
