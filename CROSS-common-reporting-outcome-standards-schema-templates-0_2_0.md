---
title: CROSS - Common Reporting Outcome Standards Schema - Templates
version: 0.3.1
date: 2026-06-05
license: CC0
status: Working draft. Companion templates document synced to the CROSS specification at CROSS-common-reporting-outcome-standards-schema-0_5_0.md. Supersedes version 0.2.0.
---

# CROSS: Common Reporting Outcome Standards Schema - Templates

Version 0.3.1 | 2026-06-08 | CC0

---

## Changelog

**0.3.1 (2026-06-08).** Frame Language own-voice pass. Own-voice watchlist terms were replaced with the structural act each names (accountability became obligation; the integrity standard became the data quality standard; mandatory became required; "name the individual who assumes personal accountability" became "who is personally answerable"; own-voice beneficiary safety became affected-population safety). Two naming updates aligned the templates with the spec: the Template 1A/1B/1C/2 titles "Build/Retroactive/Change Accountability" became "Build/Retroactive/Change Obligation", and Template 15 "Governance and Continuity Resilience Declaration" became "Continuity Capacity Declaration". Form-field labels, framework names, governance tokens, and the changelog rows were preserved as citation. Em-dash sweep clean. No template was restructured; vocabulary and naming only.

**0.3.0 (2026-06-05).** Synced to the CROSS specification version 0.5.0. Added seven entry-gate declaration templates: Organizational Identity (Template 11), Sufficiency Architecture (Template 12), Public Benefit Mechanism and Access Condition (Template 13), Development Stage (Template 14), Governance and Continuity Resilience (Template 15), Obligation Fulfillment Record for returning applicants (Template 16), and Prior Work Attribution Statement (Template 17). Added a token generation event disclosure section to the Concurrent Funding Disclosure Form (Template 4). Added the served-population risk-bearer floor as a noted consideration in the beneficiary and population sections of the build and change entry templates (Templates 1A, 1C, and 2). Added a CRAFT-inheritance note to the How-to-Use section. No existing template was restructured or rewritten.

**0.2.0 (2026-05-14).** Prior version. Templates 1A through 10.

---

## How to Use This Document

This document contains the fillable forms that applicants, reviewers, and grantees use to implement CROSS. Each template is self-contained. Brief inline instructions explain what each field requires. Completion checklists appear at the end of each template.

**CRAFT inheritance.** CROSS is a domain application of CRAFT (Chains Reveal Attested Falsifiable Truth) for the grants domain. The forms in this document are the applicant-facing surface of that application; the full inheritance, including which of CRAFT's six conditions CROSS realizes and how, is declared in the spec (Part XIII, CRAFT Inheritance Receipt). Applicants do not need to read the receipt to complete these forms, but the fields below are shaped by it: the entry declarations, the disclosure forms, and the gate evidence requirements all exist because CROSS commits to producing an attested, falsifiable record that an independent party can check.

**Which entry specification template to use.** The obligation mode for a round is declared by the funder in the published round specification before the round opens. Applicants do not choose the mode.

- Build obligation round: use Template 1A (Deliverable Specification Form)
- Change obligation round, Small Team scale: use Template 1C (FROM/TO Specification, Small Team)
- Change obligation round, Standard scale: use Template 2 (FROM/TO Specification with Theory of Change)
- Retroactive obligation round: use Template 1B (Retroactive Contribution Form)

All applications also require, at the entry specification gate, a set of declarations that are pre-conditions for gate assessment: Template 11 (Organizational Identity Declaration), Template 12 (Sufficiency Architecture Declaration), Template 14 (Development Stage Declaration), and, where the application rests on a public goods claim, Template 13 (Public Benefit Mechanism and Access Condition Declaration). Where the application produces ongoing infrastructure or names a single primary contributor, Template 15 (Continuity Capacity Declaration) also applies. Returning applicants who have received prior grants from this funder, or who cite prior work as evidence of capability, complete Template 16 (Obligation Fulfillment Record). Any applicant who cites prior work as evidence of capability, track record, or past contribution completes Template 17 (Prior Work Attribution Statement).

All applications also require: Template 3 (Indicator Registration Form, one per indicator), Template 4 (Concurrent Funding Disclosure), and Template 5 (Adverse Signal Disclosure). Reviewers complete Templates 6, 7, and 8 (conflict of interest forms). Template 9 is for privacy-sensitive accommodation requests. Template 10 (Gate Evidence Submission) is used at progress verification and completion verification gates, not at application.

The distinction between Standard and Small Team scale in change-obligation rounds is determined by the granting committee's configuration based on funding amount and the scope of the public impact claim. When in doubt, use the Standard version.

---

## Template 1A: Build Obligation - Deliverable Specification Form

*Use this form when the round operates in build obligation mode. The entry specification asks what the applicant will produce and how a reviewer could verify it is complete. Attach this form to the main application.*

---

### Project Name

> [Enter project name]

---

### Deliverable Name

*A short label for what will be produced. This is not the completion criteria; it is a recognizable name.*

> [Enter deliverable name]

---

### Deliverable Type

*What form will the deliverable take? Select the closest category or name another if none fit.*

- [ ] Working software (library, protocol, tool, module)
- [ ] Deployed smart contract or on-chain protocol
- [ ] Research or design document
- [ ] Dataset or data infrastructure
- [ ] Specification or standard
- [ ] Other: [specify]

**Format for delivery**

*How will the deliverable be made publicly available? Name the repository, registry, publication venue, or other delivery mechanism.*

> [Enter format and delivery location]

---

### Completion Criteria

*What must be true for this deliverable to be considered complete? State the criteria with enough specificity that a reviewer who did not commission the work could verify each one independently. Criteria that a reviewer cannot verify without contacting you do not satisfy this field.*

**Criterion 1**

> [Enter criterion]

**Criterion 2**

> [Enter criterion, add as many criteria as needed]

**Criterion 3**

> [Enter criterion or write "not applicable"]

**Independent verifiability statement**

*In one or two sentences: how would an independent reviewer confirm that each criterion above was met? Name any external source, registry, repository, or named party they would consult.*

> [Enter independent verifiability statement]

---

### Named Beneficiary or User

*Who will use this deliverable? Name at least one specific party (a named organization, developer community, protocol, or user type) outside your own team who has expressed a need for it. This field satisfies the beneficiary validation requirement where the coordinating party engagement dimension is activated.*

> [Enter named beneficiary or user, and briefly describe how the need was expressed]

*Served-population risk-bearer floor (noted consideration).* The served population (the people this deliverable is meant to serve) bears loss when funded work does not reach them. The spec names the served population as a risk-bearer carried through every gate, not validated only at entry. You name them here at entry; at the completion verification gate the funder additionally considers whether work recorded as delivered actually reached them. Naming the served population precisely now (not only an immediate user) makes that later consideration possible.

---

### Coordinating Party Engagement Dimension (if activated by the funder)

*Complete this section only if the funder has activated the coordinating party engagement dimension for this round. Describe the current absence or inadequacy of the deliverable, with named evidence of the gap it addresses.*

**Evidence of the gap the deliverable addresses**

*Name an independent source (a named party who has confirmed the need, an existing tool's documented limitation, or a named data source confirming the gap). Your own assessment of the gap does not satisfy this field.*

> [Enter evidence of the gap, or write "Not activated" if this dimension is not enabled for this round]

---

### Completion Checklist - Template 1A

- [ ] Deliverable name is present and descriptive
- [ ] Deliverable type is selected or named
- [ ] Format and delivery location are specified
- [ ] Completion criteria are stated with enough specificity for independent verification
- [ ] Independent verifiability statement names the source or party a reviewer would consult
- [ ] Named beneficiary or user is provided with a brief description of the expressed need
- [ ] Coordinating party engagement section is completed or marked "Not activated"
- [ ] No fields left blank

---

## Template 1B: Retroactive Obligation - Prior Contribution Form

*Use this form when the round operates in retroactive obligation mode. The entry specification asks what prior contribution was produced, when, and with what evidence of use. Attach this form to the main application.*

---

### Project Name

> [Enter project name]

---

### Contribution Summary

*In two to four sentences: what was produced, when, and what public good does it serve? This is the plain-language description of the prior contribution.*

> [Enter contribution summary]

---

### Contribution Period

*The dates during which the contribution was produced or sustained.*

**Start Date:** ___________________________

**End Date (or "ongoing"):** ___________________________

---

### Evidence of Contribution

*Name the publicly accessible sources that confirm the contribution exists. Each source must be accessible to an independent reviewer without contacting you. Provide at least two sources.*

| Source | What it confirms | URL or access method |
|---|---|---|
| [Source name] | [What this source confirms about the contribution] | [URL or how to access] |
| [Source name] | [What this source confirms] | [URL or how to access] |
| [Add rows as needed] | | |

---

### Evidence of Use

*Name the publicly accessible evidence that the contribution is being used by parties outside your team. Adoption metrics, named organizations using the contribution, public citations, download counts, or on-chain usage data from named sources all qualify. Self-reported usage without independent corroboration does not satisfy this field on its own.*

| Evidence of use | Source | Scale or scope |
|---|---|---|
| [Describe the usage evidence] | [Named independent source] | [Brief note on scale: e.g., number of users, organizations, or transactions] |
| [Add rows as needed] | | |

---

### Prior Award Disclosure

*List any prior awards received for the same or substantially overlapping contribution, from this or any other program. Non-disclosure is a disqualifier. Disclosure is not.*

- [ ] No prior awards exist for this contribution or substantially overlapping work.

- [ ] Prior awards exist. Complete the table below.

| Program or funder | Award period | Overlap with this contribution |
|---|---|---|
| [Funder name] | [Period] | [Describe the overlap] |
| [Add rows as needed] | | |

---

### Forward Commitment (if configured by the funder)

*Complete this section only if the funder has activated a forward commitment requirement for this round. State the specific action you commit to completing as a condition of receiving the award.*

**Commitment description**

*Name the deliverable or action you commit to.*

> [Enter commitment description, or write "Not configured" if this section does not apply]

**Completion criteria**

*How will a reviewer confirm the commitment was fulfilled? State verifiable criteria.*

> [Enter completion criteria]

**Timeline**

*By when do you commit to completing this?*

> [Enter timeline]

---

### Completion Checklist - Template 1B

- [ ] Contribution summary is present and specific
- [ ] Contribution period is stated
- [ ] At least two sources of independently accessible contribution evidence are named
- [ ] Evidence of use from independent sources is provided
- [ ] Prior award disclosure is complete (either "none" attestation or table)
- [ ] Forward commitment section is completed or marked "Not configured"
- [ ] No fields left blank

---

## Template 1C: Change Obligation - FROM/TO Specification (Small Team Version)

*Use this form when the round operates in change obligation mode and the committee has determined that Small Team scale applies. It captures the essential FROM state and TO state. Attach this form to the main application.*

**Fields Omitted From The Standard Version And Why:** Theory of change formalization (activities, outputs, outcomes, named assumptions), adaptive management mechanism. The Coordination Scaling Standard makes these optional for small-team applications with specific diagnoses and modest claims. All other FROM/TO fields remain required.

---

### Project Name

> [Enter project name]

---

### FROM State: The Condition Before the Intervention

*Describe the specific, measurable problem your project addresses. The FROM state is not a category of concern; it is a documented condition in a defined population. A qualifying FROM state names a condition, a population, a source of evidence, and when that evidence was collected.*

**Condition**

*In one or two sentences: what is the specific problem, expressed as a measurable state? Use numbers, rates, or observable binary conditions where possible.*

> [Enter the specific condition]

**Population**

*Who or what is affected? Name the population precisely: geography, user type, protocol, sector, or other defining characteristic.*

> [Enter the defined population]

*Served-population risk-bearer floor (noted consideration).* The population named here is a risk-bearer of the round's evaluation, not only the subject of a baseline measurement. The spec carries the served population through every gate: it bears loss when the round funds work that does not serve it. Name it precisely enough that, at the completion verification gate, the funder can consider whether the change you report actually reached this population or whether effects on it fall outside your declared indicators.*

**Source of evidence for the FROM state**

*Name the source. It must be accessible to an independent reviewer. Applicant-controlled sources without independent corroboration do not satisfy the data quality standard.*

> [Enter the named source]

**Date or period of measurement**

> [Enter date or period]

---

### TO State: The Expected Condition After the Intervention

**Target condition**

*What specific, measurable state will the indicator be in at grant end? Use the same units as the FROM state.*

> [Enter the target condition]

**Unit of measurement**

*Confirm that this is the same unit used in the FROM state above.*

> [Enter unit of measurement]

**Measurement method at grant end**

*How will you measure the TO state? Name the source and collection approach.*

> [Enter measurement method]

**Timeline**

> [Enter timeline]

---

### Connecting FROM to TO

*One paragraph explaining how your project's activities connect the FROM state to the TO state. Identify one key assumption your explanation rests on.*

> [Enter connecting paragraph]

---

### Completion Checklist - Template 1C

- [ ] FROM state names a specific condition (not a category of concern)
- [ ] FROM state identifies a defined population with sufficient precision
- [ ] FROM state includes a named, independently accessible source
- [ ] FROM state includes a date or measurement period
- [ ] TO state uses the same units as the FROM state
- [ ] TO state is expressed as a target status (non-cumulative) or cumulative total (cumulative)
- [ ] TO state names the measurement method to be used at grant end
- [ ] TO state includes a timeline
- [ ] Connecting paragraph identifies at least one key assumption
- [ ] No fields left blank

---

## Template 2: Change Obligation - FROM/TO Specification with Theory of Change (Standard Version)

*Use this form for Standard scale change-obligation applications. It captures the full FROM state, a formalized theory of change with named assumptions at each step, the TO state, and an adaptive management mechanism. Attach this form to the main application.*

---

### Project Name

> [Enter project name]

---

### FROM State: The Condition Before the Intervention

**Condition**

> [Enter the specific condition]

**Population**

> [Enter the defined population]

*Served-population risk-bearer floor (noted consideration).* The population named here is a risk-bearer of the round's evaluation, carried through every gate, not validated only at entry. The spec records that it bears loss when the round funds work that does not serve it. Name it precisely enough that, at the completion verification gate, the funder can consider whether the change you report actually reached this population, and whether effects on it fall outside your declared indicators.*

**Source of evidence for the FROM state**

> [Enter the named source]

**Date or period of measurement**

> [Enter date or period]

---

### Theory of Change

*A theory of change documents the logical pathway from your project's activities to the outcome you are claiming. Each step requires named assumptions: the conditions that must hold for that step to produce the next.*

**Activities**

| Activity | Description |
|---|---|
| Activity 1 | [Enter activity description] |
| Activity 2 | [Enter activity description] |
| Activity 3 | [Enter activity description, add rows as needed] |

**Assumptions at the activity level**

*What must be true for these activities to be executable as planned?*

> [Enter activity-level assumptions]

**Outputs**

| Output | How you will verify it was produced |
|---|---|
| Output 1 | [Enter verification method] |
| Output 2 | [Enter verification method] |
| Output 3 | [Enter verification method, add rows as needed] |

**Assumptions at the output level**

> [Enter output-level assumptions]

**Outcomes**

| Outcome | Relationship to your primary indicator |
|---|---|
| Outcome 1 | [Enter relationship to indicator] |
| Outcome 2 | [Enter relationship to indicator] |
| Outcome 3 | [Enter relationship to indicator, add rows as needed] |

**Assumptions at the outcome level**

*What must be true for your outputs to produce these outcomes?*

> [Enter outcome-level assumptions]

---

### TO State: The Expected Condition After the Intervention

**Target condition**

*Must use the same units as the FROM state.*

> [Enter the target condition]

**Unit of measurement**

> [Enter unit of measurement]

**Measurement method at grant end**

> [Enter measurement method]

**Timeline**

> [Enter timeline]

---

### Adaptive Management Mechanism

**Monitoring approach**

*How and how often will you check whether your key assumptions are holding?*

> [Enter monitoring approach]

**Decision triggers**

*What evidence of assumption failure or unexpected conditions will prompt a change in activities or outputs?*

> [Enter decision triggers]

**Adjustment authority**

*Who has authority to make significant changes to approach, and how will those changes be reported to the funder?*

> [Enter adjustment authority]

---

### Completion Checklist - Template 2

- [ ] FROM state names a specific condition (not a category of concern)
- [ ] FROM state identifies a defined population
- [ ] FROM state includes a named, independently accessible source
- [ ] FROM state includes a date or measurement period
- [ ] Theory of change lists specific activities, outputs, and outcomes (not categories)
- [ ] Named assumptions appear at each step: activity level, output level, outcome level
- [ ] TO state uses the same units as the FROM state
- [ ] TO state is expressed as a target status (non-cumulative) or cumulative total (cumulative)
- [ ] TO state names the measurement method
- [ ] TO state includes a timeline
- [ ] Adaptive management mechanism names a monitoring approach, decision triggers, and adjustment authority
- [ ] No fields left blank

---

## Template 3: Indicator Registration Form

*Complete one form for each claimed outcome indicator. Submit one form per indicator. Attach all indicator registration forms to the main application.*

*Note: this form applies in build-obligation and change-obligation rounds. In retroactive obligation rounds, complete this form only if the program has configured indicator-based forward reporting.*

*Small Team version note: the Data Cost Estimation field has a simplified version for Small Team applications, noted within that field below. All other fields are identical across both scales.*

---

### Project Name

> [Enter project name]

### Indicator Number

> Indicator number: [e.g., 1 of 3] | [ ] Primary indicator

---

### Field 1: Indicator Name

*A short descriptive label. This is not the operational definition.*

> [Enter indicator name]

---

### Field 2: Rationale for Indicator

*Explain why you selected this indicator over available alternatives. What other indicators did you consider? Why does this one best capture the outcome or deliverable you are claiming? Name at least one alternative considered. This field is required, not optional.*

> [Enter rationale, including alternatives considered and why this indicator was chosen]

---

### Field 3: Measurement Form and Evidence Classification

*Describe what a result looks like and in what form it will be reported. Be specific: name where the evidence comes from, how the result is expressed, and whether values sum across periods or describe a status at a point in time.*

*Useful description (build obligation example): "A binary indicator: either the library is published to the named package registry at the specified version, confirmed by a public repository check, or it is not. Non-cumulative."*

*Useful description (change obligation example): "A count of unique wallet addresses per 30-day window that completed at least one qualifying transaction on the named contract, sourced from on-chain public data via the named block explorer application programming interface. Non-cumulative: each month's count describes the status for that month."*

**Measurement form description**

> [Enter plain-language description of measurement form and evidence]

**Classification (complete or leave for reviewer classification)**

| Axis | Options | Your classification |
|---|---|---|
| Source type | On-chain verifiable / Off-chain verifiable / Qualitative or narrative | [Enter or leave blank] |
| Measurement form | Quantitative / Ordinal / Binary / Qualitative | [Enter or leave blank] |
| Aggregation type | Cumulative (values sum across periods) / Non-cumulative (describes a status at a point in time) | [Enter or leave blank] |

---

### Field 4: Operational Definition

*Specifies what counts and what does not count as one unit of the claimed result. Complete all four sub-fields.*

**4a. Inclusion criteria**

*What qualifies as one instance of this indicator?*

> [Enter inclusion criteria]

**4b. Exclusion criteria**

*What does this indicator explicitly not count?*

> [Enter exclusion criteria]

**4c. Unit of analysis**

*What is the entity being counted or measured? (person, wallet address, transaction, site, organization, other named unit)*

> [Enter unit of analysis]

**4d. Edge case determination**

*At least one example of an ambiguous case and how your operational definition handles it.*

> [Enter at least one edge case example and resolution]

---

### Field 5: Construction and Aggregation Methodology

*The calculation rule in sufficient detail that an independent reviewer with access to your stated data source could replicate your result.*

**Formula or counting rule** *(for build-obligation indicators: the completion determination process)*

> [Enter formula, counting rule, or completion determination process]

**Partial or missing data handling**

> [Enter partial data handling approach]

**Aggregation from sub-units**

> [Enter aggregation approach, or write "Not applicable"]

---

### Field 6: Cumulative or Non-Cumulative

- [ ] **Cumulative.** This indicator sums across reporting periods. The life-of-grant target is a total reached by addition across all periods.

- [ ] **Non-cumulative.** This indicator measures a status at a point in time. The life-of-grant target is the target status at grant end. Summing a non-cumulative indicator across periods is a data construction error.

- [ ] **Not applicable.** Binary completion criteria for a build-obligation deliverable; not subject to period-by-period accumulation.

**Implication for your target**

*In one sentence, confirm what this designation means for how your life-of-grant target is expressed.*

> [Enter confirmation]

---

### Field 7: Disaggregation Categories

**Ratchet Notice:** Disaggregation categories committed to in this form may be supplemented in subsequent reporting periods (you may add categories), but may not be removed without committee approval and documented rationale.

| Disaggregation category | How values will be reported separately |
|---|---|
| [Category 1] | [Description] |
| [Category 2] | [Description] |
| [Add rows as needed] | |

*If you do not plan to disaggregate this indicator, write "None committed" and explain why disaggregation is not applicable.*

> [Enter "None committed" with explanation, or leave the table above completed]

---

### Field 8: Data Source and Collection Method

**Named data source**

*For change-obligation indicators: the specific source (contract address, named public application programming interface endpoint, named third-party platform, institutional partner, or named survey instrument). For build-obligation indicators: the named artifact location and the named party who will confirm it meets the completion criteria.*

> [Enter named data source]

**Collection method**

> [Enter collection method]

**Independent corroboration**

*How can an independent reviewer access or verify this data without relying solely on your reporting?*

> [Enter independent corroboration mechanism]

---

### Field 9: Data Cost Estimation

**Standard Version:** Provide an estimate of the cost of data collection for this indicator across the full grant period.

**Small Team Version (simplified):** Attest that data collection for this indicator is feasible within your project budget using free or low-cost methods.

Select the version that applies:

- [ ] Standard version

> **Approximate Cost:** \$[amount]
>
> **Funding Source For Data Collection:** [Grant budget / other named source]
>
> **Budget Line Item Or Category:** [Enter line item]

- [ ] Small Team version (simplified)

> **Attestation:** Data collection for this indicator is feasible within our project budget. The data source ([enter source name]) is available at no cost or negligible cost. We have confirmed access to this source.

---

### Field 10: Baseline (FROM State)

*Complete the section that matches the obligation mode.*

**Change-obligation:** The documented state of the condition before the intervention begins.

**Baseline value**

> [Enter baseline value]

**Date or period of baseline measurement**

> [Enter date or period]

**Source of baseline data**

> [Enter baseline source]

**Pre-intervention confirmation**

*Confirm that this baseline was established before your intervention began, or explain why a pre-intervention baseline is not available and what you are using instead.*

> [Enter pre-intervention confirmation or explanation of alternative]

---

**Build-obligation (coordinating Party Engagement Dimension Activated):** The documented current absence or inadequacy of the deliverable, with named evidence of the gap.

**Evidence of the gap**

> [Enter named independent evidence of the gap this deliverable addresses, or write "Not applicable" if the coordinating party engagement dimension is not activated for this round]

---

**Retroactive Obligation:** The documented state of the prior contribution at the time the award period begins.

**Description of prior contribution state**

> [Enter description of what existed and in what condition at the start of the award period, or write "Not applicable"]

---

### Field 11: Target (TO State)

*Complete the section that matches the obligation mode.*

**Change-obligation:** The expected state of the indicator at grant end.

**Target value**

> [Enter target value]

**Target type (confirm)**

- [ ] Target status (for non-cumulative indicators): the expected state at grant end
- [ ] Cumulative total (for cumulative indicators): the total to be reached by summing across all reporting periods

**Timeline for reaching target**

> [Enter timeline]

---

**Build-obligation:** The completion criteria the deliverable must meet.

**Completion criteria**

*State the criteria with enough specificity that an independent reviewer could determine whether they are met.*

> [Enter completion criteria, or write "Covered in Template 1A" if already specified there]

**How a reviewer would verify completion**

> [Enter verification approach]

---

**Retroactive With Forward Commitment:** The named action the awardee commits to completing.

**Forward commitment target**

> [Enter forward commitment target with completion criteria, or write "Not configured"]

---

### Completion Checklist - Template 3

- [ ] Indicator name is filled in
- [ ] Rationale explains why this indicator was chosen over alternatives
- [ ] Measurement form is described in plain language with enough specificity to classify
- [ ] Classification table is completed or acknowledged as left for reviewer classification
- [ ] Operational definition includes all four sub-fields
- [ ] Construction methodology is specific enough for an independent reviewer to replicate
- [ ] Partial data handling is addressed
- [ ] Cumulative, non-cumulative, or not applicable is designated with implication confirmed
- [ ] Disaggregation categories are listed or "None committed" is stated with explanation
- [ ] Disaggregation ratchet notice has been read and acknowledged
- [ ] Named data source is specific (not a category)
- [ ] Independent corroboration mechanism is named
- [ ] Data cost estimation is complete (Standard or Small Team version)
- [ ] Baseline section appropriate to the mode is complete
- [ ] Target section appropriate to the mode is complete
- [ ] No fields left blank

---

## Template 4: Concurrent Funding Disclosure Form

*All active grants, investments, or revenue sources from the prior 24 months that are related to the scope of this application must be disclosed. Non-disclosure of concurrent funding is a disqualifier. Disclosure is not.*

*For retroactive obligation applications: also disclose any prior awards received for the same or substantially overlapping contribution from this or any other program.*

*Submit one row per disclosed source. If you have no sources to disclose, complete the attestation at the bottom and state "None."*

---

### Project Name

> [Enter project name]

### Applicant Name or Organization

> [Enter applicant name or organization]

---

### Disclosed Funding Sources

| Field | Entry |
|---|---|
| **Source name** | [Name of investor, foundation, decentralized autonomous organization, protocol, or other funder] |
| **Source type** | [ ] Grant / [ ] Investment / [ ] Revenue / [ ] Prior retroactive award / [ ] Token generation event / [ ] Other: [specify] |
| **Approximate amount** | \$[amount] or [describe if non-monetary] |
| **Grant period or investment date** | [Start date to end date, or date] |
| **Relationship to this application's scope** | [Describe how this funding source relates to the work described in this application. If the scopes are non-overlapping, explain why. If they overlap, describe the boundary.] |
| **Ongoing milestone or reporting obligations to this source** | [ ] Yes / [ ] No. If yes: [describe obligations] |
| **Decision-making rights held by this source over the funded work** | [ ] Yes / [ ] No. If yes: [describe rights held] |

*Copy this table for each additional source.*

---

### Token Generation Event Disclosure

*Token generation events, planned or executed within the prior 24 months, are required disclosure items alongside grants and investments. A token generation event is any mechanism by which the applying entity or its principals generate, allocate, or vest tokens to themselves, investors, or the public in a manner that represents or may represent economic value. This includes initial decentralized exchange offerings (IDOs), token generation events (TGEs), initial coin offerings (ICOs), liquidity bootstrapping pool launches, and continuous founder or contributor vesting schedules releasing tokens during the disclosure window. A token that has not yet launched but for which a whitepaper, tokenomics document, or allocation schedule exists is a pending token generation event and must be disclosed. The existence of a token or planned token is not a disqualifier; non-disclosure of a material token event is treated as a concurrent funding omission under the same rules as undisclosed grants or investments.*

- [ ] No token generation event, executed or planned, exists for the applying entity or its principals within the prior 24 months.

- [ ] One or more token generation events, executed or planned, exist. Complete one table per event below.

| Field | Entry |
|---|---|
| **Event type** | [ ] IDO / [ ] TGE / [ ] ICO / [ ] Liquidity bootstrapping pool launch / [ ] Founder or contributor vesting schedule / [ ] Other: [specify] |
| **Status** | [ ] Executed / [ ] Planned (pending) |
| **Date or planned date** | [Date executed, or planned date if pending] |
| **Approximate value** | \$[USD value at time of event; for pending events, the planned allocation value based on the most recent publicly stated or implied valuation] |
| **Allocation summary** | [Who receives the tokens: entity, principals, investors, public, or a combination] |
| **Supporting document** | [Name the whitepaper, tokenomics document, or allocation schedule, with a publicly accessible location where available] |

*Copy this table for each additional token generation event.*

---

### Attestation

I confirm that the above is a complete and accurate disclosure of all active funding sources related to the scope of this application from the prior 24 months, all token generation events (executed or planned) within that window, and (for retroactive applications) all prior awards for the same or overlapping contribution. I understand that non-disclosure of concurrent funding or of a material token generation event is a disqualifier under CROSS, and that disclosure itself is not a disqualifier.

**Applicant Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 4

- [ ] One table per disclosed source
- [ ] Source type is specified for each entry
- [ ] Approximate amount is provided for each entry
- [ ] Grant period or investment date is provided for each entry
- [ ] Relationship to application scope is explained in free text for each entry
- [ ] Ongoing obligations are noted (yes/no with detail) for each entry
- [ ] Decision-making rights are noted (yes/no with detail) for each entry
- [ ] Token generation event disclosure is complete: either the "none" attestation is checked or one table per executed or planned event is provided
- [ ] If no sources: "None" is stated explicitly and attestation is signed
- [ ] Attestation is signed and dated

---

## Template 5: Adverse Signal Disclosure Form

*Applicants must surface signals that contradict their self-presentation: prior grant rejections from similar programs, contradictory technical findings, and negative due diligence results from other funders. Reviewers also have an obligation: adverse signals found during evaluation must not be suppressed.*

---

### Project Name

> [Enter project name]

### Applicant Name or Organization

> [Enter applicant name or organization]

---

### Initial Determination

**Do any adverse signals exist relating to this application?**

- [ ] No. I confirm that no prior rejections, contradictory technical findings, or negative due diligence results from other funders exist that are relevant to this application. Proceed to the attestation.

- [ ] Yes. Complete the signal disclosure table(s) below for each adverse signal.

---

### Signal Disclosure (one table per adverse signal)

| Field | Entry |
|---|---|
| **Signal type** | [ ] Prior rejection from a similar program / [ ] Contradictory technical finding / [ ] Negative due diligence from another funder / [ ] Other: [specify] |
| **Source** | [Name the program, funder, publication, or entity] |
| **Date** | [Date of the rejection, finding, or due diligence result] |
| **Brief description** | [Describe the adverse signal in plain terms] |
| **Applicant's explanation** | [Explain how this signal has been addressed, or why it does not affect this application's validity] |

*Copy this table for each additional adverse signal.*

---

### Attestation

I confirm that the above disclosure is complete and accurate to the best of my knowledge. I understand that non-disclosure of adverse signals is a process violation under the Adverse-Signal Engagement Principle Core Standard, whose requirements CROSS incorporates by reference. Disclosure does not disqualify this application; it initiates a structured engagement process.

**Applicant Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 5

- [ ] Initial determination is made (yes or no)
- [ ] If no: attestation is signed and dated
- [ ] If yes: one table per adverse signal, all fields complete
- [ ] Signal type is specified for each entry
- [ ] Source is named for each entry
- [ ] Date is provided for each entry
- [ ] Brief description is clear and accurate
- [ ] Applicant's explanation addresses the signal directly
- [ ] Attestation is signed and dated

---

## Template 6: Conflict of Interest Declaration Form - Reviewer Version

*Complete this form before beginning your review of any application. Submit to the designated receiving function (named by the committee; not the person making the funding decision). Do not begin review until you have submitted this declaration.*

---

### Reviewer Name

> [Enter reviewer name]

### Application(s) Being Reviewed

> [Enter application names or identifiers]

### Date of Declaration

> [Enter date]

---

### Tier 1: Categorical Bar - No Waiver Available

*If any Tier 1 relationship exists, you must recuse from this application immediately. There is no waiver process for Tier 1.*

**1a. Direct financial interest in the applicant entity**

*Includes equity, revenue share, or token holdings above the materiality threshold (greater than 1% of circulating supply or greater than the funder's stated materiality threshold in value at time of review).*

- [ ] This relationship exists. Applicant name: ___________________________ Nature of interest: ___________________________ Approximate value: ___________________________
- [ ] This relationship does not exist.

**1b. Family relationship with any principal, director, officer, or owner of the applicant project**

- [ ] This relationship exists. Applicant name: ___________________________ Nature of relationship: ___________________________
- [ ] This relationship does not exist.

**1c. Prior receipt of funding from this funder in the same program area, where your funded work is directly related to the applicant's scope**

- [ ] This relationship exists. Applicant name: ___________________________ Nature of relationship: ___________________________
- [ ] This relationship does not exist.

**1d. Named as a team member, advisor, or contributor on the applicant project's public materials**

- [ ] This relationship exists. Applicant name: ___________________________ Nature of listing: ___________________________
- [ ] This relationship does not exist.

---

### Tier 2: Disclosure Required - Qualified Waiver Possible

*If any Tier 2 relationship exists, do not begin review until written waiver approval is granted by the named authority. Waiver is not available where the relationship creates a financial interest.*

**2a. Employment with the applicant organization in the past 36 months**

- [ ] This relationship exists. Applicant: ___ Period: ___ Role: ___ Waiver justification: ___
- [ ] This relationship does not exist.

**2b. Co-authorship or active project collaboration with applicant principals in the past 48 months**

- [ ] This relationship exists. Applicant: ___ Nature: ___ Period: ___ Waiver justification: ___
- [ ] This relationship does not exist.

**2c. Mentor or student relationship with applicant principals (no expiration)**

- [ ] This relationship exists. Applicant: ___ Nature: ___ Waiver justification: ___
- [ ] This relationship does not exist.

**2d. Governance token voting power exercised on proposals affecting the applicant project**

- [ ] This relationship exists. Applicant: ___ Description: ___ Waiver justification: ___
- [ ] This relationship does not exist.

**2e. Decentralized autonomous organization co-membership in coordinating or committee roles within the same decentralized autonomous organization as the applicant**

- [ ] This relationship exists. Applicant: ___ Organization and role: ___ Waiver justification: ___
- [ ] This relationship does not exist.

**2f. Receipt of an honorarium, award, or gift from the applicant entity in the past 12 months**

- [ ] This relationship exists. Applicant: ___ Nature and value: ___ Waiver justification: ___
- [ ] This relationship does not exist.

**2g. Active job negotiations or arrangements for future employment with the applicant organization**

- [ ] This relationship exists. Applicant: ___ Nature: ___ Waiver justification: ___
- [ ] This relationship does not exist.

**2h. Organizational conflict: your employer has a material financial relationship with the applicant**

- [ ] This relationship exists. Applicant: ___ Nature of employer's relationship: ___ Waiver justification: ___
- [ ] This relationship does not exist.

---

### Tier 3: Disclosure Encouraged

*Disclose any social and community relationships, prior cross-round interactions, or informal mentorship that apply. If the reasonable third party standard is met (an informed observer would conclude you cannot maintain independence), treat the relationship as Tier 2 and request a waiver.*

> [Enter any Tier 3 relationships, or write "None to disclose"]

---

### Web3-Specific Categories

**Token holdings in the applicant project above the materiality threshold**

- [ ] Yes. Amount: ___________________________ (assign to Tier 1 above)
- [ ] No.

**Governance token voting on applicant project proposals**

- [ ] Yes. Description: ___________________________ (assign to Tier 2 above if not financial)
- [ ] No.

**Core contributor or unpaid advisory status on applicant project**

- [ ] Yes. Nature of role: ___________________________ (assign to Tier 1 or Tier 2 depending on nature)
- [ ] No.

**Receipt of investment from the same named investor backing the applicant**

- [ ] Yes. Investor name: ___________________________ (assess under Tier 2 or Tier 3)
- [ ] No.

**Decentralized autonomous organization co-coordinating roles shared with the applicant**

- [ ] Yes. Description: ___________________________ (assess under Tier 2 or Tier 3)
- [ ] No.

---

### Attestation

I confirm that this declaration is complete and accurate to the best of my knowledge. I understand that undisclosed Tier 1 relationships constitute a disqualifying violation and that undisclosed Tier 2 relationships constitute a process violation requiring remediation. The reasonable third party standard applies to novel relationship types not listed above.

**Reviewer Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 6

- [ ] All Tier 1 items are checked (yes or no)
- [ ] If any Tier 1 item is checked yes: recusal has been initiated and committee notified
- [ ] All Tier 2 items are checked (yes or no)
- [ ] If any Tier 2 item is checked yes: waiver justification provided and waiver request submitted before review begins
- [ ] Tier 3 free text is completed or "None to disclose" is stated
- [ ] All web3-specific categories are checked
- [ ] Attestation is signed and dated
- [ ] Declaration submitted to the designated receiving function before review begins

---

## Template 7: Conflict of Interest Declaration Form - Applicant Version

*Applicants are required to disclose relationships to committee members and reviewers known to them. This form covers relationships you are aware of at the time of submission. Submit with your application.*

---

### Project Name

> [Enter project name]

### Applicant Name or Organization

> [Enter applicant name or organization]

### Date of Declaration

> [Enter date]

---

### Disclosure of Known Relationships to Committee Members and Reviewers

*For each committee member or reviewer whose identity is known to you, assess whether any of the relationships below exist. You are not required to research the identities of reviewers you do not already know.*

| Committee member or reviewer name | Nature of relationship | Tier assessment | Notes |
|---|---|---|---|
| [Name] | [Description] | Tier [ ] 1 / 2 / 3 | [Any additional context] |
| [Add rows as needed] | | | |

*If no known relationships exist, write "None known" in the first row.*

---

### Tier Definitions for Applicant Reference

**Tier 1 (categorical Bar):** Direct financial interest in the reviewer from your project, family relationship, or having the reviewer named on your project's public materials.

**Tier 2 (disclosure Required, Qualified Waiver Possible):** Employment of the reviewer by your organization in the past 36 months, co-authorship or active collaboration in the past 48 months, mentor or student relationship, governance token voting by the reviewer on your project's proposals, or organizational financial relationship between your project and the reviewer's employer.

**Tier 3 (disclosure Encouraged):** Social and community relationships, prior cross-round interactions, informal mentorship or advisory conversations.

---

### Web3-Specific Categories

**Committee member or reviewer holds tokens in your project above the materiality threshold**

- [ ] Yes. Name(s) and description: ___________________________
- [ ] No known instances.

**Committee member or reviewer has governance voting power on your project's proposals**

- [ ] Yes. Name(s) and description: ___________________________
- [ ] No known instances.

**Committee member or reviewer is a core contributor or unpaid advisor on your project**

- [ ] Yes. Name(s) and description: ___________________________
- [ ] No known instances.

**Committee member or reviewer received investment from the same named investor as your project**

- [ ] Yes. Investor name and description: ___________________________
- [ ] No known instances.

---

### Attestation

I confirm that this declaration is complete and accurate to the best of my knowledge. I understand that this form covers relationships I am aware of at the time of submission and that I will notify the committee administrator promptly if I become aware of additional relevant relationships after submission.

**Applicant Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 7

- [ ] All known relationships are listed, or "None known" is stated
- [ ] Each disclosed relationship is assigned to a tier
- [ ] Web3-specific categories are assessed and checked
- [ ] Attestation is signed and dated
- [ ] Submitted with the application

---

## Template 8: Post-Participation Conflict of Interest Certification - Reviewer Version

*Complete this form after your review of an application is complete. Submit to the designated receiving function alongside your review output.*

---

### Reviewer Name

> [Enter reviewer name]

### Application(s) Reviewed

> [Enter application names or identifiers]

### Date of Review Completion

> [Enter date]

---

### Certification

**1. No new conflicts arose during review.**

During my review of the application(s) listed above, no new relationships, financial interests, or other conflicts arose that were not disclosed in my pre-review conflict of interest declaration. My pre-review declaration remained accurate throughout the review process.

- [ ] Confirmed.
- [ ] Not confirmed. I became aware of the following during review: ___________________________ *(Submit this form to the committee administrator immediately for remediation guidance.)*

**2. Declaration remained accurate.**

The relationships and declarations in my pre-review conflict of interest declaration accurately reflected my situation throughout the review period.

- [ ] Confirmed.
- [ ] Not confirmed (see above).

---

**Reviewer Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 8

- [ ] Reviewer name and application(s) reviewed are listed
- [ ] Date of review completion is provided
- [ ] Certification items 1 and 2 are both checked confirmed, or discrepancy is described and reported
- [ ] Signed and dated
- [ ] Submitted to the designated receiving function

---

## Template 9: Privacy-Sensitive Context Accommodation Request

*For applications invoking the privacy-sensitive accommodation for indicator sourcing. The accommodation specifies which obligation mechanisms are appropriate to a context where standard measurement would compromise the safety of affected-population members; it is not an exemption from obligation. Submit with the Indicator Registration Form for the affected indicator(s).*

---

### Project Name

> [Enter project name]

### Applicant Name or Organization

> [Enter applicant name or organization]

### Indicator Number(s) Affected

*Reference the indicator number from Template 3.*

> [Enter indicator number(s)]

---

### Field 1: Standard Measurement Methodology That Would Normally Apply

*Describe the standard approach that would typically be used for this type of indicator if no privacy concern existed.*

> [Enter the standard methodology that would normally apply]

---

### Field 2: Specific Harm the Standard Methodology Would Create

*Name the specific harm, concretely: the population, the mechanism of harm (legal exposure, identification by state actors, retaliation risk), and why this harm is supportable in the specific context. Generic references to "privacy" do not satisfy this field.*

> [Enter the specific harm, population, and harm mechanism]

---

### Field 3: Alternative Methodology Proposed

**Description of alternative methodology**

> [Enter description of the alternative methodology]

**How this methodology produces verifiable outcome evidence**

*Explain how an independent reviewer could confirm, without access to affected-population-identifying information, that the claimed outcome was produced.*

> [Enter explanation of verifiability]

---

### Field 4: Institutional Partner or Established Methodology

*The alternative must draw on an institutional partner or established methodology recognized in the relevant field.*

**Named partner or methodology**

> [Name the partner or methodology]

**Explanation of appropriateness**

> [Explain why this partner or methodology is appropriate to this specific context]

---

### Field 5: Confirmation of Verifiable Outcome Evidence

- [ ] I confirm that the alternative methodology will produce verifiable outcome evidence that an independent reviewer can assess without requiring access to affected-population-identifying information.

> [Enter confirmation, or describe which condition is not met and what alternative assurance mechanism you propose]

---

### Attestation

**Applicant Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 9

- [ ] Standard methodology is named specifically
- [ ] Specific harm is described concretely with named population and harm mechanism
- [ ] Alternative methodology is described in sufficient detail for independent assessment
- [ ] Explanation of verifiability is provided
- [ ] Institutional partner or established methodology is named
- [ ] Confirmation of verifiable outcome evidence is checked
- [ ] Attestation is signed and dated
- [ ] Submitted with the relevant Indicator Registration Form

---

## Template 10: Gate Evidence Submission Form

*Use this form to submit evidence at a progress verification gate or a completion verification gate. Do not use this form at the entry specification stage; the entry specification is part of the application. Submit to the designated funder contact by the published gate deadline.*

---

### Project Name

> [Enter project name]

### Grant Reference

> [Enter grant identifier or round name]

### Gate Being Submitted For

- [ ] Progress verification gate (tranche disbursement)
  - Which tranche: _______________
  - Published gate deadline: _______________
- [ ] Completion verification gate (final payment)
  - Published gate deadline: _______________
- [ ] Continuation specification gate (progression to next stage)
  - Stage being applied for: _______________

### Date of Submission

> [Enter date]

---

### Round Configuration (confirm from published round specification)

**Obligation Mode:** [ ] Build / [ ] Change / [ ] Retroactive

**Evidence Scope Required At This Gate:** [ ] Output / [ ] Usage / [ ] Outcome / [ ] Impact

**Evidence Strength Required At This Gate:** [ ] Self-report with documentation / [ ] Third-party verifiable / [ ] Independent review / [ ] Independent evaluation

---

### Evidence Package

*Complete the section that matches the obligation mode.*

---

**Build Obligation Evidence**

**Deliverable status**

*Describe what has been produced and its current state relative to the published completion criteria.*

> [Enter deliverable status]

**Evidence of public accessibility** *(required at completion verification gate)*

*Provide the public URL, repository link, registry entry, or other publicly accessible location where the deliverable can be found and verified.*

> [Enter public location]

**Completion criteria check**

*For each completion criterion stated in the entry specification (Template 1A or Template 3), confirm whether it is met and provide evidence.*

| Criterion | Status | Evidence |
|---|---|---|
| [Criterion from entry spec] | [ ] Met / [ ] In progress / [ ] Not yet met | [Named evidence source or artifact] |
| [Add rows as needed] | | |

**Named verifying party** *(required if gate is at independent review level)*

*Name the party who has confirmed the deliverable meets the completion criteria.*

> [Enter verifying party name and role, or write "Not required at this gate level"]

---

**Change Obligation Evidence**

**Indicator and reporting period**

*Name the primary indicator and the period this submission covers.*

> Indicator: _______________
> Reporting period: _______________

**Reported value**

> Value: _______________
> Source: _______________
> Collection date: _______________

**Change from baseline**

> Baseline (FROM state): _______________
> Current value: _______________
> Target (TO state): _______________
> Progress toward target: _______________

**Evidence documentation**

*Provide the publicly accessible evidence source or attach the evidence package. Name the source and the collection method used.*

> [Enter evidence source and collection method]

**Named reviewer** *(required if gate is at independent review level)*

> [Enter reviewer name and role, or write "Not required at this gate level"]

---

**Retroactive with Forward Commitment**

**Forward commitment reference**

*Reference the commitment stated in Template 1B.*

> [Enter commitment description]

**Completion status**

> [Describe what was completed and when]

**Completion evidence**

> [Named publicly accessible evidence that the commitment was fulfilled]

---

### Applicant Attestation

I confirm that the evidence submitted in this form is accurate and complete to the best of my knowledge. I understand that grantee self-report alone does not satisfy the completion verification gate and that the funder will review this submission against the published completion criteria before releasing final payment.

**Applicant Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 10

- [ ] Project name, grant reference, and gate type are specified
- [ ] Round configuration (mode, evidence scope, evidence strength) is confirmed from the published round specification
- [ ] Evidence section appropriate to the mode is completed
- [ ] For build obligation at completion gate: public accessibility location is provided
- [ ] For gates at independent review level: named reviewer or verifying party is identified
- [ ] Applicant attestation is signed and dated
- [ ] Submitted by the published gate deadline

---

## Template 11: Organizational Identity Declaration

*Required at the entry specification gate in all obligation modes. The organizational identity declaration is a pre-condition for gate assessment, not a scored criterion: an entry submission that omits it is incomplete and is not assessed until it is provided. Complete all six fields. Disclosure is not a disqualifier; non-disclosure of a publicly documentable fact is. Submit with your application.*

---

### Project Name

> [Enter project name]

---

### Field 1: Legal Entity Name and Jurisdiction

*The name of the natural person or registered organization exactly as it appears in the relevant jurisdiction of registration, and the jurisdiction itself. A project name, display name, or code-hosting organization name does not satisfy this field unless it is also the legal name. Where no legal entity exists, state this explicitly and name the individual who is personally answerable for the obligation.*

**Legal entity name**

> [Enter legal name, or state "No legal entity exists" and name the responsible individual]

**Jurisdiction of registration**

> [Enter jurisdiction, or write "Not applicable" with explanation]

---

### Field 2: Parent Organization Declaration

*Whether the applicant operates under or is affiliated with a larger organization, network, or chapter structure. Where a parent organization exists, state its name. Where the applicant is a chapter, working group, or sub-entity, describe the relationship: does the parent know about this application, does it share the applicant's brand or personnel, and is it separately applying to this or a concurrent round of the same program? Silence is not acceptable where an affiliation is publicly documented or where the applicant's name, brand, or personnel overlaps with a known larger organization.*

- [ ] No parent organization exists. The applicant is independent.

- [ ] A parent organization exists. Name and relationship:

> [Enter parent organization name; state whether it knows of this application, whether brand or personnel are shared, and whether it is separately applying to this or a concurrent round]

---

### Field 3: Affiliated Entity Disclosure

*Any other organization, project, or entity that shares the applicant's name, brand, domain, key personnel, or codebase, whether or not a formal legal relationship exists. This field surfaces name collisions, internal fragmentation, and personnel overlap. Disclosure is not a disqualifier; non-disclosure of a publicly documentable affiliation is.*

- [ ] No affiliated entities exist.

- [ ] Affiliated entities exist. List each below.

| Entity name | What is shared (name, brand, domain, personnel, codebase) | Nature of the relationship |
|---|---|---|
| [Entity name] | [What is shared] | [Description] |
| [Add rows as needed] | | |

---

### Field 4: Prior Round History

*Whether the applicant, or any substantially overlapping entity (same personnel, same codebase, same project name, or same legal entity under a different display name), has applied to this program in prior rounds, under what name, and with what outcome. This field catches serial rebranding.*

- [ ] No prior application history with this program exists for the applicant or any overlapping entity.

- [ ] Prior application history exists. Complete the table below.

| Round or period | Name applied under | Outcome |
|---|---|---|
| [Round] | [Name] | [Funded / rejected / withdrawn / other] |
| [Add rows as needed] | | |

*Where a prior funder's gate determination exists as a publicly verifiable signed record, you may cite it here as corroboration, and the reviewing program may query it as independent verification of the claimed history.*

> [Enter any signed gate record reference, or write "None available"]

---

### Field 5: Disbursement Authority

*The named person or persons with legal authority to receive grant funds on behalf of the applying entity and approve their deployment. An entry submission without this declaration is incomplete.*

Select the state that applies:

- [ ] **Individual.** One named person with full authority.

> Name: ___________________________

- [ ] **Collective.** Shared authority through a named mechanism.

> Mechanism: ___________________________
> Current key holders: ___________________________
> Quorum threshold: ___________________________

- [ ] **Delegated.** Authority by role.

> Role: ___________________________
> Current holder: ___________________________
> Transfer mechanism: ___________________________

*For a decentralized autonomous organization applicant without a legal wrapper, name the controlling wallet address and the coordinating mechanism, with current token holders above the materiality threshold named where possible.*

> [Enter controlling wallet address and coordinating mechanism, where applicable]

---

### Field 6: On-Chain Identity Anchor

*The canonical wallet address by which the applying entity is identifiable across blockchain programs and grant databases. For entities with prior blockchain grant history, this is the address registered in those programs. For entities without prior history, this is the address that will serve as the identity root for this program's records. The anchor is used by the funder for cross-program identity matching and Attestation Corpus queries; it is not a fund receipt address unless it also serves as the disbursement authority. Non-disclosure of an on-chain address publicly associated with the applicant in any grant database is a conformance failure equivalent to non-disclosure in Field 3.*

**On-chain identity anchor address**

> [Enter wallet address]

**Is this address the same as the disbursement authority address?**

- [ ] Yes, the on-chain identity anchor and the disbursement authority are the same address.
- [ ] No, they are different addresses.

---

### Completion Checklist - Template 11

- [ ] Legal entity name and jurisdiction are provided, or absence of a legal entity is stated with a named responsible individual
- [ ] Parent organization declaration is complete (either "none" or named with relationship described)
- [ ] Affiliated entity disclosure is complete (either "none" or each entity listed)
- [ ] Prior round history is complete (either "none" or table provided)
- [ ] Disbursement authority state is selected and the matching fields are filled
- [ ] On-chain identity anchor is provided and its relationship to the disbursement authority address is stated
- [ ] No fields left blank

---

## Template 12: Sufficiency Architecture Declaration

*Required at the entry specification gate in all obligation modes, alongside the organizational identity declaration. It is a pre-condition for gate assessment. The declaration collects five elements: a scope declaration, a sufficiency position, a portfolio context statement, a grant contribution statement, and the revenue architecture declaration (the last applies to all applicants). Submit with your application.*

---

### Project Name

> [Enter project name]

---

### Element 1: Scope Declaration

*The specific program, sub-entity, or aspect of your work that this application covers, stated clearly enough that an independent reviewer could determine what falls within it and what falls outside it. Where the application covers your entire operation, state this explicitly. Declaring the scope is what allows evaluators to assess additionality and attribute outcomes.*

> [Enter the scope this application covers, and what falls outside it]

---

### Element 2: Sufficiency Position

*Your current resource position at the declared scope, not at the entity level overall. Select one.*

- [ ] **Critical gap.** Resources cover less than half of full scope requirements, and the program's viability depends on closing this gap.
- [ ] **Partial.** Resources cover more than half, but the program operates below intended capacity.
- [ ] **Approaching.** Resources are sufficient for current operations but not for the next intended scope expansion.
- [ ] **Surplus.** Resources exceed current scope requirements in the current period.

**Corroborating evidence (required)**

*The sufficiency position requires at least one piece of corroborating evidence from a source outside your control. Acceptable evidence: publicly accessible treasury data (on-chain balance, Open Collective balance, or equivalent); grant history records from a named external database (KarmaGAP, Gitcoin Explorer, RPGF recipient lists, or equivalent); or disclosed revenue figures from a named independent source. A declaration with no corroborating evidence is accepted at self-report strength only. Where no publicly accessible corroborating evidence exists (for example, a recently formed entity with no prior funding history), state this explicitly and explain why the declared position is reasonable given the absence of verifiable evidence.*

> [Enter the named corroborating source and what it confirms, or state the absence of evidence with explanation]

---

### Element 3: Portfolio Context Statement

*How other funding sources in your funding architecture address other scopes or aspects of your work. This is not concurrent funding disclosure (which asks about other funding for the same scope); it asks how you have organized your pursuit of sufficiency across all your programs, so this application can be evaluated as part of a coherent architecture. Other funding sources for other scopes are expected and are not a disqualifier. Silence about other funding sources in an entity with multiple programs requires explicit explanation.*

> [Enter the portfolio context, or explain the absence of other funding sources]

*Where co-funding is documented in a publicly verifiable coordination record before any work begins, name that record here; it constitutes independently verifiable evidence of this statement.*

> [Enter coordination record reference, or write "None"]

---

### Element 4: Grant Contribution Statement

*What specific gap at the declared scope this grant would close, and what the sufficiency position at that scope would be after the grant's contribution. This is a declaration of where in the sufficiency architecture the grant fits, not a promise about what will be achieved.*

> [Enter the gap this grant closes and the resulting sufficiency position at the declared scope]

---

### Element 5: Revenue Architecture Declaration

*Required for all applicants. Declare your revenue architecture type. For grant-only applicants, this confirms that no commercial revenue model exists. For fee-for-service, commercial, and hybrid applicants, this activates the additionality delineation requirement: you must identify which portion of your work or budget the commercial revenue does not cover, and the grant must be scoped to that non-commercial portion.*

- [ ] **Grant-only.** No commercial revenue model exists.
- [ ] **Fee-for-service.**
- [ ] **Commercial.**
- [ ] **Hybrid.**

*If fee-for-service, commercial, or hybrid: identify the portion of your work or budget the commercial revenue does not cover, to which this grant is scoped.*

> [Enter the non-commercial portion the grant is scoped to, or write "Not applicable: grant-only"]

---

### Completion Checklist - Template 12

- [ ] Scope declaration states what is in and out of scope
- [ ] Sufficiency position is selected (one of four)
- [ ] Corroborating evidence from a source outside the applicant's control is named, or its absence is explained
- [ ] Portfolio context statement is provided, or absence of other funding is explained
- [ ] Grant contribution statement names the gap closed and the resulting position
- [ ] Revenue architecture type is selected
- [ ] For fee-for-service, commercial, or hybrid: the non-commercial portion the grant is scoped to is identified
- [ ] No fields left blank

---

## Template 13: Public Benefit Mechanism and Access Condition Declaration

*Required at the entry specification gate for any application whose eligibility is assessed against a public goods claim. Where active, it is a pre-condition for gate assessment alongside Templates 11 and 12: an entry submission that includes a public goods claim but omits this declaration is incomplete. The declaration collects two elements: a mechanism type statement and an access condition statement. The mechanism type declared at entry constrains the evidence scope required at the completion gate. Submit with your application.*

---

### Project Name

> [Enter project name]

---

### Element 1: Mechanism Type Statement

*Which of the four mechanism types your public goods claim rests on. Each commits you to a minimum evidence scope at the completion gate. A declared mechanism that cannot be supported by the evidence scope available at the completion gate is a misrepresentation in the entry specification. If the program's round configuration accepts only certain mechanism types, select only from those accepted.*

- [ ] **Output production.** Benefit arises from producing an artifact and releasing it openly. Commits to output evidence at minimum.
- [ ] **Access provision.** Benefit arises from providing access to a resource. Commits to usage evidence.
- [ ] **Condition change.** Benefit arises from changing a condition in a defined population. Commits to outcome evidence.
- [ ] **Ecosystem shift.** Benefit arises from shifting an ecosystem-level condition. Commits to a documented impact contribution argument.

---

### Element 2: Access Condition Statement

*The specific terms under which the declared mechanism delivers benefit to the stated population, specified with enough precision that an independent reviewer could confirm them without contacting you. The required content is determined by the mechanism type. Complete the block matching your selection above.*

**For output production**

*Provide the SPDX license identifier and the location of the license file. A copyright notice that permits free viewing without granting modification or redistribution rights does not satisfy this condition. A "source available" or "fair code" license that restricts commercial use does not satisfy it unless the program's published round configuration explicitly accepts such licenses and states the accepted SPDX identifiers. The license must be present in the artifact at the completion gate; a future licensing commitment without a current license does not satisfy the condition at entry.*

> SPDX license identifier: ___________________________
> License file location: ___________________________

*Is the license applied to the outputs now, or committed for the completion gate?*

- [ ] Applied now.
- [ ] Will be applied by the completion gate. Date or condition: ___________________________

**For access provision**

> Access mechanism: ___________________________
> Cost structure: ___________________________
> Non-excludability mechanism: ___________________________

**For condition change**

> FROM state: ___________________________
> Population definition: ___________________________

**For ecosystem shift**

> Named causal pathway: ___________________________
> Co-factor list: ___________________________

---

### Element 3: Timing of the Access Condition

*State whether the access conditions are current at the time of application, will be achieved at the completion gate, or both.*

- [ ] Current at the time of application.
- [ ] Will be achieved at the completion gate.
- [ ] Both.

---

### Completion Checklist - Template 13

- [ ] Mechanism type is selected (one of four), and is among the types the program accepts
- [ ] The access condition block matching the selected mechanism type is complete
- [ ] For output production: an SPDX license identifier and license file location are provided, and license timing is stated
- [ ] Timing of the access condition is stated (current, at completion gate, or both)
- [ ] The declared mechanism is consistent with the evidence scope available at the completion gate
- [ ] No fields left blank

---

## Template 14: Development Stage Declaration

*Required at the entry specification gate in all rounds. Universal. The declared stage constrains which obligation modes are coherent and which evidence scopes are achievable at the completion gate. Funders declare in their round configuration which stages are within scope; check the published configuration before completing this form. A declared stage not supported by the provided evidence is a material discrepancy requiring investigation. Submit with your application.*

---

### Project Name

> [Enter project name]

---

### Field 1: Declared Stage

*Select one. Each stage carries a minimum evidence requirement, stated in the field.*

- [ ] **Stage 1: Proof of concept.** Provide output evidence of the existing artifact.
- [ ] **Stage 2: Early adoption.** Provide usage evidence from at least one named external user.
- [ ] **Stage 3: Growth.** Provide independently verifiable adoption data with a trend.
- [ ] **Stage 4: Established infrastructure.** Provide 12 months of sustained usage data from sources outside the team.
- [ ] **Stage 5: Retroactive recognition.** Provide prior contribution evidence in the entry submission.

---

### Field 2: Why This Stage Rather Than an Adjacent One

*Describe why your work is at the declared stage and not the stage below or above it. A Stage 1 declaration paired with independent usage evidence, or a Stage 3-or-higher declaration paired with no independently verifiable adoption data, is a discrepancy a reviewer will investigate.*

> [Enter the description]

---

### Field 3: Evidence Confirming the Declared Stage

*At least one piece of evidence from a source outside your control, matching the minimum for your declared stage above.*

| Evidence | Source (outside applicant control) | What it confirms about the stage |
|---|---|---|
| [Describe the evidence] | [Named source] | [What it confirms] |
| [Add rows as needed] | | |

---

### Field 4: Consistency With Obligation Mode

*The declared stage constrains obligation mode selection. A Stage 1 applicant committing to a change obligation must provide a FROM state and population baseline at entry, coherent only if the Stage 1 artifact is specifically designed to measure against an existing condition. A Stage 4 applicant selecting a build obligation must specify what new functionality is added beyond sustained operation. Confirm consistency or explain it.*

> [Enter confirmation of consistency between declared stage and obligation mode, or the explanation]

---

### Completion Checklist - Template 14

- [ ] Declared stage is selected (one of five) and is within the round's published scope
- [ ] Explanation of why this stage rather than an adjacent one is provided
- [ ] At least one piece of evidence from a source outside the applicant's control is provided, matching the stage minimum
- [ ] Consistency between the declared stage and the chosen obligation mode is confirmed or explained
- [ ] No fields left blank

---

## Template 15: Continuity Capacity Declaration

*Required where the Continuity Capacity dimension is active: grants above a funder-defined size threshold, grants producing ongoing infrastructure with continuing operational requirements, and any application where the applying entity has a single named primary contributor and no documented backup capacity. For programs that fund infrastructure maintenance or sustained service delivery, this dimension is always active. The declaration of a single point of failure is not a disqualifier; it is a material fact affecting the sustainability assessment at the continuation gate. Submit with your application where the dimension is active.*

---

### Project Name

> [Enter project name]

---

### Field 1: Resilience State

*Declare one of three states, with supporting evidence.*

- [ ] **Single.** Continuation depends on one named person, with no documented backup capacity.
- [ ] **Partial.** Some continuity capacity exists beyond a single person, but it is incomplete.
- [ ] **Resilient.** Continuity does not depend on any single person; documented backup capacity exists.

---

### Field 2: Supporting Evidence

> [Enter the evidence supporting the declared state: named roles, documented backup arrangements, key-holder lists, or equivalent]

---

### Field 3: Single Point of Failure Detail (complete if "Single" or "Partial" is declared)

*For single-point-of-failure continuity, name the person on whom continuation depends and state what would happen to active grants and funded deliverables if that person became unavailable.*

**Person on whom continuation depends**

> [Enter name or role]

**What would happen to active grants and funded deliverables if that person became unavailable**

> [Enter the description]

---

### Field 4: Acknowledgement of Completion Gate Conditions

*A funder may configure the completion gate to require evidence of partial or resilient continuity as a condition of final disbursement for grants above the threshold. Confirm you have reviewed the published round configuration for any such condition.*

- [ ] I have reviewed the round configuration and understand whether evidence of partial or resilient continuity is a condition of final disbursement for this grant.

---

### Completion Checklist - Template 15

- [ ] Resilience state is declared (one of three)
- [ ] Supporting evidence for the declared state is provided
- [ ] For single or partial states: the person depended upon is named and the consequence of their unavailability is stated
- [ ] The completion gate condition acknowledgement is checked
- [ ] No fields left blank

---

## Template 16: Obligation Fulfillment Record (Returning Applicants)

*Required at the entry specification gate, before gate assessment proceeds, where any of these apply: you have received prior grants from this funder in any prior round; you cite prior work as evidence of capability at the entry gate; or your prior round history includes unresolved KarmaGAP milestones or open gate conditions. An unfulfilled prior obligation is not automatically disqualifying; it is a disclosed fact affecting the track record assessment. An unfulfilled obligation that is not disclosed here but is discovered through research is a material discrepancy: non-disclosure of a prior failure is treated more seriously than the failure itself. Submit with your application where applicable.*

---

### Project Name

> [Enter project name]

---

### Prior Grant Record (one table per prior grant from this funder)

| Field | Entry |
|---|---|
| **Prior round or grant reference** | [Round name or grant identifier] |
| **Obligation mode of that round** | [ ] Build / [ ] Change / [ ] Retroactive |
| **What was committed at the entry gate** | [The deliverable specification, the FROM-TO state, or the contribution evidence, as appropriate to the mode] |
| **What was produced during the grant period** | [The artifact, the measured change, or the verified contribution, with a publicly accessible link] |
| **Fulfillment status** | [ ] Fulfilled / [ ] Partially fulfilled / [ ] Unfulfilled |
| **Explanation where fulfillment was not complete** | [What prevented fulfillment and what has changed since; required where status is partial or unfulfilled] |

*Copy this table for each additional prior grant from this funder.*

---

### Attestation

I confirm that this record is a complete and accurate account of my prior obligations to this funder and of the prior work I cite as evidence of capability. I understand that non-disclosure of a prior obligation that is later discovered through research is treated more seriously than the underlying failure itself.

**Applicant Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 16

- [ ] One table per prior grant from this funder
- [ ] Obligation mode of each prior round is stated
- [ ] What was committed at the entry gate is recorded for each
- [ ] What was produced is recorded for each, with a publicly accessible link
- [ ] Fulfillment status is stated for each
- [ ] Where status is partial or unfulfilled: an explanation is provided
- [ ] Attestation is signed and dated

---

## Template 17: Prior Work Attribution Statement

*Required wherever an applicant cites prior work as evidence of capability, track record, or past contribution in any entry gate submission. This activates for all three obligation modes: build-obligation applicants citing prior deliverables; change-obligation applicants citing prior outcomes as a baseline or established methodology; and retroactive-obligation applicants whose entire entry submission consists of prior work. The statement is an adverse signal disclosure requirement: an applicant who cannot truthfully complete it for cited prior work has surfaced a misrepresentation in the core evidential basis of the application. Submit with your application where applicable.*

---

### Project Name

> [Enter project name]

---

### Prior Work Attribution (one block per piece of prior work cited)

**Cited prior work**

> [Name and briefly describe the prior work cited]

**Question 1: Entity of performance**

*Under which legal entity or organizational context was the cited work performed? If it was performed as an employee, contractor, or contributor to an organization that is not the applying entity, name that organization. If it was performed under the applying entity's own resources, state that explicitly.*

> [Enter the entity of performance]

**Question 2: Applicant's relationship at the time and now**

*What was your role in the entity under which the work was performed, and what is the current status of that relationship? State both the relationship at the time of creation and the relationship at the time of application. An individual who founded a project within an organization and has since departed is in a materially different position from one who founded and has controlled an independent project throughout.*

> [Enter relationship at the time of creation and at the time of application]

**Question 3: Current ownership and access**

*Who currently holds the intellectual property rights to the cited work, who controls the deployment or codebase, and who has the user relationship with any users cited as evidence of impact? If the applying entity does not hold the rights, does not control the deployment, or does not have the relationship with the cited users, state this.*

> [Enter current ownership, control of deployment, and user relationship]

*Copy this block for each additional piece of prior work cited.*

---

### Attestation

I confirm that this attribution statement is complete and accurate for each piece of prior work I cite. I understand that citing work performed under a different entity, without that entity's knowledge or endorsement of this application, claims responsibility for outcomes I did not control.

**Applicant Signature (or Equivalent Attestation):** ___________________________

**Date:** ___________________________

---

### Completion Checklist - Template 17

- [ ] One block per piece of prior work cited
- [ ] Entity of performance is named for each
- [ ] Relationship at the time of creation and at the time of application is stated for each
- [ ] Current ownership, control of deployment, and user relationship are stated for each
- [ ] Attestation is signed and dated

---

*End of CROSS Templates, version 0.3.0.*
