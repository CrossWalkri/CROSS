---
title: Optimism Retro Funding CROSS+WALKRI Compatibility Statement
version: 0.2.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
conforms_to: cross-walkri/primitives-foundation@0.1.6
supersedes: Optimism-Retro-Funding-CROSS-WALKRI-compatibility-0_1_0.md (v0.1.0, 2026-05-18)
companion: Optimism-Retro-Funding-Impact-Evaluation-CROSS-WALKRI-compatibility-0_1_0.md
source_framework: Optimism Retro Funding (Season 7, 2025 onward)
source_framework_authority: Optimism Foundation, Optimism Collective Citizens House
references:
  - Optimism Foundation. "Retro Funding 2025." optimism.io/blog/retro-funding-2025
  - Open Source Observer. "Unpacking the evaluation algorithms behind Optimism's latest funding round." docs.oso.xyz/blog/retro-funding-s7-release
  - Optimism Governance Forum. "Optimism Retro Funding Voting Design Evaluation." gov.optimism.io/t/optimism-retro-funding-voting-design-evaluation/8872
  - Optimism Collective Operating Manual. github.com/ethereum-optimism/OPerating-manual
lens_tags:
  calibration_tier: Tier 3 (Outcome Specified, mixed sourcing) with elements at Tier 4 (Independently Verified) on metric inputs and at Tier 1 (Impressionistic) on algorithm selection
  authority_source: Voluntary Published
  cultural_methodological_lineage: Western institutional
  funder_typology: DAO or protocol (Optimism Collective)
  framework_scope_type: Allocator process framework (primary) with grantee outcome measurement framework characteristics (secondary)
---

# Optimism Retro Funding (RetroPGF) - CROSS+WALKRI Compatibility Statement v0.2.0

## Summary

Optimism Retro Funding (RetroPGF) is the Optimism Collective's mechanism for distributing OP tokens to projects whose contributions to the Optimism ecosystem have already occurred. It is structurally a retroactive funding program and maps cleanly onto CROSS's retroactive-obligation mode (Part III Section C). The Season 7 architecture (2025 onward) operates as a continuous reward mechanism with metrics drawn from independent data sources combined under vote-selected algorithm weights, replacing the unconstrained badge holder voting of Rounds 1-4.

CROSS+WALKRI compatibility is strongest at the evidence sourcing layer (Independent Verifiability, Attestation Corpus alignment, Format Agnosticism) and at the modular allocator architecture layer (Determination Body Separation at the algorithm-design and badge holder layers). Compatibility gaps appear at the pre-commitment layer (algorithms are selected mid-round, not pre-published before the contribution period), at the affected population verification layer (direct affected parties do not participate in evaluation), and at the badge holder declaration layer (relationships to evaluated projects are not formally declared per round).

This statement covers Season 7 (2025) and forward; Rounds 1-4 are noted as a structural predecessor with different compatibility characteristics. The companion Impact Evaluation Methodology statement (`Optimism-Retro-Funding-Impact-Evaluation-CROSS-WALKRI-compatibility-0_1_0.md`) covers the weighted formula, Impact Chain dependency graph, and human-in-the-loop override mechanism as a separate analytical angle.

## The Optimism Retro Funding Framework

### Program Structure

In 2025 the Optimism Foundation announced that "Retro Funding will no longer reward impact within annual domain-specific rounds. Instead, Retro Funding will run as a continuous reward mechanism, with a regular cadence of impact measurement and reward distribution." Season 7 launched two concurrent missions: Dev Tooling (libraries, debuggers, developer infrastructure) and Onchain Builders (projects driving cross-chain activity). A third program covers OP Stack contributions including Ethereum Core Development.

The program's overall budget is "850M OP dedicated to Retro Funding" with 2024's three rounds having distributed "20m OP across 3 retro rounds" to "over 400 builders." Season 7 distributes rewards monthly, with the first round covering February 2025 impact and five additional monthly rounds through July 2025.

### Evaluation Mechanism

RetroPGF Season 7 replaced direct project voting with a layered structure. The Optimism Foundation describes the approach as "metrics-driven, human in the loop" combining "data's systematic reach with human intuition's nuanced adjustments."

The structural innovation is that badge holders do not vote on individual projects or specific metrics. Instead, "badgeholders vote on evaluation algorithms, each representing a different philosophy for measuring impact. These algorithms are applied to two distinct Missions: Dev Tooling and Onchain Builders, with each Mission having its own pool of funds and its own set of algorithms."

The formula transitions from `evaluationAlgorithm(project) = median(badgeholder1Assesment, badgeholder2Assesment, ...)` (the Rounds 1-4 pattern) to `weight * impactMetric1 + weight * impactMetric2 + ...` (the Season 7 pattern with vote-selected weights).

For the Dev Tooling mission, three algorithms were presented in Season 7:

- **Arcturus** (winner): "rewards widely adopted tools with many downstream dependents. It emphasizes package dependencies and economic weight."
- **Bellatrix**: "favors fast-growing tools and recent developer engagement."
- **Canopus**: "emphasizes developer collaboration and GitHub activity."

For the Onchain Builders mission, three algorithms aggregating "transaction counts, gas fees, TVL, and user activity" across three variants (Adoption: current values; Growth: net increase; Retention: minimum values):

- **Goldilocks** (winner): "emphasizes retention and supports projects with consistent engagement."
- **Superscale**: "emphasizes adoption and rewards projects with high current usage."
- **Acceleratooor**: "emphasizes growth and highlights projects gaining traction."

### Data Architecture

Underlying metrics are drawn from "OSO's public data models" sourcing from "OP Atlas, raw Superchain data, decoded 4337 transactions, GitHub archive, DefiLlama, Farcaster, deps.dev, and more." This source set lies outside any individual project's control.

Dev Tooling evaluation specifically constructs "a trust graph linking onchain projects, developers, and devtooling projects" using the EigenTrust algorithm.

### Voting Design Status

A GovXS evaluation of RetroPGF voting designs found that "none of the voting rules applied in Round 1-4 is strategyproof," meaning voters could achieve better outcomes by not voting truthfully. The team proposed "two voting rule variants to address this challenge and make Retro Funding strategyproof in Round 5 and onwards." Protective measures being tested include "secret voting and random voter assignments, which are currently being tested in Rounds 5-6."

## How CROSS Satisfies the Obligation Architecture RetroPGF Operates Under

### Retroactive Obligation Mode (CROSS Part III Section C)

RetroPGF is a retroactive funding program: it rewards contributions that have already occurred rather than funding future work. CROSS Part III Section C specifies the retroactive obligation entry gate. A retroactive application must present:

1. A description of what contribution was produced
2. The period during which it was produced
3. Evidence of who is using or has benefited from it, accessible from sources outside the applicant's control
4. Concurrent funding disclosure covering any prior awards for the same or overlapping contribution

RetroPGF's metric-based architecture satisfies element 3 structurally: the metrics defining contribution and use are computed from sources outside the applicant's control (GitHub archive, on-chain data, deps.dev, DefiLlama). A project's package dependency count, transaction volume, or TVL is queryable from named public sources without the project's cooperation.

Element 4 (concurrent funding disclosure) is partially satisfied through OP Atlas project profile requirements but does not match CROSS's required field specificity (source name, source type, approximate amount, relationship to scope, ongoing obligations, decision rights). A CROSS-conformant RetroPGF would add explicit concurrent funding fields at the project profile level.

### Independent Verifiability (Commitment 6)

The Independent Verifiability commitment in the CROSS+WALKRI Evolution Rules specifies that every checkable claim must be verifiable from a source outside the claimant's control. RetroPGF's data architecture is structurally aligned with this commitment: the metrics on which allocations are based are not project self-reports. They are computed from independent registries and on-chain sources.

This is a stronger alignment than most CROSS+WALKRI-mapped frameworks achieve. Where most grants programs require independent verification of claimed outcomes after the fact, RetroPGF builds its evaluation entirely on independently sourced signals from the start.

### Attestation Corpus Alignment

The CROSS+WALKRI Attestation Corpus primitive (Layer 4) specifies a queryable record of contribution and use evidence. RetroPGF's data sources (Superchain transaction data, GitHub archive, deps.dev, DefiLlama) constitute a de facto Attestation Corpus: queryable, dated, independently maintained, addressed by named identifiers (contract addresses, package names, GitHub repos).

A CROSS-conformant RetroPGF would specify the attestation corpus formally at the round configuration level, naming the sources, the query methodology, and the dating convention. RetroPGF Season 7 effectively does this through OSO's public data models, though the formalization sits outside the program's own published documentation.

### Format Agnosticism (Commitment 5)

RetroPGF satisfies Format Agnosticism strongly. The program does not prescribe a single format for contributions. A library is counted via its package metadata; a smart contract is counted via its on-chain footprint; a developer collaboration is counted via GitHub signals. Any contribution that produces measurable activity in the data sources is admissible. Format prescription is absent; the content requirement (the contribution must be observable in the corpus) is what binds.

### Determination Body Separation (Layer 4 Primitive)

The Determination Body Separation primitive specifies that the body making the funding determination must be structurally distinct from the body receiving funding. RetroPGF satisfies this primitive at the algorithm-design layer (algorithms are written by external parties including OSO) and at the badge holder layer (badge holders are not the projects being evaluated). The relationship is mediated by the Citizens House badge distribution process, which is itself a community process. Where badge holders themselves operate or have material interest in projects being evaluated, Tier 1 and Tier 2 conflict provisions under CROSS Part VIII apply.

A CROSS-conformant RetroPGF would publish badge holder declarations of project relationships at the start of each round, mirroring the pre-review conflict declaration requirement in Part VIII.

## How WALKRI Complements RetroPGF

### Pre-Commitment as Structural Posture

The CROSS+WALKRI commitment to Falsifiability operationalizes through pre-commitment: criteria are fixed before the round runs, evidence is assessed after. RetroPGF's Season 7 architecture has a structural gap here. The algorithms are selected by badge holder vote during the round, not pre-published before contributions are made. A project contributing in February 2025 cannot know which algorithm will be chosen to score February 2025 impact until the badge holders have voted.

This is the central CROSS+WALKRI compatibility gap. The metric inputs are independently sourced and falsifiable; the weights applied to those inputs are determined after the fact by vote. Pre-published metrics with vote-selected weights produce a partially falsifiable evaluation; the falsifiability holds at the metric layer but not at the weighting layer.

A CROSS-conformant RetroPGF would pre-publish either the algorithm itself or a stable algorithm family (defining which metric combinations are admissible) before the period of contribution begins. The community vote could then occur within the pre-committed algorithm space rather than determining the algorithm space itself.

### Adverse Signal Engagement Principle

The Adverse-Signal Engagement Principle Core Standard requires that adverse signals (prior rejections, contradictory findings, negative due diligence) be surfaced rather than suppressed. RetroPGF's metric-based architecture is partially compatible: where a project's metrics reveal adverse signals (declining usage, narrow dependency footprint, concentrated user base), the algorithms surface those signals through their scoring. The GovXS evaluation's strategyproofness finding (Rounds 1-4 not strategyproof) is itself an adverse signal about the voting design that the Optimism Foundation has surfaced and acted on by testing strategyproof variants in Rounds 5-6.

A CROSS-conformant RetroPGF would publish a standing adverse signal log per round naming the structural concerns identified and the response taken.

### Affected Population Verification Mechanism

The Affected Population Verification Gate primitive (Layer 4) specifies that the affected population of a program has a mechanism for engaging with the program. RetroPGF's structure does not include direct affected-population engagement: the downstream parties of RetroPGF-funded work are developers, users, and protocols, and these parties do not participate in the evaluation. This is a structural feature of retroactive funding more broadly; the question of who counts as the affected population and how they participate is a known unresolved area in web3 grants design.

This gap is not a defect; it is a known boundary of the retroactive-funding model. A CROSS-conformant RetroPGF would name the boundary explicitly in its published documentation rather than leave the affected-population question implicit.

### Pre-Award Indicator Confirmation Stage

The Pre-Award Indicator Confirmation Stage primitive (Layer 3) specifies a stage where the program confirms with the applicant that the indicators of contribution to be measured are agreed before the evaluation runs. In RetroPGF, projects can register on OP Atlas and submit their project information; this is a partial implementation. A full Pre-Award Indicator Confirmation Stage would have each project explicitly acknowledge which metric set will be applied to its evaluation before the badge holder vote on algorithms occurs.

## The OSO Bridge

CROSS+WALKRI has a published compatibility statement for Open Source Observer (`OSO-WALKRI-compatibility-0_1_0.md` in this series). The conclusion of that statement is directly relevant here: a WALKRI-conformant recipient profile that includes the on-chain identity anchor, GitHub URL, and npm package identifiers is directly importable as an OSO oss-directory entry. Because CROSS+WALKRI is already OSO-compatible, Optimism's OSO-powered metrics are inherently CROSS+WALKRI-compatible. Programs that run CROSS-conformant rounds with WALKRI-specified OSO evidence forms produce the exact data infrastructure that RetroPGF evaluation requires.

## Compatibility Findings

### Strong alignments

- Retroactive obligation mode mapping is structural and clean
- Independent Verifiability commitment satisfied at the metric input layer
- Attestation Corpus structurally present via OSO data models, deps.dev, GitHub archive
- Format Agnosticism satisfied (no format prescription beyond observability)
- Determination Body Separation present at algorithm-design and badge holder layers

### Partial alignments

- Falsifiability holds at metric layer, falters at algorithm-weighting layer (algorithms selected mid-round)
- Adverse Signal Engagement is present in the public availability of voting-design findings (GovXS evaluation published openly) but not formalized as a program discipline
- Concurrent funding disclosure occurs through OP Atlas but lacks CROSS field specificity

### Compatibility gaps requiring program adjustment for full conformance

- Pre-commitment: algorithms or algorithm family should be published before the contribution period begins
- Affected Population Verification: the boundary of who participates as affected population should be named explicitly
- Determination Body Separation: badge holder relationships to evaluated projects should be declared per round
- Pre-Award Indicator Confirmation: projects should explicitly acknowledge applicable metrics before evaluation

### Structural compatibilities of historical interest

RetroPGF Rounds 1-4 used direct project voting and operated structurally closer to a project-selection allocator process. The Season 7 transition to algorithm voting represents a structural pivot toward Independent Verifiability and away from impressionistic project selection. The pivot is in the direction of CROSS+WALKRI compatibility. The Impact Evaluation Methodology companion statement (v0.1.0, 2026-05-18) covers the weighted formula, Impact Chain dependency graph, and human-in-the-loop override mechanism as separate structural innovations layered on this base.

## Mapping Table

| Optimism Retro Funding Element | CROSS Provision | WALKRI Provision |
| :-- | :-- | :-- |
| Continuous reward mechanism with monthly rounds | Retroactive obligation mode operating at sub-annual cadence | Pre-publication requirements apply per round |
| Metric definitions published before evaluation opens | Entry specification gate: criteria fixed before applications open | Pre-publication field requirements: criterion intent, operational definition, conformance threshold |
| Metrics verifiable from independent public sources | Independent Verifiability (Commitment 6); Attestation Corpus query | Validity standard (5.1); Integrity standard (5.2) |
| Metrics reproducible by any evaluator | Gate configuration includes evidence scope and strength specification | Evidence form requirement (OSO query with named access path) |
| Project identity anchored to on-chain addresses and GitHub orgs | Organizational Identity primitive (Field 6: on-chain identity anchor) | Recipient profile exportable as OSO oss-directory YAML |
| Algorithms selected by badge holder vote during round | Gap: pre-commitment not satisfied at the algorithm-weighting layer | Gap: evidence form weighted post-publication |
| Badge holders distinct from evaluated projects | Determination Body Separation (Layer 4 primitive) | Not applicable at the field level |
| Algorithm-design by external parties (OSO, GovXS) | Determination Body Separation reinforced at the algorithm-design layer | Not applicable at the field level |
| Direct affected-population non-participation | Affected Population Verification Gate not implemented (known retroactive-funding boundary) | Not applicable at the field level |
| Strategyproofness testing (Rounds 5-6) | Adverse Signal Engagement Principle structurally present in published GovXS findings | Not applicable at the field level |

## Calibration Tier Assessment

RetroPGF Season 7 sits at a mixed calibration tier in the CROSS+WALKRI Lenses Framework:

- **Tier 4 (Independently Verified)** at the metric input layer: contributions counted from sources outside applicant control
- **Tier 1 (Impressionistic)** at the algorithm selection layer: badge holders select algorithms by vote without published rubric criteria

Aggregating, the program operates at Tier 3 (Outcome Specified, mixed sourcing). Progression to Tier 4 requires algorithm family pre-publication. Progression to Tier 5 (Falsifiable) requires Adverse Signal Engagement as an explicit program discipline plus multi-cycle Retrospective Assessment publication. The Season 7 architecture is structurally positioned for incremental advancement to higher tiers without methodology replacement.

**Current+target trajectory:**

- Current: Tier 3 (mixed sourcing as described above)
- Next achievable target (Season 8 or 9, within current architecture): Tier 4 via algorithm family pre-publication
- Long-range target (within 2-3 years if pursued): Tier 5 via formal Adverse Signal Engagement discipline plus published multi-cycle Retrospective Assessment

## Pre-Funding Specification Layer

A CROSS+WALKRI-conformant RetroPGF round produces something the current framework does not require but would benefit from: a pre-funding specification layer that makes the metrics trustworthy before evaluation begins. The current process publishes metric definitions before evaluation opens. CROSS+WALKRI extends this by requiring those definitions to meet the WALKRI field specification standard: each metric must have a stated criterion intent, an operational definition that specifies its boundary conditions, a documented evidence form with an OSO access path, and a conformance threshold. This elevates the metric definition from a name-and-description pair to a structured, auditable specification.

The result is that badge holders evaluate contributions against metrics whose measurement instruments are documented in advance, whose access paths are independently verifiable, and whose operational definitions remove ambiguity about what counts. This is the structural counterpart to the Falsifiability commitment, applied at the round-configuration layer.

## Compatibility Statement Maturity

This is a Tier 2 compatibility statement under the CROSS+WALKRI primitives framework index: the source framework is a structurally novel exemplar of metric-driven retroactive funding with vote-selected weights, and it warrants a full statement rather than a Tier 2 index entry. The statement will be revised as RetroPGF Season 7 results are published and as Rounds 5-6 strategyproofness experiments report.

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

Optimism Operating Manual: https://github.com/ethereum-optimism/OPerating-manual

Optimism Governance Forum: https://gov.optimism.io

Open Source Observer: https://docs.opensource.observer

Optimism Retro Funding announcement: optimism.io/blog/retro-funding-2025

OSO evaluation algorithm analysis: docs.oso.xyz/blog/retro-funding-s7-release

License: CC0

## Changelog

- **0.2.2 (2026-06-08):** Re-verified Frame Language own-voice clean as part of the corpus-wide 2026-06-08 sweep; the substantive own-voice pass was applied earlier (see prior entry). No further changes; vocabulary already aligned and primitive-rename references confirmed against current canon.
- **0.2.1 (2026-05-23):** Primitive rename cascade applied. The "Beneficiary Accountability Mechanism" section heading is now "Affected Population Verification Mechanism"; the referenced primitive is renamed from "Beneficiary Accountability Gate" to "Affected Population Verification Gate" (Layer 4; the prior text incorrectly stated Layer 3 and is corrected to Layer 4 to match the rest of the corpus). The compatibility-gaps bullet, the mapping-table row for direct affected-population non-participation, and the lead-paragraph compatibility summary are updated to the new primitive name. RetroPGF's structural gap remains unchanged. Historical changelog entry below retains the prior primitive name as it stood at the time of release.
- **0.2.0 (2026-05-23):** Major revision incorporating Season 7 algorithm-voting architecture (Dev Tooling and Onchain Builders missions; Arcturus/Bellatrix/Canopus and Goldilocks/Superscale/Acceleratooor algorithm sets), GovXS strategyproofness evaluation findings, and CROSS+WALKRI Evolution Rules v0.1.2 alignment (six design commitments including Format Agnosticism and Independent Verifiability). Added lens tags (Tier 3 mixed sourcing; Voluntary Published authority; Western institutional lineage; DAO or protocol funder typology; Allocator process primary scope). Added Calibration Tier current+target trajectory. Added pre-commitment, beneficiary accountability, and badge holder declaration gap analysis. Source quotation discipline applied: verbatim quotes from Optimism Foundation blog, OSO blog, Optimism governance forum. Frame Language audit applied throughout. Supersedes v0.1.0 (2026-05-18).
- **0.1.0 (2026-05-18):** Initial draft. Retroactive obligation mode alignment with RetroPGF structure. WALKRI evidence form mapped to verifiability and reproducibility requirements. OSO compatibility bridge documented. Mapping table covering entry specification gate, on-chain identity anchor, cohort position assessment, and WALKRI data quality standards.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri. For the source framework, see optimism.io.*
