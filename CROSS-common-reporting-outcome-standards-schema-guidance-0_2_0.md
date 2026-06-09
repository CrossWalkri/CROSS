---
title: CROSS - Common Reporting Outcome Standards Schema - Guidance
version: 0.3.1
date: 2026-06-08
license: CC0
status: Working draft. Companion guidance document synced to CROSS-common-reporting-outcome-standards-schema-0_5_0.md. Supersedes version 0.2.0.
---

# CROSS: Common Reporting Outcome Standards Schema - Guidance

Version 0.3.1 | 2026-06-08 | CC0

---

This document is the practitioner companion to CROSS (Common Reporting Outcome Standards Schema) version 0.5.0. It does not restate the standard. It explains how to apply the standard's criteria, what qualifies and what does not at each decision point, and what the most common failure modes look like. It is written for two audiences: applicants completing a CROSS-conformant grant application, and reviewers evaluating one.

This version of the guidance covers three obligation modes: build obligation, change obligation, and retroactive obligation. Part 1 covers the entry specification for each mode. Part 2 covers the gate architecture. Part 2-A covers the entry-gate declarations the standard requires before any gate assessment proceeds. Parts 3 through 9 cover indicator specification and conformance requirements that apply across modes, with mode-specific notes where the application differs.

**A note on what CROSS inherits.** CROSS is a domain application of CRAFT (Chains Reveal Attested Falsifiable Truth), the meta-standard for evaluation chain legibility. A program that adopts CROSS thereby satisfies CRAFT's six conditions for its grant evaluations; there is no separate CRAFT implementation step. Practitioners do not need to read CRAFT to apply this guidance. The full record of which CRAFT conditions CROSS realizes, which upstream standards it rests on, and where named gaps remain open is the CRAFT inheritance receipt in Part XIII of the standard. The practical consequence for a reviewer is that the entry-gate declarations, the gate determinations, and the indicator fields described in this guidance are not local preferences of one program: they are how CROSS makes a grant evaluation a chain that an independent party can rely on.

---

## Part 1: How to Answer the Entry Specification

### 1A: Build Obligation

**What the entry gate is asking.** Can the applicant name a falsifiable deliverable with independently verifiable completion criteria?

A falsifiable deliverable is an artifact, product, or documented output whose existence and quality can be confirmed by a reviewer who did not commission the work. The test is not whether the deliverable will be valuable or widely adopted. The test is whether a reviewer at the end of the grant period, looking at what was submitted, could determine whether it was done.

**What makes a deliverable specification falsifiable.** A deliverable specification is falsifiable when the completion criteria are specific enough that failure is a recognizable outcome. "Build a reporting tool" is not falsifiable because any tool, however incomplete, could be claimed to satisfy it. "A reporting module that produces a human-readable fee summary for any ERC-4626 vault, published as an open-source library under MIT license, with at least one deployed instance on Ethereum mainnet, a documented application programming interface, and a test suite covering the three functions specified in the design document" is falsifiable because a reviewer can check each element.

The completion criteria do not need to be technical. "A research report of at least 15,000 words, published under a Creative Commons open license, covering the three questions named in the application's research plan, with a literature review, at least five primary source interviews, and a named target audience who received the draft before publication" is falsifiable. The reviewer can count words, check the license, verify the scope, and confirm whether the interviews and review were conducted.

**What disqualifies a build-obligation entry specification.** The primary failure mode is offering a direction or vision in place of a deliverable. "Making DeFi more transparent" is a direction. "Building better tooling for privacy" is a direction. A direction cannot be verified at grant end because it does not specify what done looks like. An application that describes what it is trying to achieve, not what it will produce, fails the entry gate.

A second failure mode is naming a deliverable without specifying completion criteria. "A working prototype" names a form (a prototype) but not a standard (what working means). A reviewer cannot verify whether a prototype is working without criteria. The entry gate requires both: a named artifact and verifiable criteria for what counts as complete.

**Build obligation is not the same as "has begun building."** Some programs incorrectly apply change-obligation gate logic to build-obligation applications, treating an applicant who has already started building as though that is a suspicious circumstance. It is not. A team that has already built part of what they are proposing is in a stronger position to specify the deliverable and the completion criteria precisely, because they have working knowledge of the problem. The entry gate asks whether the commitment is falsifiable; it does not ask when the work began.

**The deliverable specification at different scales.** A small-team discovery sprint and a large multi-stage development program both use build obligation, but the depth of specification is calibrated to scale. A small team committing to a design document needs: the document type, the scope (what questions it addresses or what design decisions it makes), the format for delivery (public publication, named repository, or named partner), and what constitutes a complete document. A large development program additionally needs: milestone-level completion criteria for each grant period, a named verification mechanism at the completion gate, and evidence that the deliverable will be publicly accessible.

---

### 1B: Change Obligation

**What the entry gate is asking.** Can the applicant name the FROM state as a specific measurable condition in a defined population?

This is the gate that appeared in version 0.1.0 as the sole entry gate. In version 0.2.0, it is correctly scoped to change-obligation rounds. The Theory of Build gate now refers to a named failure mode within this mode (offering a deliverable commitment where a problem diagnosis is required), not to the gate itself.

**The FROM state.** A FROM state is specific when it names a condition. A condition describes an observable state that exists in the world and can be measured. A category describes a type of problem without grounding it in an observable measurement. The difference matters because conditions can be verified; categories cannot.

A FROM state that passes: "96 to 99 percent network reachability drops for users in Iran during government-imposed shutdowns, as measured by Open Observatory of Network Interference probe data from 2023 to 2025." This names a measurable quantity (reachability rate), a defined population (users in Iran), a triggering condition (government-imposed shutdowns), a data source (Open Observatory of Network Interference probe data), and a time period (2023 to 2025). A reviewer can verify that this condition exists.

A FROM state that fails: "There is a lack of privacy tools for people in repressive contexts." This names a category (lack of privacy tools) and a vague population (people in repressive contexts). Neither is measurable. A reviewer cannot verify whether this condition exists or how severe it is.

**Class D2 failure (values aspiration without conditions).** Some applications offer values language, community commitments, or a mission statement in place of a diagnosis. When asked for a specific FROM state, these applications produce more values language because no diagnostic work preceded the application. They articulate what they are trying to achieve: more privacy, better coordination, greater equity. These are directions, not conditions. Applications of this type cannot produce a plausible FROM state on request because the diagnostic work was not done before the application was written.

This is a structural failure, not a communication failure. Applicants in this situation cannot name the FROM state because they do not know what it is. They began with a desired outcome and worked backward to a scope of work, rather than beginning with a documented problem and working forward to an intervention designed to address it.

**Class D1 failure (canonical vocabulary without structural grounding).** A second type of application passes the gate because it uses technically correct vocabulary and names something resembling a problem diagnosis. The failure appears at the rigor tier: the specific measurable indicators are unsupported, the baseline is undocumented, or the construction methodology cannot be replicated. An application of this type may score 2s and 1s across the indicator rubric after passing the gate.

These two failure types require different responses from a review committee. A D2 failure is a gate failure: the path to resubmission is to do the diagnostic work first. A D1 failure is a rigor-tier failure: the path to resubmission is specific field completion. Treating a D1 failure as a D2 failure misdirects the applicant.

**Application timing is not the diagnostic.** A team that built something before the grant application opened is not automatically exhibiting a gate failure. They can name the FROM state precisely because they built the solution to address it. Application-window activity is a weak corroborating signal about whether work was shaped around funder expectations; it is not a gate criterion.

**Build nested inside change is valid.** Describing what will be built is not a failure in a change-obligation round. What matters is whether the build commitment replaces or sits inside the change specification. Build is validly nested when the applicant can name a FROM state that satisfies the entry gate, and the built thing is the mechanism for addressing that condition. The change specification is intact; the build is the delivery vehicle for the change. Build becomes the failure mode when it has replaced the change specification entirely: the applicant names a deliverable where a problem diagnosis was required, and cannot produce a FROM state because the problem was never diagnosed before the solution was designed. An applicant who began with the problem produces the FROM state naturally, because naming a specific measurable condition in a defined population is the output of having diagnosed it. An applicant who began with the solution cannot, because no problem was named before the solution was conceived.

**Change obligation at different scales.** A small team with a clear diagnosis and a modest claim needs less formal documentation of the FROM state than a large institutional applicant making a broad population-level claim. The Coordination Scaling Standard calibrates this. Both must name a specific measurable condition; the depth of corroboration and the formality of the indicator specification scale upward with the scope of the claim.

---

### 1C: Retroactive Obligation

**What the entry gate is asking.** Does the applicant present evidence of prior contribution meeting the program's published threshold criteria?

Retroactive obligation is not the absence of obligation; it is obligation for what has already happened. The applicant must demonstrate, not assert, that prior contribution occurred. The difference is evidence that an independent reviewer can access and assess without relying on the applicant's self-report.

**What qualifies as evidence of prior contribution.** Evidence that meets the standard is publicly accessible from sources the applicant does not control. On-chain usage data with a named contract address or deployment record. A public code repository with a documented commit history, stars, forks, or downloads. Published documentation that other projects cite. Named organizations or individuals who use the contribution and can confirm that use. Ecosystem metrics from named third-party data providers.

What does not qualify on its own: the applicant's description of their own work, a team bio, or a list of features the applicant says they built. These may be accurate but they are not independently verifiable. They must be accompanied by at least one external source that confirms the contribution is real and in use.

**The prior award disclosure requirement.** Retroactive applications must disclose any prior awards received for the same or substantially overlapping contribution, from this or any other program. This is the concurrent funding disclosure requirement applied to the retroactive context. Receiving multiple retroactive awards for the same contribution is not automatically disqualifying, but it must be disclosed and may be weighted in the rubric assessment. Non-disclosure is a disqualifier.

**The forward commitment option.** Programs may configure a forward commitment as a condition of the retroactive award. If activated, the awardee commits to a named forward action (a specified deliverable, a continuation commitment, a public-access maintenance obligation) as a condition of receiving the award. The forward commitment is assessed under build-obligation criteria: it must name a falsifiable deliverable with verifiable completion criteria. If a program has activated a forward commitment and the applicant's forward commitment fails the build-obligation entry specification, that is a rigor-tier finding, not a gate failure for the retroactive application itself.

**What reviewers are assessing.** The program's published rubric covers the substantive scoring of retroactive applications; it is not the same as the CROSS indicator specification rubric. The CROSS conformance checks (concurrent funding disclosure, adverse signal disclosure, conflict of interest) apply in full. The indicator specification rubric in Section 3 of the assessment rubric applies only if the program has configured indicator-based forward reporting alongside the retroactive award.

---

## Part 2: Gate Architecture

Understanding the gate architecture helps applicants prepare the right evidence at the right time, and helps reviewers know what they are authorized to require.

### The four gates

The entry specification gate determines who enters the round. Its content depends on the mode (Part 1 above). It is always present; what it asks is mode-specific.

Progress verification gates trigger mid-funding disbursements. Each tranche disbursement is contingent on verification of progress against the milestone committed at the prior stage. The minimum acceptable evidence at a progress verification gate is a publicly linkable artifact demonstrating work toward the specified deliverable or indicator. Funders may configure higher evidence requirements. Where no mid-funding disbursement is planned, progress verification gates are not required.

The completion verification gate determines who receives final payment. This gate cannot be informal. The funder must have a published mechanism for determining whether completion criteria have been met. Grantee self-report alone does not satisfy the completion verification gate at any evidence strength level.

For build-obligation rounds: the completion gate must additionally confirm that the specified deliverable is publicly accessible before final payment is released. A deliverable that was produced but is not public does not satisfy a build-obligation completion gate.

For change-obligation rounds: the completion gate requires outcome evidence against the baseline established at entry, assessed by the named mechanism in the infrastructure declaration.

The continuation specification gate covers progression across rounds or stages. It is configured at the program level, not the round level, and it must be published before any round in the program opens. It is the primary mechanism for escalating evidentiary pressure as a project matures.

### What applicants need to know about gate configuration

Before applying to any round, applicants should confirm: which gates are active, what evidence scope and strength is required at each gate, and whether the funder has published an infrastructure declaration for gates at independent review level. The infrastructure declaration names who will review the evidence, their qualifications, and the timeline. If a gate is configured at independent review level and no infrastructure declaration is present, the funder has a conformance obligation to fulfill before the round can proceed.

The gate configuration cannot be retrospectively tightened against applicants who entered the round under a published configuration. A funder may not apply a higher evidence requirement than was published at round opening. A funder may not waive a published requirement without documented rationale submitted to a named authority before the gate is reached.

### Evidence scope and strength

Evidence scope describes what kind of evidence the gate accepts: output evidence (the deliverable exists), usage evidence (the deliverable is being used by external parties), outcome evidence (a measurable change has occurred in the specified population), or impact evidence (a supportable causal link is established between the funded work and the measured change).

Evidence strength describes the verification mechanism: self-report with documentation (grantee narrative reviewed by funder staff), third-party verifiable (publicly accessible from sources outside the applicant's control), independent review (a named party outside the funder-grantee relationship confirms the evidence), or independent evaluation (a qualified evaluator conducts a structured assessment).

Applicants who understand these two dimensions can calibrate their evidence preparation to the gate requirements. A progress verification gate configured at output scope and self-report strength needs a publicly linkable artifact and a brief narrative. A completion verification gate configured at outcome scope and independent review strength needs a structured outcome report with data at the operational definition level and a named reviewer who has agreed to conduct the assessment.

### The served-population risk-bearer floor

The standard names three parties who bear loss when a round's evaluation misjudges: the applicant whose work may be misclassified, the funder whose resources may be misdirected, and the served population, the people a funded intervention is meant to serve. The served population bears loss when the round funds work that does not reach them, or excludes work that would have served them. The standard treats this population as a risk-bearer of the evaluation itself, carried through every gate, not confirmed once at entry and then set aside.

**What the floor requires of a reviewer.** Where a round's eligibility rests on serving a defined population, each gate determination must account for that population's exposure, not only the applicant's claim about it. The entry-gate affected-population validation (Part 9 of this guidance) performs part of this work by confirming the claimed need from outside the applicant's control. The floor extends the same consideration to the completion verification gate. At completion, the reviewer additionally asks two questions: is there work recorded as delivered that does not actually reach the served population, and are there effects on that population that the declared indicators do not capture? The unintended outcomes disclosure is where the second question surfaces.

**How a reviewer confirms the determination record shows the consideration was applied.** This is the test, and it is specific. It is not enough that the served population was named in the application or validated at entry. The determination record at each gate must show that the population's exposure was considered at that gate. A completion determination that records only whether the deliverable exists or whether the indicator moved, with no statement about whether the result reached the served population and no engagement with the unintended outcomes disclosure on that point, has not applied the consideration. A determination that records the reviewer's finding on reach and on uncaptured effects, even a brief finding that no exposure was identified, has applied it. The qualifying difference is a visible consideration in the record, not a named population at entry.

**What the floor does not require.** The floor is a named consideration each gate is checked against. It does not, on its own, require a standing channel through which the served population raises concerns during the grant period. A program may add such a channel as a separate configuration, but a program without one is not non-conformant with the floor. A reviewer assessing floor conformance is checking for the applied consideration in the determination record, not for a participation mechanism.

---

## Part 2-A: Entry-Gate Declarations

Before any gate is assessed, the entry submission must carry a set of declarations. These are pre-conditions for gate assessment, not scored criteria: an entry submission missing a required declaration is incomplete and is not assessed until the declaration is provided. This Part gives the what-qualifies and what-does-not guidance for each declaration the standard requires at entry.

### Organizational identity declaration

Every entry submission, in all three obligation modes, must include an organizational identity declaration with six required fields.

**Legal entity name and jurisdiction.** Qualifies: the name of the natural person or registered organization exactly as it appears in the jurisdiction of registration, plus the jurisdiction itself. Where no legal entity exists, an explicit statement that none exists, naming the individual who assumes personal responsibility for the obligation. Does not qualify: a project name, display name, or code-repository organization name offered in place of the legal name, where these are not themselves the legal name. The test a reviewer applies is whether the named entity could be located in a registry, or, for an unregistered applicant, whether a specific named person stands behind the obligation.

**Parent organization declaration.** Qualifies: a statement of whether the applicant operates under or is affiliated with a larger organization, network, or chapter structure, and where one exists, the parent's name and the relationship (whether the parent knows of this application, shares brand or personnel, and is separately applying to this or a concurrent round). Does not qualify: silence where an affiliation is publicly documented, or where the applicant's name, brand, or personnel overlap with a known larger organization. Silence in that situation is the specific failure this field exists to catch.

**Affiliated entity disclosure.** Qualifies: disclosure of any other organization, project, or entity sharing the applicant's name, brand, domain, key personnel, or codebase, whether or not a formal legal relationship exists. The field is built to surface three things a reviewer should watch for: a new applicant using a name associated with an established organization (name collision), a sub-entity applying separately from a parent that may also apply (internal fragmentation), and team members holding funded roles in other organizations applying to the same round (personnel overlap). Disclosure is not a disqualifier; non-disclosure of a publicly documentable affiliation is.

**Prior round history.** Qualifies: a statement of whether the applicant, or any substantially overlapping entity (same personnel, same codebase, same project name, or same legal entity under a different display name), has applied to this program before, under what name, and with what outcome. Does not qualify: a clean "no prior history" from an entity whose personnel or codebase carry a prior application under another name. This field catches serial rebranding, where an applicant who received a prior rejection returns under a new name claiming no history. Where a prior funder's gate determination exists as a publicly verifiable signed record, the applicant may cite it and the reviewer may query it as independent corroboration, which is stronger than the applicant's own account of the same outcome.

**Disbursement authority.** Qualifies: the named person or persons with legal authority to receive grant funds on behalf of the applying entity and approve their deployment, in one of three declared states. Individual: one named person with full authority. Collective: shared authority through a named mechanism, with current key holders named and the quorum threshold stated. Delegated: authority by role, with the current holder named and the transfer mechanism stated. For a decentralized autonomous organization applicant without a legal wrapper, the declaration must name the controlling wallet address and the decision mechanism, with current token holders above the materiality threshold named where possible. Does not qualify: an entry submission with no disbursement authority declaration, which is incomplete.

**On-chain identity anchor.** Qualifies: the canonical wallet address by which the applying entity is identifiable across blockchain programs and grant databases. For an entity that has applied to or received funding from any blockchain-based grant program, this is the address registered in those programs. For an entity with no prior blockchain grant history, this is the address that will serve as the identity root for this program's records. The anchor is what the funder uses to perform cross-program identity matching and Attestation Corpus queries. It is not a fund-receipt address unless it also serves as the disbursement authority; where the two are the same address, the applicant must state this explicitly. Does not qualify: non-disclosure of an on-chain address publicly associated with the applicant's identity in any grant database. That non-disclosure is a conformance failure equivalent to non-disclosure in the affiliated entity field.

**The funder-side query that pairs with the anchor.** For each application that provides an on-chain identity anchor, the program queries the Attestation Corpus for that address across named public sources (on-chain attestation registries, the KarmaGAP grants and milestone interface, and any program-specific databases the round names) before gate assessment is complete. This is a funder-side procedure, not an applicant submission. Where the query reveals prior grants, milestones, or obligations the applicant did not disclose in the obligation fulfillment record below, that is non-disclosure of a prior obligation and is treated as a material discrepancy.

### Sufficiency architecture declaration

Every entry submission must include a sufficiency architecture declaration alongside the organizational identity declaration. It collects five elements: the four below plus the revenue architecture declaration, which is described in its own subsection.

**Scope declaration.** Qualifies: the specific program, sub-entity, or aspect of the applying entity's work this application covers, stated clearly enough that an independent reviewer could determine what falls inside it and what falls outside. Where the application covers the entity's entire operation, an explicit statement to that effect. Does not qualify: a scope so general the reviewer cannot place a given activity inside or outside it. The scope declaration is what later allows the reviewer to assess additionality and attribute outcomes; an unbounded scope defeats both.

**Sufficiency position.** Qualifies: one of four declared positions at the declared scope. Critical gap: resources cover less than half of full scope requirements and viability depends on closing the gap. Partial: resources cover more than half but the program operates below intended scope. Approaching: resources are sufficient for current operations but not for the next intended scope expansion. Surplus: resources exceed current scope requirements in the current period. The position is declared at the declared scope, not at the entity level; an entity may be approaching on one program and at critical gap on another. Does not qualify: a position declared for the whole entity where the application covers one scope within it.

**The corroborating-evidence requirement on the sufficiency position.** The sufficiency position must carry at least one piece of corroborating evidence from a source outside the applicant's control. Qualifies: publicly accessible treasury data (on-chain balance, Open Collective balance, or equivalent) showing the scale of current resources at the declared scope; grant-history records from a named external database (KarmaGAP, Gitcoin Explorer, retroactive-funding recipient lists, or equivalent) confirming the number and scale of active grants; or disclosed revenue figures from a named independent source. A declaration with no corroboration is accepted at self-report strength only and must be labeled as such. Where the program configures this declaration at independent review strength or above, corroboration is required before assessment proceeds. Where no public corroboration exists (a recently formed entity with no funding history), the applicant must state this explicitly and explain why the declared position is reasonable given the absence. The corroboration need not precisely match the declared position; it provides the factual basis against which the declaration is assessed.

**Portfolio context statement.** Qualifies: an account of how other funding sources in the entity's funding architecture address other scopes or aspects of its work. This is distinct from concurrent funding disclosure, which asks about other funding for the same scope; the portfolio context asks how the entity has organized its pursuit of sufficiency across all its programs. The presence of other funding sources for other scopes is expected and is not a disqualifier. Does not qualify: silence about other funding sources in an entity that plainly runs multiple programs, absent an explicit explanation. Where co-funding is documented in a publicly verifiable coordination record dated before any work begins, that record is independently verifiable evidence of this statement and is stronger than a self-reported account.

**Grant contribution statement.** Qualifies: a statement of the specific gap at the declared scope this grant would close, and what the sufficiency position at that scope would be after the grant's contribution. Does not qualify: a promise about outcomes in place of a statement of where in the sufficiency architecture the grant fits. This is a declaration of fit, not an outcome commitment.

### Revenue architecture declaration

The revenue architecture declaration is the fifth element of the sufficiency architecture declaration and is universal: every applicant declares it regardless of obligation mode.

**What qualifies.** A declaration of one of four revenue architecture types. Grant-only: no commercial revenue model exists, and the declaration confirms this; additionality requires no further delineation. Fee-for-service, commercial, or hybrid: the declaration names the type and activates the additionality delineation requirement, under which the applicant must identify which portion of their work or budget the commercial revenue does not cover, with the grant scoped to that non-commercial portion.

**What does not qualify.** A fee-for-service, commercial, or hybrid applicant who declares the type but does not delineate which portion of the work the commercial revenue leaves uncovered. For these three types the type declaration alone is incomplete; the delineation is the substance. The reason the revenue architecture sits inside the sufficiency architecture declaration rather than standing alone is that the revenue type and the sufficiency position are the two parameters that together determine whether an additionality argument is coherent. A reviewer reads them together.

### Public benefit mechanism and access condition declaration

Where eligibility is assessed against a public goods claim, which is the case in every public goods grant program, the entry submission must include a public benefit mechanism and access condition declaration. This is a pre-condition for assessment alongside the two declarations above. An entry submission that makes a public goods claim in its eligibility section but omits this declaration is incomplete.

**Mechanism type statement.** Qualifies: a statement of which of four mechanism types the public goods claim rests on, using the declared vocabulary. Output production: the benefit is the produced artifact made openly available. Access provision: the benefit is access to a service or resource. Condition change: the benefit is a measured change in a population's condition. Ecosystem shift: the benefit is a contribution to a broader change. Where the program accepts only certain types, the field must say which are accepted and what evidence scope each requires. Does not qualify: a benefit claim that does not name which of the four mechanisms it rests on, since the mechanism type is what binds the evidence scope at completion.

**The mechanism type constrains the completion evidence.** A reviewer should read the declared mechanism as a commitment about the completion gate. Output production commits the applicant to output evidence at minimum. Access provision commits to usage evidence. Condition change commits to outcome evidence. Ecosystem shift commits to a documented impact-contribution argument. A mechanism declared at entry that the available completion-gate evidence cannot support is a misrepresentation in the entry specification, not a late surprise at completion.

**Access condition statement.** Qualifies: the specific terms under which the declared mechanism delivers benefit to the stated population, with the required content set by the mechanism type. For output production: an SPDX license identifier and the location of the license file. For access provision: an access mechanism, a cost structure, and a non-excludability mechanism. For condition change: a FROM state and a population definition. For ecosystem shift: a named causal pathway and a co-factor list. Does not qualify, specifically for output production: a copyright notice that permits free viewing without granting modification or redistribution rights; a "source available" or "fair code" license restricting commercial use, unless the program's published round configuration explicitly accepts such licenses and names the accepted SPDX identifiers; or a future licensing commitment with no current license, which does not satisfy the access condition at entry. The license must be present in the artifact at the time of the completion gate.

**The contradiction a reviewer must surface.** The most common failure pattern is an applicant who describes work produced under standard all-rights-reserved copyright while claiming an output production mechanism. The output production access condition requires an open license; all-rights-reserved is its opposite. This contradiction cannot be resolved by reviewer judgment. It must be surfaced as a discrepancy, and the applicant must address it before assessment proceeds.

### Development stage declaration

The development stage dimension is active in all rounds, so every entry submission includes a development stage declaration.

**What qualifies.** A declared stage number from one to five, the applicant's account of why the work sits at that stage rather than an adjacent one, and at least one piece of evidence from a source outside the applicant's control confirming the stage. The stage-specific evidence the standard expects: Stage 1 (proof of concept) provides output evidence of the existing artifact; Stage 2 (early adoption) provides usage evidence from at least one named external user; Stage 3 (growth) provides independently verifiable adoption data with a trend; Stage 4 (established infrastructure) provides twelve months of sustained usage data from sources outside the team; Stage 5 (retroactive recognition) provides prior contribution evidence in the entry submission.

**What does not qualify, and what a reviewer investigates.** A declared stage not supported by the provided evidence is a material discrepancy requiring investigation, not a passing declaration. Two patterns recur. A Stage 1 declaration paired with usage evidence from independent users is either a misstatement of stage or an understatement the reviewer should probe. A Stage 3 or higher declaration paired with no independently verifiable adoption data is a discrepancy to investigate. The reviewer's task is to check the declared stage against the rest of the entry submission, not to accept the number on its own.

**The stage constrains the obligation mode.** The declared stage limits which obligation modes are coherent. A Stage 1 applicant committing to a change obligation must supply a FROM state and a population baseline at entry; this is coherent only if the Stage 1 artifact is specifically designed to measure against an existing condition. A Stage 4 applicant selecting a build obligation must specify what new functionality is being added beyond sustained operation; declaring Stage 4 with a build obligation for what amounts to continued maintenance of existing function is a framing misrepresentation. Funders declare in the round configuration which stages are within scope; a round accepting all stages must say so explicitly, and a round targeting specific stages must name them and say why others are excluded.

### Continuity and resilience declaration (the Continuity Capacity dimension)

This dimension is triggered by grants above a funder-defined size threshold, grants producing ongoing infrastructure with continuing operational requirements, and any application where the applying entity has a single named primary contributor and no documented backup function. For programs that fund infrastructure maintenance or sustained service delivery, it is always active regardless of threshold.

**What qualifies.** A declaration of one of three resilience states with supporting evidence. Single: continuation depends on one person. Partial: some backup function exists but coverage is incomplete. Resilient: continuation does not depend on any single person. For a single-point declaration, the evidence must name the person on whom continuation depends and state what would happen to active grants and funded deliverables if that person became unavailable.

**What does not qualify, and why disclosure is the point.** A single-point-of-failure declaration is not a disqualifier, so an applicant should not conceal one to pass. What does not qualify is silence where the trigger applies, or a resilient or partial claim with no evidence of the backup function it asserts. The disclosed single-point state is a material fact that affects the sustainability assessment at the continuation gate and the funder's configuration of completion-gate conditions; a funder may configure the completion gate to require evidence of partial or resilient continuity as a condition of final disbursement for grants above the threshold. A reviewer treats the honest single-point disclosure as conformant and the concealed one as the failure.

### Obligation fulfillment record

The obligation fulfillment record is required, before assessment proceeds, where any of three conditions apply: the applicant has received prior grants from this funder in any prior round; the applicant cites prior work as evidence of capability at entry; or the applicant's prior round history includes unresolved KarmaGAP milestones or open gate conditions.

**What qualifies.** For each prior grant from this funder, a record of three things: what was committed at the entry gate of that prior round (the deliverable specification, the FROM-TO state, or the contribution evidence, as fits that round's mode); what was produced during the grant period (the artifact, the measured change, or the verified contribution, with a publicly accessible link); and whether the commitment was fulfilled, partially fulfilled, or unfulfilled, with the applicant's explanation where fulfillment was not complete.

**What does not qualify, and the asymmetry a reviewer should hold.** An unfulfilled prior obligation is not automatically disqualifying. It is a disclosed fact that affects the track-record assessment at the continuation gate and may be addressed by a written account of what prevented fulfillment and what has changed since. What does not qualify is non-disclosure: an unfulfilled prior obligation omitted from the record but discovered through research, including through the Attestation Corpus query, is a material discrepancy. The standard treats the non-disclosure of a prior failure more seriously than the failure itself. A reviewer assesses the disclosed shortfall on its explanation and the undisclosed one as a conformance discrepancy.

### Prior work attribution statement

Where an applicant cites prior work as evidence of capability, track record, or past contribution in any entry submission, a prior work attribution statement is required. It activates in all three modes: build-obligation applicants citing prior deliverables, change-obligation applicants citing prior outcomes as a baseline or established methodology, and retroactive-obligation applicants whose entire submission consists of prior work.

**What qualifies.** For each piece of cited prior work, an answer to three questions. Entity of performance: under which legal entity or organizational context the work was performed; if it was done as an employee, contractor, or contributor to an organization that is not the applying entity, that organization must be named; if it was done under the applying entity's own resources, that must be stated. Applicant's relationship at the time: the applicant's role in the entity under which the work was performed, and the current status of that relationship, with both the relationship at creation and the relationship at application stated. Current ownership and access: who currently holds the intellectual property rights, who controls the deployment or codebase, and who holds the user relationship with any users cited as evidence of impact; if the applying entity does not hold the rights, control the deployment, or hold the user relationship, that must be stated.

**What does not qualify, and why this is an adverse signal field.** The statement is an adverse signal disclosure requirement, not a procedural form. What does not qualify is a track record built on work performed under a different entity, presented as the applicant's own without that entity's knowledge or endorsement of the application. An applicant who cannot truthfully complete the attribution statement for their cited work has surfaced a misrepresentation in the core evidential basis of the application: a claim of responsibility for outcomes the applicant did not control and cannot warrant continuing. A reviewer reads a clean attribution statement as the applicant's own track record, and a contributor-to-another-entity's-work pattern, presented as ownership, as the misrepresentation the field exists to surface.

---

## Part 3: How to Complete Each Indicator Field

CROSS requires applicants to self-specify their outcome indicators. The funder specifies the domain; the applicant specifies what their intervention produces within it. CROSS specifies the fields each indicator must contain and the quality standards those fields must meet.

### Field 1: Indicator name

A short descriptive label. Not the operational definition. Keep names short and move the precision to Field 4. A name that tries to contain the operational definition ("number of users meaningfully engaged with privacy-preserving tools on a sustained basis") is trying to do too much; the qualifier language belongs in Field 4.

### Field 2: Rationale for indicator

Rationale is required. It documents the diagnostic thinking that preceded tool selection. A weak rationale restates the claim without defending the choice ("this indicator measures our core outcome"). A strong rationale names at least one alternative indicator considered and explains why the chosen indicator better matches the intervention's causal claim. The rationale should also note what the indicator does not capture; an applicant who describes the indicator's limitations demonstrates a more mature understanding of the measurement problem than one who describes only its strengths.

### Field 3: Measurement form and evidence classification

This field replaces the constrained four-option data type list from version 0.1.0. Applicants now describe the measurement form in plain language. Reviewers classify the description against three axes for data quality assessment purposes.

**What to write in this field.** Name what a result looks like and in what form it will be reported. Be specific enough that a reviewer can answer three questions: where does the evidence come from (on-chain, off-chain verifiable source, or qualitative/narrative assessment), how is the result expressed (as a number, a position on a scale, a binary yes/no, or a documented condition), and how do period values relate (can they be summed, or does each period describe a status point in time?).

A useful description: "A count of unique wallet addresses per month that completed at least one qualifying transaction on the named contract, sourced from on-chain data via the named block explorer application programming interface. This is a non-cumulative indicator: each month's count reports the status for that month; the life-of-grant target is the count in the final month, not the sum of all months."

A description that requires the reviewer to infer too much: "User engagement metrics." This names a category, not a form.

**Mode-specific notes on measurement form.**

For build-obligation indicators: the form is typically binary (the deliverable either meets the completion criteria or does not) or qualitative (the deliverable is an artifact assessed against named criteria). The description should name what done looks like and how a reviewer would confirm it: "A binary yes/no indicator: either the library is published to the named package registry with the specified version number and passes the automated tests in the public repository, or it is not. Confirmed by the named reviewer checking the registry and the test results."

For change-obligation indicators: the form is typically quantitative or ordinal. Name the unit of measurement and the direction of desirable change: "A quantitative indicator expressed as a count of unique addresses per 30-day window, sourced from on-chain public data. An increasing count indicates progress toward the target."

For retroactive indicators where a forward commitment is configured: apply the build-obligation description guidance to the forward commitment indicator.

**The common error in this field.** Applicants who come from the v0.1.0 format sometimes try to select one of the old four options (number, percentage, yes/no, index). The field no longer works that way. Index and composite indicators require the same plain-language description as any other indicator, with the component specification in the construction methodology field (Field 5) rather than in a sub-table here.

### Field 4: Operational definition

The operational definition specifies what counts and what does not count as one unit of the claimed result. It has four required sub-components.

Inclusion criteria define what qualifies as one instance. Example: "A unique wallet address that completed at least one transaction using the protocol's privacy module during the reporting month, as recorded by the named contract address on Ethereum mainnet."

Exclusion criteria name what the indicator explicitly does not count. Example: "Test transactions from the development team's identified wallet addresses. Transactions on testnet. Transactions using the non-privacy-preserving legacy module." Exclusions matter because without them a reviewer cannot determine whether reported numbers are clean.

Unit of analysis is the named entity being counted: person, household, wallet address, transaction, site, session, message, or other. The unit must be consistent throughout the indicator's life. If the unit changes between reporting periods, the comparability of prior periods must be formally assessed and documented.

Edge case determination is at least one example of how an ambiguous instance is handled. Example: "A wallet address that transacts using both the privacy module and the legacy module in the same reporting month is counted once in the privacy module indicator and once in the legacy module indicator, not twice in either." Edge cases that are not specified in advance produce inconsistent counting criteria across periods. The operational definition is the field that makes cross-funder and cross-period comparability possible.

For build-obligation indicators, the operational definition specifies what completion means at a level of precision that resolves ambiguity: what qualifies as one passing instance of the deliverable, what does not qualify, and how an edge case (a deliverable that meets some but not all criteria) is handled.

### Field 5: Construction and aggregation methodology

The calculation rule in sufficient detail that an independent reviewer with access to the stated data source could replicate the result without contacting the applicant. Three elements are required: the formula or counting rule, how partial data is handled, and how values from sub-units are aggregated to the project level.

An unusable description: "We track user engagement through our analytics platform and report quarterly." A reviewer cannot replicate this. A replicable description: "We query unique visitor counts from Plausible Analytics at the project domain, using the application programming interface endpoint at [named location], with the date range set to the reporting quarter, counting unique visitor fingerprints as defined by Plausible's methodology, excluding traffic from the IP ranges listed in our exclusions table."

For build-obligation indicators: the methodology specifies how completion is determined, who performs the verification, and by what process. "Completion is determined by the named reviewer, who will check that the library is published to the named package registry at the specified version, that the named test suite passes without errors in the public continuous integration log, and that the application programming interface documentation is publicly accessible at the named location. The reviewer will document their finding in a brief written statement submitted to the program within two weeks of the submission deadline."

### Field 6: Cumulative or non-cumulative

A cumulative indicator can be summed across reporting periods. If a project commits to 1,200 unique users over a twelve-month grant and the indicator is cumulative, the target is reached when the running total equals 1,200. Each period adds to the previous total.

A non-cumulative indicator measures a status at a point in time. If a project commits to 500 active monthly users by grant end, the target is the status at grant end, not a sum. Summing a non-cumulative indicator across periods is a data construction error: it would be like adding January's temperature to February's temperature to get the year's total temperature.

Reviewers must flag this designation at the application stage. A project that specifies a non-cumulative indicator but sets a life-of-grant target that can only be reached by summing across periods has a structural inconsistency that, if uncorrected, will produce a reporting dispute at grant end.

### Field 7: Disaggregation

Disaggregation categories specify how the indicator will be reported broken down by subgroup: by geography, by user type, by protocol version, by language, or by other named categories.

The disaggregation ratchet is a one-way constraint: categories committed to in the application may be supplemented in subsequent reporting periods but may not be removed without committee approval and documented rationale. The purpose is to protect longitudinal comparability. Adding a new category enriches the data; removing one degrades it.

When requesting approval to remove a category, the applicant must document the reason and specify how prior-period comparability will be preserved or documented as broken.

### Field 8: Data source and collection method

The named source must be accessible to an independent reviewer. Named on-chain contract addresses, named public application programming interface endpoints, named third-party platforms with documented methodology, named institutional partners, and named survey instruments administered by third parties satisfy this requirement.

Sources that do not satisfy the data quality standard on their own: applicant-controlled dashboards with no external corroboration, internal databases accessible only to the applicant, and self-reported results without a named external verification mechanism. These may be supplementary evidence; an indicator whose sole evidence originates from applicant-controlled systems fails the data quality standard.

Naming the source is not the same as describing the collection method. "Google Analytics" is not a collection method. "Monthly unique visitor count exported from Google Analytics property [named ID] using the standard unique users metric, with bot filtering enabled, covering the date range [specified]" is a collection method.

For build-obligation indicators: the data source for completion verification is the named artifact plus the named verifying party. "The library repository at [named public URL], confirmed by [named reviewer] against the completion criteria listed in the application."

### Field 9: Data cost estimation

An attestation that data collection is operationally feasible within the project budget. Where data collection is free, name the source and confirm access. Where it has a cost, provide an approximate cost and name the budget line that funds it.

An indicator that cannot be collected within the project budget has not been operationalized. It is a commitment the project cannot keep.

### Field 10: Baseline (FROM state)

For change-obligation indicators: the documented state of the problem before the intervention begins. Specific, measurable, and sourced. Specific means a named condition, not a category. Measurable means expressed in the same units as the indicator and target. Sourced means the measurement originated from a named source independent of the applicant.

A sourced baseline: "As of December 2025, 340 unique wallet addresses per month had completed at least one transaction using the protocol's privacy module, based on on-chain data from the named contract address, queried using the specified application programming interface." This names the measurement, the unit, the source, and the time point. A reviewer can verify it independently.

For build-obligation indicators where the coordinating party engagement dimension is activated: the documented current absence or inadequacy of the deliverable, with named evidence of the gap it addresses. A named party outside the applicant's organization who has confirmed the need, or a named existing tool's documented limitation, satisfies this requirement. The applicant's assertion of the gap does not.

For retroactive obligation indicators: the documented state of the contribution at the time the award period begins, with named evidence of use. The prior contribution replaces the pre-intervention baseline; the evidence of use replaces the data source for the baseline value.

### Field 11: Target (TO state)

For change-obligation indicators: the expected state of the indicator at the end of the grant period, expressed in the same units as the baseline and operational definition. For cumulative indicators, a cumulative total. For non-cumulative indicators, a target status at grant end.

A target not grounded in the baseline creates an obligation vacuum. A project claiming a six-fold increase against baseline requires an explanation of the mechanism that produces that growth. Without it, the target is aspirational rather than evidence-grounded.

For build-obligation indicators: the completion criteria the deliverable must meet, expressed with enough specificity that an independent reviewer could determine whether they are met. "A working prototype" fails. "A prototype that executes the three functions specified in the design document, demonstrated in a public recording with no fatal errors, with test results from the specified test suite attached" passes.

For retroactive obligation with a forward commitment: the named action the awardee commits to completing as a condition of the award, expressed with falsifiable completion criteria. Apply the build-obligation guidance to the forward commitment target.

---

## Part 4: Common D1 Indicator Sourcing Failures in Change-Obligation Rounds

Class D1 (canonical vocabulary without structural grounding) passes the entry specification gate and fails at the rigor tier. Three patterns account for most D1 sourcing failures.

**The single-day peak metric.** The indicator is a metric derived from a single-day peak rather than a sustained measurement. An application reports a FROM state of "up to 50,000 users" accessing the network during the largest observed traffic event, as evidence of baseline demand. The "up to" language signals a maximum observation, not a median or average. Reviewers identify this pattern by checking whether the baseline is expressed with a central tendency measure (mean or median) and a variance measure, or only as a peak. A sourced baseline expressed only as a maximum without a distribution is not a reliable baseline for calculating change.

**The reach figure without a collection method.** A reach figure ("we have reached 10,000 people with this information") with no specified collection method. The number is present; the mechanism by which it was determined is absent. A count of newsletter subscribers is not the same as a count of people who read the newsletter. A count of social media impressions is not a count of people. Reviewers identify this pattern by checking Fields 5 and 8 against the reported number.

**The applicant-self-assertion baseline.** The coverage claim or baseline is sourced only from the applicant's own assertions, internal records, or self-reported data without named independent corroboration. A conformant application in this situation names the limitation explicitly, proposes a verification mechanism for future reporting periods, and differentiates what is known from independent sources from what is known only from internal records.

---

## Part 5: Concurrent Funding Disclosure in Practice

### What "related to the scope of this application" means

The disclosure requirement covers all active grants, investments, or revenue sources from the prior 24 months that are related to the scope of the application. "Related" is interpreted broadly: it covers funding that supports the same work, the same product, the same team's function to deliver this work, or the same affected population through an overlapping mechanism.

### What must be disclosed

Venture capital investment in the same product or platform the grant work extends. A grant from another funder for the same work, running concurrently. Revenue from a commercial product that the grant work extends or subsidizes. Token issuance or protocol revenue that funds team operations, where the team's operations overlap with the scope of the grant.

For retroactive applications: all prior awards for the same or substantially overlapping contribution, from this or any other program, in any period.

### Token generation events

Token generation events, whether planned or already executed within the prior 24 months, are required disclosure items alongside grants and investments. A token generation event is any mechanism by which the applying entity or its principals generate, allocate, or vest tokens to themselves, to investors, or to the public in a manner that represents or may represent economic value.

**What qualifies as a token generation event to disclose.** Initial decentralized exchange offerings, token generation events, initial coin offerings, liquidity bootstrapping pool launches, and continuous founder or contributor vesting schedules that release tokens during the disclosure window. A token that has not yet launched but for which a whitepaper, tokenomics document, or allocation schedule already exists is a pending token generation event and must be disclosed. The disclosed amount is the approximate United States dollar value at the time of the event; for a pending event, the planned allocation value based on the most recent publicly stated or implied valuation.

**What does not qualify as an excuse for omission.** The existence of a token, or a planned token, is not a disqualifier, so it should not be concealed to avoid scrutiny. What does not qualify is non-disclosure of a material token event: a reviewer treats it as a concurrent funding omission under the same rules as an undisclosed grant or investment, which is to say a disqualifying conformance failure rather than a remediable paperwork gap. The diagnostic for a reviewer is the same asymmetry that applies to the rest of this Part: the disclosed token event is assessed on its relationship to the grant scope; the discovered-but-undisclosed one is a conformance failure.

### What need not be disclosed

Unrelated work by team members that does not overlap with the grant scope. Personal income from employment unrelated to the grant scope. Prior grants in different program areas with no overlap with the current application's scope or affected population.

### Non-disclosure versus disclosure

Disclosure is not a disqualifier. A project with venture capital backing can receive public goods grant funding if the relationship between commercial financing and the public goods ask is clearly articulated and the grant is specifically scoped to work the commercial funding does not cover.

Non-disclosure is a disqualifier. It is not treated as an error that can be remediated. An applicant who fails to disclose a material concurrent funding relationship, where that relationship is subsequently discovered by reviewers, faces disqualification. The asymmetry is deliberate: non-disclosure is a conformance failure, not a paperwork failure.

---

## Part 5-A: Scope Attribution and Outcome Credit in Practice

### When the additionality declaration is triggered

The additionality declaration is triggered whenever concurrent funding is disclosed under Part VI of the standard. If an applicant discloses any active grants, investments, or revenue sources related to the scope of this application in the prior 24 months, the declaration is required as part of the entry specification. It is not an optional supplement. Failure to submit it when concurrent funding has been disclosed is treated as a gate failure at entry, not as a rigor-tier gap.

The trigger is the disclosure itself, not the funder's subsequent assessment of whether the concurrent funding overlaps materially. An applicant who is uncertain whether a given funding relationship is material to the scope should disclose it and address the scope boundary in the declaration.

### What "scope boundary" means in practice

The scope boundary is the applicant's answer to a specific question: what work, deliverables, or costs does this grant fund that the concurrently disclosed sources do not?

The scope boundary must be specific enough that a reviewer can make a binary determination about any proposed activity: does it fall inside this grant's scope or outside it? A scope boundary that says "this grant funds our research while our commercial revenue funds operations" may or may not be specific enough, depending on whether the research and operations are cleanly separable in practice. A scope boundary that names specific work packages, deliverable stages, geographic scope, or cost categories is more likely to pass review.

Common failures at the scope boundary: naming the concurrent source and the grant without specifying what differs between them; asserting "no overlap" without explaining the mechanism by which overlap is avoided; specifying a boundary at a level of generality (for example, "this grant funds public goods work") that does not allow a reviewer to place any given activity inside or outside the boundary.

For build-obligation applications, the scope boundary specifies which parts of the deliverable or which development stages this grant covers, and which the concurrent source covers. For change-obligation applications, it specifies which portion of the intervention pathway, population segment, geography, or time period is funded by this grant relative to others.

### What attribution fractions are

Attribution fractions are declared percentages that sum to 100 percent across all funders, and where relevant a residual category, that materially contributed to a reported outcome. They appear at the reporting stage, not at application entry, and are required whenever outcome or usage evidence is submitted at a gate configured at usage, outcome, or impact evidence scope.

The fractions are a documentation commitment, not a causal proof claim. The applicant declares what percentage of the reported result they attribute to this funder's support, and names the main factors driving that determination: relative funding amounts, timing of disbursements, specific work packages each funder supported, or other distinctions that are documentable and defensible.

The attribution rationale must accompany the fractions. A declaration without a rationale does not satisfy the field. The rationale should also acknowledge material uncertainties where they exist, including cases where the contribution of each funder cannot be cleanly separated.

### The failure mode: absence, not imprecision

The failure mode the standard is designed to catch is the absence of an attribution position where concurrent funding exists and outcome evidence is submitted. An applicant who submits outcome evidence claiming a result entirely to this funder, while having disclosed concurrent funding from another source for the same scope and period, has failed the attribution requirement whether or not the fractions are precisely calculable.

Imprecision in the fractions is not a failure by itself. If the applicant has made a genuine documented effort to attribute the result across funders and the rationale is present and coherent, modest uncertainty in the percentages does not produce a failing finding. The reviewer's job is to assess whether an attribution position is present and internally coherent with the concurrent funding disclosure and the additionality declaration, not to verify the mathematical accuracy of the percentages.

### How reviewers assess attribution

Reviewers confirm three things. First: is an additionality declaration present? If concurrent funding was disclosed and no declaration was submitted, note the gate failure. Second: is the scope boundary specific enough to adjudicate? A boundary too vague to determine whether a given activity falls inside or outside the grant's scope requires clarification before the entry gate can pass. Third (at reporting stage, not entry): is an outcome credit attribution statement present for any evidence submitted at usage, outcome, or impact scope? If the statement is present, is it internally coherent with the additionality declaration and the indicator specification? If attribution fractions for the same indicator change across reporting periods, is the change documented?

Reviewers do not re-derive the attribution fractions from first principles. They assess internal coherence, not mathematical correctness.

---

## Part 6: Adverse Signal Disclosure in Practice

### What the Adverse-Signal Engagement Principle Core Standard requires in the grant context

The Adverse-Signal Engagement Principle Core Standard requires that applicants surface signals that contradict their self-presentation. In the grant application context: prior rejections from similar programs based on substantive grounds, contradictory technical assessments, and negative due diligence results from other funders, where those signals are material to the current application's claims.

### What counts as an adverse signal

A prior rejection from a program with similar eligibility criteria, where the rejection was based on substantive grounds. If a project was declined because reviewers assessed the FROM state as undiagnosed, and the same application is now being submitted to a different funder, that rejection is an adverse signal that must be disclosed.

A contradictory technical assessment: an independent audit, technical review, or peer assessment that found the project's core claims unsupported, the technology insufficiently mature, or the proposed approach unlikely to achieve the stated outcome.

Negative due diligence from other funders: a documented finding by another funder's evaluation process that surfaced a concern material to the current application.

### What adverse signal disclosure does not require

Adverse signals not material to the current application's claims. A rejection from a program with different eligibility criteria that the project did not qualify for geographically is not material to a substantive evaluation of outcomes. Informal negative opinions from ecosystem participants who have not conducted a formal evaluation are not adverse signals in the Adverse-Signal Engagement Principle Core Standard sense.

### Reviewer obligations

Reviewers who find adverse signals during evaluation must not suppress them. If a reviewer discovers that an applicant was declined by another funder on substantive grounds, that finding must enter the review record. The reverse obligation applies: reviewers must not fabricate or amplify adverse signals beyond what the evidence supports.

---

## Part 7: The Conflict of Interest Reasonable Third Party Standard in Practice

### How to apply the standard to novel relationship types

The conflict of interest framework's checklist covers common relationship types, but the applicable standard is the reasonable third party test, not the checklist. Novel relationship types not on the checklist that meet the standard require the same treatment.

The test: would an informed observer with knowledge of the relevant facts conclude that this person cannot maintain independence and is therefore not capable of exercising objective and impartial judgment on this application?

Two questions apply to novel relationships. First: does this relationship create a financial interest, a loyalty interest, or a reputational interest in the outcome of the evaluation? Second: would a member of the public who understood both the relationship and the evaluation role conclude that the evaluation would be influenced by it?

A relationship that meets the standard even though it is not on the checklist: a reviewer who co-authored a position paper with the applicant's lead researcher six months ago, where that position paper directly supports the theoretical framework the application is built on. The co-authorship is recent, the intellectual alignment is direct, and an informed observer would reasonably conclude the reviewer cannot evaluate the application's theory of change impartially. Tier 2 treatment applies.

A relationship that does not meet the standard: a reviewer who attended the same conference as an applicant principal and exchanged messages in a shared community space. This is Tier 3 (disclosure encouraged) but does not meet the reasonable third party standard for a waiver or recusal requirement absent other factors.

### Tier 1 and Tier 2: the key distinction

Tier 1 relationships are categorical bars. No judgment is required and no waiver is available. If a reviewer holds equity in the applicant organization, that reviewer is out. These categories are defined to eliminate the need for judgment precisely because the relationships they describe are ones where judgment cannot be trusted.

Tier 2 relationships require judgment. Whether a relationship rises to the level of a disqualifying one depends on the nature and recency of the relationship, the degree of financial interest, and whether a reasonable third party would conclude independence is compromised. Tier 2 waivers require written justification submitted before participation, approval from a named authority other than the conflicted party, and documentation in the review record. Disclosure must come before participation, not after.

### Who is the named receiving function in a small grants program

Small grants programs often do not have dedicated conformance staff. The receiving function is whoever receives conflict of interest declarations and processes waiver requests. In a small program, this may be a program lead or a board member who does not participate in application review. The function must be a person, not a process. "Submit to the committee" is not a named receiving function.

If the program is small enough that all available staff have potential conflicts with at least some applications, an external trusted person should serve this function. It is operationally untenable for the person reviewing a conflict of interest declaration to be the same person whose independence is in question.

---

## Part 8: Privacy-Sensitive Context Accommodation

### When the accommodation applies

The privacy-sensitive accommodation applies when standard outcome measurement would compromise the safety of the affected population. The harm must be specific and supportable, not hypothetical. The population must face elevated risk from the act of measurement itself, not merely from the subject matter of the intervention.

The paradigm case: an application for a censorship-circumvention tool serving users in jurisdictions where use of such tools is criminalized. Standard outcome measurement (device identifiers, IP addresses, user accounts) would create a data trail that could be used to identify and prosecute users. The harm from measurement is specific: identification by state actors. The harm is supportable: documented cases of user identification leading to prosecution exist in the relevant jurisdiction.

### What the accommodation requires

First, the applicant must name the specific harm that standard measurement would create. Not a general preference for privacy; a specific, named harm to a specific, named population. "Standard analytics would create identifiable records of users in Iran accessing censorship-circumvention tools, which could be used by Iranian state authorities to prosecute those users under [named legal provision]" is a specific harm statement.

Second, the applicant must name the specific alternative methodology they will use. Acceptable alternatives include Open Observatory of Network Interference-style network measurement (which assesses network conditions without identifying individual users), ethics-reviewed studies conducted by institutional partners under institutional review board protocols, differential privacy techniques applied to aggregate reporting, or other named methodologies with documented privacy properties.

The alternative methodology must be specific enough that a reviewer can evaluate whether it actually addresses the harm named. "We will use privacy-preserving methods" is not an alternative methodology.

### What does not qualify as an accommodation invocation

A general preference for privacy is not a harm statement. Absence of analytics infrastructure is not a harm statement. Discomfort with data collection is not a harm statement. The accommodation exists to protect affected-population members, not to relieve applicants of measurement obligations they find burdensome.

---

## Part 9: Affected-Population Validation

### What "validated by parties outside the applicant's control" means

For change-obligation rounds: the FROM state must be confirmed as real by sources the applicant did not produce and does not control. This has two components. The baseline measurement must come from a named independent source. The existence of the problem must be corroborated by evidence the applicant did not generate.

"Validated by parties outside the applicant's control" means that at least one of the following is true: the baseline data comes from a named independent data source (Open Observatory of Network Interference, a government statistical agency, a peer-reviewed study, a third-party audit), or the problem is documented in a named source (journalism, non-governmental organization reports, independent technical analyses) that the applicant did not produce and does not control.

An applicant who cites only their own assessments, their own user feedback, and their own network as evidence that the problem exists has not demonstrated affected-population validation. They have demonstrated that they believe the problem exists.

For build-obligation rounds where the coordinating party engagement dimension is activated: the claimed need for the deliverable must be validated by at least one party outside the applicant's organization who would use or benefit from it. A named person or organization who has expressed a specific need for this deliverable satisfies the requirement. A general claim that the ecosystem needs better tooling does not.

### The alternative-tool check

For change-obligation rounds: applicants who cannot name existing alternatives to their proposed solution for the stated affected population have not diagnosed a problem; they have proposed a solution in search of one. The check does not ask applicants to demonstrate that no competition exists; it asks them to demonstrate awareness of the landscape and to explain why existing approaches are insufficient for the stated population.

An applicant who names existing alternatives and explains specifically why those alternatives do not serve the stated population under the stated conditions has completed the affected-population validation exercise. An applicant who asserts that nothing comparable exists without evidence of having looked has not. When existing tools address the stated FROM state for the stated population, the applicant must explain what additional value their intervention provides.

---

## Part 10: On-Chain Execution and Verification Instruments

### When this section applies

The on-chain execution and verification instruments subsection of Part V applies when the primary deliverable is a smart contract, a protocol, or an on-chain system, and the obligation object is the contract's behavior under specified conditions rather than a count of discrete outputs or a narrative artifact. In these cases, "did the deliverable meet its completion criteria" is answered by behavioral verification, not by checking that a file was published or that a number reached a target.

The key diagnostic: is the thing being funded a system whose correctness is a property of how it behaves, not just a property of whether it exists? A library that is published and documented is assessed against output evidence. A vault contract that is required to conserve balances under any sequence of deposits and withdrawals is assessed against behavioral properties. The second case triggers this section.

Not every on-chain project falls into this category. A project that happens to involve a contract but whose primary obligation is a count of users or a published report is assessed under the standard measurement form fields. This section is for projects where the obligation object is the contract itself, and where the completion criteria cannot be expressed as a discrete count or a binary file-exists check.

### What each required field means

**Invariant specification.** An invariant is a property the contract must always satisfy or never violate, regardless of who interacts with it or in what order. The invariant specification is a human-readable statement of those properties written at a level of precision that a technically competent reviewer who did not write the contract can understand. It is the counterpart of the formal specification used in verification tools, written in prose.

Examples of adequate invariant statements: "The contract must never release more tokens than were deposited, across any sequence of deposit and withdrawal operations by any number of users." "The protocol fee must not exceed the declared maximum rate for any transaction, regardless of order size." "The proposal execution function must not execute without the required number of valid signatures, as specified in the deployment parameters."

An inadequate invariant statement: "The contract is secure." This is a direction, not an invariant. It cannot be checked and cannot fail.

**Verification method.** This field names how conformance with the stated invariants will be demonstrated. The applicant selects one or more approaches and names the tool, firm, or framework: formal verification using a named model checker or theorem prover, independent security audit by a named firm or type of firm, on-chain invariant monitoring via a named watchdog contract or monitoring service, or manual review of named canonical transaction patterns from public chain data. The verification method must be one that a reviewer outside the applicant's organization can access or reproduce. "We ran internal tests" is not a verification method for this field.

**Verification artifact.** This is the concrete deliverable that constitutes completion evidence. It is the thing the reviewer examines to confirm that the verification method was applied and that the invariants were satisfied. Three types satisfy the requirement: a public proof artifact produced by a named formal verification tool (accessible from a public repository or publication), an audit report from a named independent firm (published publicly or submitted to the funder with confirmation of the firm's independence), or a named contract address and a named query that an independent reviewer can execute from public chain data to reproduce the behavioral check.

The verification artifact must be independently accessible. A document that the applicant holds and has not published, or a test suite that only the applicant can run, does not satisfy this field.

**Failure surface.** At least one example of behavior that would indicate the invariant was violated, stated specifically enough that an observer monitoring the contract could recognize the failure. "If a deposit of X tokens followed by a withdrawal of X tokens results in a net token balance decrease for the depositor with no fees charged, the balance-conservation invariant has been violated" is a failure surface. "The contract fails" is not.

The failure surface serves two purposes. It demonstrates that the applicant has thought concretely about failure modes, which is a signal of adequate specification. And it gives the verification instrument a concrete behavioral check to run, rather than an abstract property to assess.

### Common mistakes

The most common mistake is naming a test suite the applicant controls as the sole verification instrument. A test suite run by the same team that wrote the contract and benefits from a passing result does not satisfy the data quality standard, because the reviewer cannot independently confirm the result. Test suites may appear as supplementary evidence alongside an independent verification instrument. They do not replace one.

A second common mistake is confusing the invariant specification with a description of what the contract does. What the contract does is its functionality. What the contract must always do or never do regardless of conditions is its invariants. A contract's purpose is to allow users to deposit and withdraw tokens; that is its functionality. Its invariant is that any sequence of deposits and withdrawals must leave the user no worse off than the stated fee schedule allows; that is what must be verified.

A third mistake is specifying a verification method that produces a private artifact. An audit conducted by a named firm but with the report held confidential by the applicant does not satisfy this section. The artifact must be accessible to a reviewer who did not commission it.

---

## Part 11: Funder Obligations and Redress in Practice

### The internal clarification mechanism and the structured appeals procedure

These are two distinct instruments that serve different purposes. Applicants and grantees sometimes conflate them; the distinction matters because the appropriate remedy depends on which problem is present.

The internal clarification mechanism is available first, and it is not a quasi-judicial proceeding. It is a structured way for an applicant or grantee to obtain a written explanation of how a specific gate decision was consistent with the published gate configuration, the applicable rubric, and the evidence on record. An applicant who received a completion failure and wants to understand how the funder applied the published criteria to their submission uses the clarification mechanism. The funder's obligation is to respond in writing within a named time bound, with an explanation anchored to the published configuration. The clarification mechanism does not have the authority to reverse decisions; it produces a record.

The structured appeals procedure is available for procedural non-conformance claims: claims that the funder did not follow its own published gate configuration, infrastructure declaration, or conflict of interest framework in a way that materially affected the applicant or grantee. An applicant who believes the funder changed its gate criteria between application and decision without published justification, or that a conflicted reviewer participated in the decision, uses the appeals procedure. The appeals body assesses whether the funder followed the process it published, not whether the substantive scoring was correct.

### What "funder obligation violation" means

A funder obligation violation is a specific condition: the funder did not follow its own published gate configuration or infrastructure declaration in a way that materially affected an applicant or grantee. The violation has two components that must both be present.

First, the deviation must be from the published configuration, not from an informal expectation. If the funder's published gate configuration does not require independent review at the completion gate, a decision made without independent review is not a violation of the published configuration. If the published configuration requires independent review and the funder waived it without documented justification, that is a deviation that may constitute a violation.

Second, the deviation must have materially affected the applicant or grantee. A procedural irregularity that did not change the outcome and did not affect the applicant's ability to prepare is not a violation in the redress sense, even if it was sloppy practice. Material effect means the applicant or grantee was disadvantaged in a way that a conformant process would not have produced.

Non-conformance at the program or infrastructure level (for example, failure to maintain a round configuration record) creates a conformance obligation for the funder but does not automatically give rise to an individual claim unless the failure materially affected a specific applicant or grantee.

### What is and is not appealable

Appeals under Part XI assess procedural grounds only. They address whether the funder followed the process it published. They do not reopen substantive scoring: a reviewer's assessment that an applicant's FROM state was not sufficiently specific is a substantive judgment that the appeals body does not second-guess, unless the applicant can show that the review was conducted by a person with an undisclosed conflict of interest, or that the published rubric criteria were not the ones actually applied.

Appealable: the funder applied gate criteria that differ from what was published at round opening. The infrastructure declaration named a specific reviewer, and a different reviewer was used without documented justification. A conflict of interest violation occurred and was not remediated. The time window for a gate decision was materially shorter than published, and the applicant lost an opportunity to respond.

Not appealable: a reviewer scored an indicator field differently than the applicant expected. The funder's overall program priorities shifted between rounds. A decision the applicant disagrees with on the merits but that was made following the published process.

### Practical guidance on redress body structure

Programs at Stage 1 of their development, or below a funder-defined threshold for program scale, may designate a single board member or an external advisor who did not participate in the original decision as the appeals body. The requirement is structural separation from the original decision-making panel, not organizational independence from the funder. A co-director who reviewed no applications in the round and has no conflict with the appellant satisfies this requirement.

Programs at Stage 2 or above in their Grant Configurator progression should consider whether a single board member or advisor provides adequate structural separation given the volume and complexity of decisions being appealed. At this scale, the program may benefit from a standing advisory panel or a named external arbitrator. The independent redress mechanism referenced in Part XI of the standard is a more formal version of this for large-scale programs. It is optional under the standard but serves a function that becomes harder to discharge through informal channels as programs grow.

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.3.1 | 2026-06-08 | Frame Language own-voice pass. Own-voice watchlist terms replaced with the structural act each names (the govern family became covers or applies to; accountability became obligation or verification; mandatory became required; the integrity standard became the data quality standard; credible became supportable; the Governing standard became the Applicable standard). Part 9 heading Beneficiary Validation became Affected-Population Validation and own-voice beneficiary population became affected population; backup capacity was read as backup function where it named a delivery capability. Framework names and citations preserved. Em-dash sweep clean. No guidance content or requirement changed; vocabulary and naming only. |
| 0.3.0 | 2026-06-05 | Synced to the 0.5.0 standard. Added Part 2-A (Entry-Gate Declarations) with what-qualifies and what-does-not guidance for the organizational identity declaration's six fields including the on-chain identity anchor, the sufficiency architecture declaration's five elements including revenue architecture, the public benefit mechanism and access condition declaration, the development stage declaration, the governance and continuity resilience declaration, the obligation fulfillment record, and the prior work attribution statement. Added the served-population risk-bearer floor guidance to Part 2, with the reviewer test for confirming the determination record shows the consideration was applied. Added token generation event disclosure guidance to Part 5. Added a CRAFT-inheritance note to the introduction. No existing guidance restructured. |
| 0.2.0 | 2026-05-14 | Companion guidance covering three obligation modes (build, change, retroactive), the four-gate architecture, and the eleven indicator fields, with mode-specific notes. Superseded version 0.1.0. |
