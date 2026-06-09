---
title: Gitcoin Grants CROSS+WALKRI Compatibility Statement
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
conforms_to: cross-walkri/primitives-foundation@0.1.6
source_framework: Gitcoin Grants (2025 strategy onward)
source_framework_authority: Gitcoin Foundation
references:
  - Gitcoin Foundation. "Gitcoin Grants 2025 Strategy." gitcoin.co/blog/gitcoin-grants-2025-strategy
  - Gitcoin Foundation. "Quadratic Funding." gitcoin.co/mechanisms/quadratic-funding
  - Gitcoin Foundation. "Grants Program." gitcoin.co/program
  - Gitcoin Foundation. "Gitcoin Grants 24." gitcoin.co/campaigns/gitcoin-grants-24-gg24
  - Gitcoin Foundation. "GG23 Predictive Funding Challenge Retrospective." gitcoin.co/case-studies/gg23-predictive-funding-challenge-retrospective
  - Gitcoin Foundation. Quadratic Funding open-source implementation. github.com/gitcoinco/quadratic-funding
lens_tags:
  calibration_tier: Tier 2 (Process Conformant) aggregate, with Tier 1 (Impressionistic) at the eligibility review layer, Tier 2 at the Quadratic Funding mechanism layer, and Tier 3 (Outcome Specified, Self-Reported) at the metrics-based retroactive layer for mature projects
  authority_source: Voluntary Published
  cultural_methodological_lineage: Western institutional with academic-economics hybrid (mechanism design lineage)
  funder_typology: DAO or protocol (Gitcoin Foundation)
  framework_scope_type: Allocator process framework (primary), with grantee outcome measurement framework characteristics (secondary) for the metrics-based retroactive layer
---

# Gitcoin Grants - CROSS+WALKRI Compatibility Statement

## Summary

Gitcoin Grants is the Gitcoin Foundation's mechanism for distributing matching funds to open-source software, public goods, and community initiatives via Quadratic Funding. The 2025 strategy introduced a layered architecture: Quadratic Funding for early-stage projects, metrics-based retroactive funding for mature high-impact initiatives, and Community Rounds with smaller per-round funding pools. The Quadratic Funding mechanism is the structurally distinctive element: matching allocations are determined by the breadth of contributor participation rather than the size of contributions, making Gitcoin Grants a participation-weighted allocator process rather than a committee-driven evaluation framework.

CROSS+WALKRI compatibility is strongest at the pre-commitment layer (matching pool sizes, eligibility rules, and the formula itself are pre-published per round), at the Determination Body Separation layer (the community is the determination body via QF, structurally outside the applying projects), and at the Independent Verifiability layer (Gitcoin Passport and COCM source signals from outside the applicant's control). Compatibility gaps appear at the eligibility review layer (Gitcoin team review against unpublished rubric specifics is Tier 1 impressionistic) and at the Affected Population Verification layer (downstream users of funded public goods do not directly participate in matching).

This statement covers Gitcoin Grants 2025 strategy onward (GG24, GG25, and Community Rounds); earlier rounds operated under the same QF core mechanism but with a less developed retroactive-funding layer and less robust Sybil resistance.

## The Gitcoin Grants Framework

### Program Structure

The 2025 Gitcoin Grants strategy is explicit about Open Source Software as the cornerstone of the program. The Foundation announces plans to "distribute over **$4.29M** across three major OSS rounds" with the OSS rounds carrying both Quadratic Funding for early-stage projects and metrics-based retroactive funding for mature projects.

Two round formats operate concurrently: major OSS rounds (the primary funding distribution mechanism) and Community Rounds. The Foundation states: "Each Community Round will have a funding pool of **$130K per round**" with a "council" using "**Grant Ships**, a competitive allocation model on Allo Protocol, to vote and review transparently while tracking metrics onchain."

The Foundation also names structural innovations for 2025: "**Dynamic Quadratic Funding** will adjust eligibility and caps, benefiting emerging builders." Round-specific rules are subject to community ratification: "each round will be ratified through governance ahead of time."

### Quadratic Funding Mechanism

Quadratic Funding (QF) is the core allocation mechanism. The Foundation describes the formula in plain terms: "For each project, the square root of every individual contribution is summed, and that sum is squared." The structural consequence is that participation breadth outweighs contribution size: "Funding outcomes are determined by the number of contributors rather than the size of individual donations, prioritizing broad participation over concentrated spending."

The Foundation summarizes the participation rule: "Each donation can be any size; identity verification or sybil resistance mechanisms ensure that each contribution represents a unique human participant."

A reference implementation of the QF mechanism is published as an open-source library at `github.com/gitcoinco/quadratic-funding`. This makes the mechanism independently verifiable: any party can audit the math against the documented formula.

### Sybil Resistance Architecture

Identity verification is structurally essential for QF integrity. The Foundation describes the layered approach: "Identity verification or sybil resistance mechanisms ensure that each contribution represents a unique human participant." Post-round adjustments combine multiple signals: "Gitcoin Passport scoring, Connection-Oriented Cluster Matching (COCM), and pairwise coordination analysis may reduce, reallocate, or otherwise adjust final allocations."

Gitcoin Passport is described as a system that "aggregates verifiable identity signals to support Sybil resistance. Rounds can require minimum scores for eligibility or use attestation data to weight matching outcomes via Connection-Oriented Cluster Matching (COCM)."

### Project Eligibility and Review

Projects must satisfy eligibility criteria specific to each round before entering the QF allocation pool. The Foundation states: "Grantees can apply to a specific round or in some cases, multiple rounds, where they meet the eligibility criteria before going through an onboarding process. Once the application period has closed, the team carefully reviews each one."

The specific evaluation criteria the Gitcoin team applies are not publicly detailed at the published-rubric level. The Foundation indicates: "Projects are evaluated based on their impact, community engagement, and technical feasibility, ensuring that donations go to deserving initiatives that are making a real difference."

GG24 introduced a focus shift: "from participation metrics (number of projects, donors) to impact metrics specific to each domain's problem area."

### Outcomes To Date

Aggregate outcomes reported by the Foundation: "3,715 projects funded; 3.8M unique donations; $50M+ distributed toward public goods." These aggregates are summary metrics across all Gitcoin Grants rounds since program inception, not per-round figures.

## How CROSS Satisfies the Obligation Architecture Gitcoin Grants Operates Under

### Mixed Obligation Mode

Gitcoin Grants 2025 operates in two CROSS obligation modes concurrently. The QF mechanism applies primarily to forward-looking funding of early-stage projects (Build obligation: producing artifacts, infrastructure, or public goods; or Change obligation: shifting conditions in a defined population), while metrics-based retroactive funding for mature projects operates in CROSS's Retroactive obligation mode (Part III Section C).

A CROSS-conformant Gitcoin Grants round would declare the obligation mode at the round level. The QF rounds for early-stage OSS are Build mode (the obligation object is the produced output: code, documentation, infrastructure). The retroactive rounds for mature projects are Retroactive mode (the obligation object is prior contribution assessed against published criteria).

### Pre-commitment (Falsifiability Operationalization)

The QF formula, the matching pool size, the round timeline, and the eligibility rules are all published before contribution begins. This is pre-commitment as structural posture: criteria are fixed before the round runs, evidence (contribution patterns) is assessed against the fixed criteria after. The QF formula itself is mathematically pre-committed; no committee deliberates over its parameters mid-round.

This is structurally stronger than RetroPGF's Season 7 architecture (where algorithms are selected by vote during the round). Gitcoin Grants pre-commits the entire allocation function at round configuration.

### Determination Body Separation (Layer 4 Primitive)

The Determination Body Separation primitive specifies that the body making the funding determination must be structurally distinct from the body receiving funding. Gitcoin Grants satisfies this primitive in an unusual way: the determination body is the community itself, operating through the QF formula. Each contributor participates in the determination by donating; no project can self-determine its own allocation because the formula weights breadth over size.

The Gitcoin team operates an eligibility gate upstream of the QF determination (deciding which projects enter the pool), and this gate is staffed by a body structurally distinct from applicants. However, the specific rubric the team applies is not publicly detailed at the level CROSS Part VIII requires.

A CROSS-conformant Gitcoin Grants would publish the eligibility review rubric explicitly: what criteria the team applies, what disqualifies a project, what evidence the team weighs.

### Attestation Corpus Alignment

The CROSS+WALKRI Attestation Corpus primitive (Layer 4) specifies a queryable record of contribution and use evidence. Gitcoin Grants assembles a de facto Attestation Corpus through Gitcoin Passport (aggregating verifiable identity signals across multiple platforms), the open-source QF implementation (auditable allocation logic), and Allo Protocol (on-chain tracking of round operation and disbursement). These sources constitute queryable, dated, independently maintained records.

A CROSS-conformant Gitcoin Grants would formalize the Attestation Corpus specification at the round configuration level, naming the Passport version, the COCM parameters, and the Allo Protocol contract addresses each round operates against.

### Format Agnosticism (Commitment 5)

Gitcoin Grants satisfies Format Agnosticism strongly. Projects participating in QF rounds are not required to adopt any particular reporting format; their inclusion is mediated by donor participation, which the QF formula counts independent of project-side format choices. Each round's eligibility rules specify content requirements; format prescription is otherwise absent.

### Independent Verifiability (Commitment 6)

The QF mechanism's conformance with Independent Verifiability is split:

**Strong alignment at the allocation layer.** The QF formula is open-source. Allocations can be recomputed by any party with access to the contribution data. The Foundation's open-source implementation at `github.com/gitcoinco/quadratic-funding` makes this auditable.

**Strong alignment at the Sybil resistance layer.** Gitcoin Passport aggregates signals from sources outside the applicant's control (verified accounts on external platforms, on-chain activity, attestations from third parties). COCM applies coordination analysis to detect non-genuine participation. The signals lie outside any project's control.

**Partial alignment at the eligibility review layer.** The Gitcoin team's review of projects against impact, community engagement, and technical feasibility produces a determination that is not independently re-derivable; the underlying rubric specifics are not publicly published at the level the commitment requires.

## How WALKRI Complements Gitcoin Grants

### Evidence Form Specification

WALKRI's evidence form specification requires that every measurement instrument include a documented data source and an independently accessible access path. For QF allocations, the evidence forms are: contribution records (on-chain, Allo Protocol), Sybil resistance scores (Gitcoin Passport), and COCM coordination signals. Each has a queryable access path.

A WALKRI-conformant Gitcoin Grants round publishes for each measurement instrument: criterion intent (what the signal indicates), operational definition (exactly what counts), response form (how the value is calculated), evidence form (where the data is sourced and how to access it), and conformance threshold (the minimum the signal must meet to count). For the QF formula itself, all five are structurally satisfied through the open-source implementation; for the eligibility review and the metrics-based retroactive funding layer, the specifications are less explicit.

### Adverse Signal Engagement Principle

The Adverse-Signal Engagement Principle Core Standard requires that adverse signals be surfaced rather than suppressed. Sybil resistance in Gitcoin Grants is structurally aligned with this principle: the Foundation publishes information about Sybil detection methods, COCM operation, and how post-round adjustments may "reduce, reallocate, or otherwise adjust final allocations." When Sybil patterns are detected, the response is documented rather than concealed.

The GG23 Predictive Funding Challenge Retrospective is a model of adverse-signal-conformant practice at the round level: the Foundation publishes a retrospective document examining what worked and what did not in that round.

A CROSS-conformant Gitcoin Grants would publish per-round adverse signal logs naming the Sybil and coordination concerns identified and the response taken.

### Beneficiary Validation Mechanism (Layer 3 Primitive)

The Beneficiary Validation Mechanism primitive specifies that the FROM state, population definition, or need claim of an applying entity must be independently validated by parties drawn from or accountable to the affected population at the entry specification gate. Gitcoin Grants partially satisfies this through Quadratic Funding itself: donor participation can be interpreted as a form of population validation (the community signals which projects it values).

However, the formal Beneficiary Validation Mechanism is stronger than QF participation. It requires that named parties from the affected population assess the applying entity's characterization of the population, the need, and the FROM state. In QF, donors signal preference but do not formally assess the entity's characterization. The gap is structural: QF measures revealed preference, not deliberative validation.

A CROSS-conformant Gitcoin Grants for change-obligation rounds would add a structured beneficiary validation step at the eligibility gate, particularly for population-targeted public goods grants.

### Affected Population Verification Gate (Layer 4 Primitive)

The Affected Population Verification Gate operates at completion: the affected population participates in verifying what was delivered. Gitcoin Grants' structure does not include direct affected-population engagement at completion: the affected population of funded public goods is typically distributed users (developers using OSS libraries; communities using infrastructure) and they do not participate in the verification of round outcomes.

This is a structural feature of the public-goods QF model. Quadratic Funding allocates based on contributor signal at entry, not on affected-population verification at completion. The completion-side architecture is light: Allo Protocol tracks disbursement; no formal completion gate verifies that funded projects delivered what they proposed.

A CROSS-conformant Gitcoin Grants would add a completion gate with documented downstream-user or affected-population verification, particularly for the metrics-based retroactive funding layer where outcomes are claimed.

## Compatibility Findings

### Strong alignments

- Pre-commitment as structural posture (QF formula, matching pool, eligibility published before contribution begins)
- Determination Body Separation at the allocation layer (community via QF is structurally outside applicants)
- Attestation Corpus structurally present via Gitcoin Passport, Allo Protocol, and the open-source QF implementation
- Format Agnosticism satisfied (no format prescription beyond eligibility requirements)
- Independent Verifiability at the allocation layer (open-source formula, recomputable from public data)
- Adverse Signal Engagement structurally aligned via Sybil resistance and retrospective publication

### Partial alignments

- Independent Verifiability at the eligibility review layer (the specific rubric is not publicly published at CROSS Part VIII granularity)
- Beneficiary Validation Mechanism approximated through QF participation but not formally satisfied (revealed preference, not deliberative validation)

### Compatibility gaps requiring program adjustment for full conformance

- Eligibility review rubric should be published (what criteria the Gitcoin team applies, what disqualifies a project)
- Completion gate absent: no formal verification that funded projects delivered what they proposed
- Affected Population Verification Gate not implemented at completion (consistent with QF model, but unnamed as a boundary)
- Concurrent funding disclosure should be added to project profiles at CROSS Part II Dimension 4 specificity
- Adverse signal logs should be published per round in a standing format

### Structural compatibilities of historical interest

Gitcoin Grants and Optimism RetroPGF occupy adjacent positions in the web3 allocator-process space. RetroPGF Season 7 evaluates contributions retroactively using algorithmic metrics with vote-selected weights; Gitcoin Grants evaluates contributions prospectively through community participation under a pre-committed formula. The two together represent two distinct lineages of web3 grants design: ex-post metric-driven (RetroPGF) and ex-ante participation-driven (Gitcoin Grants). CROSS+WALKRI maps both, with different compatibility profiles.

## Calibration Tier Assessment

Gitcoin Grants 2025 sits at a mixed calibration tier in the CROSS+WALKRI Lenses Framework:

- **Tier 2 (Process Conformant)** at the QF mechanism layer: pre-published formula, pre-published matching pool, pre-published eligibility rules; the program conforms to its own published process
- **Tier 1 (Impressionistic)** at the eligibility review layer: published process exists but specific evaluation criteria are not detailed at the published-rubric level
- **Tier 3 (Outcome Specified, Self-Reported)** at the metrics-based retroactive funding layer for mature projects (limited to the OSS rounds with that component)

Aggregating, the program operates at Tier 2 (Process Conformant) overall, with elements at Tier 1 and Tier 3.

**Current+target trajectory:**

- Current: Tier 2 aggregate as described above
- Next achievable target (next strategic cycle, within current architecture): Tier 3 via publication of the eligibility review rubric and structured completion gate evidence
- Long-range target (within 2-3 years if pursued): Tier 4 (Independently Verified) via independent verification of completion outcomes for mature funded projects and formal Beneficiary Validation Mechanism at the eligibility stage

## Mapping Table

| Gitcoin Grants Element | CROSS Provision | WALKRI Provision |
| :-- | :-- | :-- |
| Pre-published QF formula | Entry specification gate (criteria fixed before applications) | Pre-publication field requirements |
| Matching pool size published per round | Entry specification gate budget publication discipline | Conformance threshold publication |
| Open-source QF implementation | Independent Verifiability (Commitment 6) | Evidence form documentation (formula is the evidence form for allocation) |
| Gitcoin Passport identity verification | Independent Verifiability at the Sybil resistance layer | Integrity standard (5.2): evidence independent of applicant |
| COCM coordination analysis | Adverse Signal Engagement Principle | Integrity standard applied to coordination signals |
| Allo Protocol on-chain tracking | Attestation Corpus structurally present | Evidence form with on-chain access path |
| Eligibility review by Gitcoin team | Determination Body Separation (eligibility gate) | Partial: rubric specifics not public at CROSS Part VIII granularity |
| Community participation as allocator | Determination Body Separation at allocation layer (community is determinator) | Not applicable at the field level |
| Metrics-based retroactive funding (mature projects) | Retroactive obligation mode (Part III Section C) | Outcome evidence requirements for completion |
| No completion gate verification | Gap: completion gate absent | Gap: completion-side evidence forms absent |

## Pre-Funding Specification Layer

A CROSS+WALKRI-conformant Gitcoin Grants round produces something the current framework approximates but does not formalize: a pre-funding specification layer that explicitly publishes (per round) the eligibility rubric, the Sybil resistance configuration, the COCM parameters, the matching cap structure, and the Adverse Signal Engagement plan. The QF mechanism is already pre-committed; the surrounding configuration layer would join it under the same pre-commitment discipline.

## Compatibility Statement Maturity

This is a Tier 2 compatibility statement under the CROSS+WALKRI primitives framework index: the source framework is a structurally novel exemplar of participation-weighted allocation as a retroactive-funding-adjacent mechanism, with a distinct mechanism-design lineage (academic economics derived) layered on the Western institutional grants tradition. It warrants a full statement.

The statement will be revised as Gitcoin Grants 2025 rounds report (GG24, GG25, Community Rounds) and as the metrics-based retroactive funding layer for mature projects matures.

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

Gitcoin Grants Program: gitcoin.co/program

Gitcoin Foundation Blog: gitcoin.co/blog

Open-source Quadratic Funding implementation: github.com/gitcoinco/quadratic-funding

License: CC0

## Changelog

- **0.1.2 (2026-06-08):** Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only.
- **0.1.1 (2026-05-23):** Primitive rename cascade applied. References to the Layer 4 primitive renamed from "Beneficiary Accountability Gate" to "Affected Population Verification Gate"; the gate's role and Gitcoin's structural gap remain unchanged. The "Beneficiary Validation Mechanism" (Layer 3, entry-gate primitive) retains its name and is unaffected. Descriptive references to "beneficiaries" of funded public goods rephrased where they discussed the renamed primitive's operation; references that describe Gitcoin's public-goods context (downstream users of OSS libraries and infrastructure) are unchanged.
- **0.1.0 (2026-05-23):** Initial compatibility statement covering Gitcoin Grants 2025 strategy onward. Maps Quadratic Funding mechanism, Sybil resistance architecture (Gitcoin Passport, COCM), Allo Protocol tracking, and mixed obligation mode (forward QF for early-stage, retroactive for mature). Identifies strong alignments at the allocation layer (pre-commitment, Determination Body Separation, Independent Verifiability, Format Agnosticism, Adverse Signal Engagement) and gaps at the eligibility review layer (rubric not publicly detailed at CROSS Part VIII granularity) and the completion verification layer (no formal completion gate). Lens-tagged: Tier 2 aggregate with Tier 1 eligibility review and Tier 3 retroactive layer; Voluntary Published authority; Western institutional with academic-economics hybrid lineage; DAO or protocol funder typology; Allocator process primary scope.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri. For the source framework, see gitcoin.co.*
