---
title: ENS DAO Grants CROSS+WALKRI Compatibility Statement
version: 0.1.1
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
conforms_to: cross-walkri/primitives-foundation@0.1.7
source_framework: ENS DAO Grants ecosystem (2024-2026)
source_framework_authority: ENS Foundation (Cayman Islands), ENS DAO (ENS token holders), Public Goods Working Group, Ecosystem Working Group, Meta-Governance Working Group
references:
  - ENS Documentation. "ENS DAO." docs.ens.domains/dao
  - ENS Documentation. "Governance Process." docs.ens.domains/dao/governance/process
  - ENS DAO Basics. "Constitution." basics.ensdao.org/ensdao-constitution
  - ENS DAO Basics. "Working Groups." basics.ensdao.org/working-groups
  - ENS DAO Basics. "Public Goods WG." basics.ensdao.org/public-goods
  - ENS DAO Basics. "Voting." basics.ensdao.org/voting
  - ENS DAO Basics. "Executable Proposals." basics.ensdao.org/executable-proposals
  - ENS DAO Basics. "Funding Requests." basics.ensdao.org/funding-requests
  - ENS DAO Governance Forum. "ENS Public Goods Working Group - Term 6 (2025) Report." discuss.ens.domains/t/ens-public-goods-working-group-term-6-2025-report/21689
  - ENS DAO Governance Forum. "[Temp Check] ENS Retro: An ENS DAO Retrospective and Stakeholder Analysis." discuss.ens.domains/t/temp-check-ens-retro-an-ens-dao-retrospective-stakeholder-analysis/21648
  - ENS DAO Governance Forum. "Retrospective Research Update: Phase 1 Complete." discuss.ens.domains/t/retrospective-research-update-phase-1-complete/21935
  - ENS DAO Proposal Record. "[5.17.3] [Social] Funding Request: ENS Public Goods Working Group." docs.ens.domains/dao/proposals/5.17.3
  - ENS DAO Proposal Record. "[5.5] Public Goods Working Group Term 5 (Q1/Q2)." docs.ens.domains/dao/proposals/5.5
  - ENS DAO Proposal Record. "[6.6.2] April Funding Request ENS Public Goods." docs.ens.domains/dao/proposals/6.6.2
  - ENS Small Grants. "Frequently Asked Questions." ensgrants.xyz/faq
  - Karpatkey. "Kpk 2025 Review for the ENS Endowment." discuss.ens.domains/t/kpk-2025-review-for-the-ens-endowment/21829
lens_tags:
  calibration_tier: Tier 2 (Process Conformant) aggregate, with Tier 1 (Impressionistic) at the Working Group steward discretion layer for strategic and discretionary grant decisions and at the Small Grants snapshot-vote outcome interpretation layer, and Tier 3 (Outcome Specified, Self-Reported) at the Large Grants milestone-tied disbursement layer; the in-progress Metagov retrospective points toward Tier 4 trajectory
  authority_source: Voluntary Published
  cultural_methodological_lineage: Western institutional with hybrid DAO decision-making lineage
  funder_typology: DAO or protocol (ENS DAO via ENS Foundation)
  framework_scope_type: Allocator process framework (primary), with grantee outcome measurement framework characteristics (secondary)
---

# ENS DAO Grants - CROSS+WALKRI Compatibility Statement

## Summary

ENS DAO Grants is a multi-track funding ecosystem operated by three elected Working Groups (Public Goods, Ecosystem, Meta-Governance) under ENS DAO (ENS token holder) decision-making, with the ENS Foundation (a Cayman Islands foundation company) providing a legal wrapper. Funding flows through a two-step decision-making pattern in which Working Group budgets are first approved as Social Proposals on Snapshot, then bundled into a Collective Executable Proposal that transfers treasury funds on-chain to each Working Group's four-of-four multisig (three elected stewards plus an appointed secretary, with 3-of-4 signing authority). The Public Goods Working Group operates Small Grants (community-voted micro-grants per quarter), Large Grants (up to 50k USDC with milestone-tied disbursement), Strategic Grants (up to 150k USDC for named long-term initiatives), Builder Grants, and discretionary bounty pools. The Ecosystem Working Group operates a parallel grants track for ENS-specific work.

CROSS+WALKRI compatibility is strongest at the pre-commitment layer (Working Group budgets, Constitution, and treasury commitments are pre-published via on-chain Executable Proposal records with a 2-day timelock before execution), at the Determination Body Separation layer (Working Group stewards are elected by ENS token holders annually and are structurally separate from applicants within their domain; the DAO itself sits outside Working Group budget allocation as the ratifying body), at the Independent Verifiability layer (Snapshot offchain votes are stored on IPFS, executable proposals are on-chain at vote.ensdao.org, treasury movements are queryable from public chain data, and Karpatkey endowment operations are reported in quarterly forum posts), and at the Inter-cycle Reflection Stage layer (the Metagov-led ENS DAO Retrospective and Stakeholder Analysis, contracted at approximately $125k for completion by March 2026, is itself a structurally aligned exemplar of the primitive). Compatibility gaps appear at the published-rubric layer for steward-discretionary grant decisions (Strategic, Builder, and discretionary tracks operate against narrative criteria rather than published criteria at CROSS Part VIII granularity), at the Affected Population Verification Gate layer (downstream users of funded public goods do not formally participate in completion verification), and at the standing Adverse Signal Engagement layer (the Metagov retrospective is a one-time research contract rather than a continuing program discipline, with structural change to the Working Group architecture itself under discussion via the Coordination Layer and Admin Panel temp checks).

This statement covers the 2024-2026 era of ENS DAO Grants, including the Term 6 (2025) Public Goods Working Group cycle and the in-progress Metagov retrospective whose Phase 1 (Michael Cooper, 23 key informant interviews, 30 hours of interview time) completed in early 2026.

## The ENS DAO Grants Framework

### DAO Structure and Legal Wrapper

The ENS DAO operates under a Constitution ratified in November 2021 by social vote of ENS token holders (per ENS DAO Basics: 97% approval of 84,350 wallets and 15m votes participating). The Constitution names five articles binding the DAO: Name Ownership Protection (Article 1); Fee Purpose (Article 2: "Fees are primarily an incentive mechanism" to prevent speculative name hoarding); Treasury Allocation (Article 3); DNS Integration (Article 4: "ENS integrates with the global namespace" without sacrificing decentralization); and Amendment Process (Article 5: changes require two-thirds majority with minimum 1% participation, currently 1m ENS).

Treasury Allocation under Article 3 is the constitutional anchor for grants spending. The Constitution specifies that "income must first ensure ENS's long-term viability and development. Surplus may fund other web3 public goods, provided recipients commit to constitutional principles and funded projects align with ENS goals."

The ENS Foundation is the Cayman Islands legal wrapper that gives the DAO real-world contracting authority and the demonstrated function to hold assets and execute agreements on the DAO's behalf. Per the ENS Documentation, "The ENS Foundation's Articles of Incorporation give significant powers to the ENS DAO (referred to as 'The Council' in the Articles)." The DAO may "vote to appoint or remove a director, member, or supervisor, prohibit admitting any members in future, instruct the directors to wind up the foundation," and direct the foundation to take specific actions on its behalf. A Cayman firm (DS Limited) holds the supervisor role.

### Decision-Making Architecture

ENS DAO recognizes three proposal types per the published Governance Process documentation:

- **Social Proposal**: "A proposal that asks for the agreement of the DAO on something that cannot be enforced onchain." Voted on Snapshot (offchain, gasless, IPFS-stored). 5-day voting period. Submission threshold: 10,000 ENS delegated.
- **Constitutional Amendment**: A specialized Social Proposal requesting changes to the Constitution. Requires a diff showing exact modifications. Two-thirds approval threshold and 1% quorum.
- **Executable Proposal**: "A proposal for a series of smart contract operations to be executed by accounts the DAO controls." On-chain at vote.ensdao.org. 7-day voting period. Submission threshold: 100,000 ENS delegated. Passes if at least 1m votes (1% of total supply) vote in favor. 2-day timelock before execution.

The process follows three sequential phases per the published documentation: Temperature Check on the Discourse forum; Draft Proposal on GitHub; Active Proposal on Snapshot for social votes or on the on-chain Governor contract for executable votes. Per ENS DAO Basics on Executable Proposals, "all code related to Executable Proposals is simulated using Tenderly prior to a proposal being submitted," since execution cannot be stopped once a proposal passes.

### Working Group Architecture

Three Working Groups operate the DAO's work portfolio: Meta-Governance, Public Goods, and ENS Ecosystem. Per ENS DAO Basics on Working Groups: "Working groups are governed by a set of rules covering the creation, management, and dissolution of working groups." The current rules were passed as a social proposal in December 2021 with subsequent amendments in June 2022 and November 2023.

Each Working Group is structured identically. Per ENS DAO Basics: "Each working group has three stewards" serving 12-month terms, elected annually in December. "Each working group has a multi-sig managed by four multisig-signers" (the three stewards plus an appointed secretary), and "each multi-sig requires three-of-four signing to approve transactions." Within five days of a term starting, "each working group must appoint a Lead Steward." The Meta-Governance Working Group stewards select the steward election method each term; ENS DAO Basics notes "the first two used ranked-choice voting; the third used approval voting."

### Funding Request Flow

Working Group funding follows a two-step proposal cycle. Per ENS DAO Basics on Funding Requests: working group stewards "must first prepare and pass a social funding request" before "combining all funding requests into a single collective executable proposal." After the collective executable passes, "working group funds are distributed to each working group's multisig. Stewards then have discretion over how those funds are disbursed to initiatives."

Recent funding requests illustrate the scale and structure of Public Goods Working Group operations:

- **EP 5.17.3 (April 2025 funding through April 2025)**: 226,000 USDC requested for Builder Grants, Public Goods Perpetual Bounty, Events and Hackathons (ETHGlobal Bangkok, Devcon, ETHDenver 2025), and Discretionary funds. The proposal cited Article III of the Constitution as the authorization basis.
- **EP 6.6.2 (April 2025 second funding request)**: 356k USDC requested. Categories: Strategic Grants 300k, Builder Grants 150k, Discretionary (10% buffer) 45k. The proposal references "clear criteria for success and impact measurement from the outset" for strategic grants without specifying a published rubric.
- **EP 5.5 (Term 5 Q1/Q2)**: 450.3k USDC and 21.5 ETH requested for a six-month period covering Large Grants (387.5k USDC for milestone-based disbursement up to 50k per grantee), Small Grants (approximately 12.5 ETH per quarter), Bounties (45k USDC), Events & Hackathons (115k USDC), and Discretionary (50k USDC and 5 ETH).

### Grant Tracks Inside the Public Goods Working Group

Within the Public Goods Working Group budget, four named tracks operate concurrently:

**Strategic Grants** target "underfunded yet critical areas such as developer tools, core dependencies and infrastructure." Per the Term 6 (2025) Report, Strategic Grants in Term 6 totaled 375,000 USDC across six named initiatives: Decentralization Research Center ($150,000 for policy advocacy and decentralization research), Vyper ($50,000 matched by Ethereum Foundation), Remix Labs ($50,000 supporting transition to independent sustainability), Fabric ($50,000 for rollup standards and infrastructure coordination), Argot Collective ($100,000 for Solidity and related tools stewardship), and ICANN Engagement (up to $25,000 for naming policy representation). Strategic grants are "structured with co-funding compatibility and milestone accountability in mind."

**Large Grants** provide up to 50k USDC with applications accepted on a rolling basis throughout the term. Per the Term 5 proposal: "Large Grants up to 50k USDC with applications accepted on a rolling basis throughout the year-long term." Per the search summary findings on the Term 6 documentation: "Large Grants allow projects to request tailored funding amounts, ranging from 12k to 50k USDC, supporting impactful initiatives that demonstrate exceptional usefulness or a proven track record of benefiting users or developers." Applications are "reviewed by the Public Goods Working Group stewards on a rolling basis and evaluated based on the project's usefulness and impact." Grant stages and milestones are "reviewed by the stewards, with proof of completion needing to be clear."

**Small Grants** (operated through the ensgrants.xyz platform) are quarterly micro-grants voted on by ENS token holders directly via Snapshot. Per the ENS Small Grants FAQ: "The intention of both the Ecosystem and Public Goods Working Groups is to run one round per quarter." Round 12 returned to the standing token-weighted rule: "1 ENS token = 1 vote." Two categories operate: "Projects eligible for the Public Goods small grants rounds have a broader scope that benefits the entire Ethereum or Web3 space"; "Projects eligible for the Ecosystem small grants rounds are those that build on or improve the ENS Ecosystem." Submissions are "signed and stored in an offchain database, then later uploaded to Arweave."

**Builder Grants** are smaller-amount grants distributed at hackathons and through rolling submissions. Per the Term 6 (2025) Report: "Total distributed: 57.75 ETH + 10,000 USDC across 46 grants" to "approximately 40+ unique builder participants" in the range "0.25 ETH to 2 ETH, milestone-based."

### The Endowment and Karpatkey Treasury Architecture

ENS treasury operations are split between the Working Group multisig disbursement layer (described above) and the Endowment layer operated by Karpatkey under a delegated multisig with Zodiac Roles-modifier permissions. Per the Kpk 2025 Review for the ENS Endowment: "Since its inception, the Endowment has generated $2.92M in DeFi results (net of fees) for ENS, with DeFi results representing 12% of total revenue for ENS in 2024." Karpatkey publishes quarterly reviews in the Treasury Management category of the Discourse forum. The Endowment is bound by an "Investment Policy Statement defining key roles and responsibilities" and operates "a robust risk management stack, leveraging risk data service providers including Hypernative and Redefine."

### In-Progress Retrospective Evaluation

ENS DAO contracted Metagov in late 2025 to conduct an independent retrospective evaluation. Per the temp check proposal: "The ENS DAO Retro and Stakeholder Analysis would be fully conducted by Eugene and Metagov.org as an independent party." The proposal targets approximately "$125k +/- $25k" budget across a four-month delivery window, with Metagov as the named neutral third party so "no internal DAO politics blur the intent or output."

Per the Phase 1 update post from early 2026: the Metagov Research team led by Michael Cooper conducted "approximately 23 key informant interviews with ENS stakeholders, totaling just under 30 hours of interview time" plus "full inventory and ingestion of all agreed public data sources into a shared repository." Phase 1 deliverables include "a synopsis of interview findings (covering the main governance challenges and systemic patterns identified so far)." Phase 1 results were scheduled for presentation on March 10, 2026.

Concurrently, several restructuring proposals are under discussion: a Coordination Layer 12-month pilot proposal, a Working Group Restructure temp check, and an Admin Panel temp check that, if approved, would require "all Working Groups must return remaining funds to the DAO and transfer ownership of multisigs to the elected Admin Panel by December 31, 2025." The future of the three-Working-Group architecture is under active deliberation as of mid-2026.

## How CROSS Satisfies the Obligation Architecture ENS DAO Grants Operates Under

### Mixed Obligation Mode

ENS DAO Grants operates across CROSS's three obligation modes (Part III) simultaneously, depending on the grant track. Large Grants and Strategic Grants operate primarily in Build mode (the obligation object is the produced output: developer tooling, infrastructure, policy work, or named programmatic deliverables) with milestone-tied disbursement against committed completion criteria. Small Grants operate in a participation-weighted retrospective-adjacent mode (the obligation object is contribution as judged by the ENS-token-weighted vote at the close of each quarterly round). Builder Grants operate in a hybrid Build-mode-with-light-completion-verification pattern (small amounts, milestone-based with steward review, low evidence-strength configuration).

A CROSS-conformant ENS DAO Grants would declare the obligation mode at each grant track's published criteria. The current architecture is implicit; declaration would be additive without breaking the existing Working Group structure.

### Pre-commitment as Structural Posture (Falsifiability Operationalization)

The Discourse-to-Snapshot-to-Executable flow is structurally aligned with pre-commitment. Working Group budgets are published on Discourse during temperature check, voted on Snapshot as Social Proposals, and then bundled into Executable Proposals voted on-chain with a 2-day timelock before disbursement. Once the executable proposal passes and the timelock elapses, the funds transfer to the Working Group multisig and the budget categories named in the proposal are the operative envelope.

This is pre-commitment at the budget-envelope layer: the categories and totals are fixed before the term runs; subsequent steward decisions occur within the pre-committed envelope. The Constitution itself is a stronger form of pre-commitment, having been ratified in 2021 and amendable only by two-thirds majority of ENS token holders.

The structural form is closer to Arbitrum DAO's Discourse-to-Tally pattern than to RetroPGF's Season 7 mid-round algorithm vote. The pre-commitment holds at the budget envelope and the program structure; it does not hold at the per-grant level, where steward discretion operates within the envelope.

### Determination Body Separation (Layer 4 Primitive)

The Determination Body Separation primitive is satisfied at multiple layers in ENS DAO:

**At the macro DAO decision-making layer.** ENS token holders voting on Snapshot and on-chain at vote.ensdao.org are structurally separate from grant applicants. The on-chain Executable Proposal record is queryable from public Ethereum data; Snapshot offchain votes are queryable from IPFS. The determination body's actions are independently verifiable.

**At the Working Group steward layer.** Stewards are elected by ENS token holders for 12-month terms and are structurally separate from applicants within their domain. The election method itself is selected by the Meta-Governance Working Group (ranked-choice or approval voting), which is itself elected by the broader DAO. Re-election or non-renewal is the named response to non-conformance at the steward layer.

**At the Foundation layer.** The ENS Foundation is a Cayman Islands legal entity with a supervisor (DS Limited) and Articles of Incorporation that give the DAO authority over the Foundation's directors. The Foundation cannot itself grant funds; it executes what the DAO directs.

A residual gap appears at the steward-discretion layer within Working Group multisigs: the 3-of-4 signing requirement means that any three of the four signers (three stewards plus one appointed secretary) can authorize disbursement. Where stewards make discretionary grant decisions (Strategic Grants, Builder Grants, discretionary bounty pools), the determination body is structurally separate from applicants but the determination criteria are not published at CROSS Part VIII granularity. The Determination Body Separation primitive is satisfied at the institutional layer; the criterion specification is not.

### Attestation Corpus Alignment

The CROSS+WALKRI Attestation Corpus primitive (Layer 4) is satisfied at depth by the ENS architecture. Multiple queryable sources operate without applicant participation: on-chain Executable Proposal records (every proposal at vote.ensdao.org, with execution traces on Ethereum mainnet); Snapshot offchain vote records (stored on IPFS, signed by delegates); on-chain treasury movements (every transfer from the DAO wallet to a Working Group multisig is queryable from Etherscan); the Karpatkey Endowment dashboard and quarterly forum reviews; the ensgrants.xyz Arweave-archived Small Grants submissions; the Discourse forum (publicly accessible, with full proposal histories); and the Dune dashboards referenced in the Term 6 Report ("clear public accountability via Dune dashboard").

A CROSS-conformant ENS DAO Grants would formalize the Attestation Corpus specification at each grant track's configuration, naming which sources apply to which evaluation layer (e.g., on-chain identity anchor for the recipient wallet; GitHub repository for Builder Grant deliverables; Arweave hash for Small Grant submission persistence).

### Format Agnosticism (Commitment 5)

ENS DAO Grants satisfies Format Agnosticism partially. The program does not prescribe a single output format; grantees can deliver code, documentation, dashboards, research, events, hackathon participation, or policy work. The Small Grants FAQ specifically notes "No required proposal template; creative submissions encouraged."

However, application content varies considerably across tracks (Small Grants are short Snapshot proposals; Large Grants and Strategic Grants are longer narrative submissions to stewards; Builder Grants are minimal). A CROSS-conformant ENS DAO Grants would name the content requirements that bind across all tracks (e.g., organizational identity declaration, on-chain identity anchor, public benefit mechanism declaration) and leave format prescription absent per the commitment.

### Independent Verifiability (Commitment 6)

The ENS DAO Grants architecture's compatibility with Independent Verifiability is layered:

**Strong at the on-chain decision-making layer.** Snapshot votes are on IPFS, queryable by any party. Executable Proposal votes are on-chain. The Tenderly simulation requirement for Executable Proposals is itself a structural pre-execution verification step.

**Strong at the disbursement layer.** Every transfer from the DAO wallet to a Working Group multisig is on-chain. Every multisig transaction (3-of-4 approval) is on-chain. The traceability of treasury flows from DAO to Working Group to grantee is publicly accessible.

**Partial at the grant outcome layer.** Large Grants and Strategic Grants are milestone-tied; "each grant stage and its milestones are reviewed by the stewards, with proof of completion needing to be clear." The verification of completion is steward-internal rather than independently re-derivable from a published rubric and independent reviewer. Where deliverables are public artifacts (open-source code, published research, hackathon outputs), Independent Verifiability is structurally available; where deliverables are operational milestones interpreted by stewards, it is partial.

**Weak at the discretionary-track layer.** Discretionary grants and Builder Grants distributed at steward judgment within the multisig envelope are recorded on-chain (the transfer is verifiable) but the decision logic is not published at a level allowing independent re-derivation.

## How WALKRI Complements ENS DAO Grants

### Evidence Form Specifications

WALKRI's evidence form requirement specifies that every measurement instrument include a documented data source and an independently accessible access path. ENS DAO Grants' evidence forms vary by track. Small Grants outcome evidence is the Snapshot vote tally (independently verifiable from IPFS). Large Grants milestone evidence is steward-reviewed (steward report on the forum is the access path). Strategic Grants outcome evidence is the grantee's reported delivery against the named initiative scope (typically public artifacts, GitHub commits, or research publications).

A WALKRI-conformant ENS DAO Grants would specify for each grant track: the criterion intent (what the track is designed to fund and what counts as success), the operational definition (exactly what artifacts or evidence count and what does not), the response form (how the evidence is recorded), the evidence form (where the data is sourced and how it can be accessed), and the conformance threshold (the minimum that triggers grant approval or final disbursement). For Strategic Grants and Large Grants in particular, this would convert the current narrative "usefulness and impact" criterion into a structured specification.

### Adverse Signal Engagement Principle

The Adverse-Signal Engagement Principle Core Standard requires that adverse signals be surfaced rather than suppressed. ENS DAO has structural openings for this principle but currently operates with limited standing discipline.

The Metagov-led retrospective is itself an Adverse Signal Engagement Principle-aligned exercise at the DAO-portfolio level. Per the Phase 1 update: the Metagov team is producing "a synopsis of interview findings (covering the main governance challenges and systemic patterns identified so far)." The temp check proposal explicitly named the research questions: "What funding was approved versus withheld? What deliverables materialized versus fell short? What are ways in which the DAO can be more rigorous and more easily held accountable?" This is exactly the discipline the principle requires.

However, the retrospective is a one-time research contract, not a standing program discipline. The Term 6 Public Goods Report itself, per the source extract, "does not explicitly identify shortcomings or failures. It presents Term 6 as the 'most productive and strategically aligned term' without detailed retrospective critique of challenges or unsuccessful initiatives." This is the structural gap.

A CROSS-conformant ENS DAO Grants would integrate the Metagov-style assessment as a recurring discipline at each Working Group's term close, producing per-term adverse signal logs that name specific structural concerns identified and the response taken.

### Inter-cycle Reflection Stage (Layer 4 Primitive)

The Metagov retrospective functions as an Inter-cycle Reflection Stage applied retroactively to the DAO's first multi-term cycle of operations. The Primitives Foundation specifies the Inter-cycle Reflection Stage as a reflection on round outcomes published before the next cycle opens with three required elements: the reflection artifact, the design response, and the publication timing.

The Metagov work matches the artifact element (a published synthesis from 23 interviews and 30 hours of interview time, plus the data repository). The design response element is structurally indicated by the concurrent restructuring temp checks (Coordination Layer, Working Group Restructure, Admin Panel). The publication timing element is partially satisfied: Phase 1 was scheduled for presentation on March 10, 2026, with subsequent phases targeting completion by March 2026 to feed into the next round of structural changes to the Working Group architecture.

A CROSS-conformant ENS DAO Grants would make Inter-cycle Reflection Stage publications a standing pre-committed requirement at each Working Group's term configuration, with publication deadlines tied to the December election cycle. The Metagov contract is structurally adjacent to this requirement; making it standing would close the temporal gap.

### Affected Population Verification Gate (Layer 4 Primitive)

The Affected Population Verification Gate primitive specifies that the people or communities served by a funded program participate in verifying what was delivered. ENS DAO Grants' structure does not include direct affected-population engagement at completion: the affected population of funded public goods is typically the broader Ethereum and Web3 developer community (for Strategic and Large Grants funding developer tooling, infrastructure, research) and they do not participate formally in the verification of grant outcomes.

ENS Small Grants approaches this primitive through token-weighted voting, which serves as a form of community signal but operates on contributor preference rather than affected-population verification of delivered work. The ENS-token-weighted vote represents the community of token holders, not the community of downstream users of funded work.

This is a structural feature of the public-goods grants model that ENS shares with Gitcoin Grants. The Small Grants model substitutes participation-at-allocation for verification-at-completion; the Large Grants and Strategic Grants tracks are steward-verified at completion rather than affected-population-verified.

A CROSS-conformant ENS DAO Grants would add a completion-side affected-population verification mechanism for Strategic and Large Grants, particularly for grants whose declared public benefit mechanism is condition change or access provision in a named population. Builder Grants and Small Grants would be excepted on Coordination Scaling Standard grounds (the grant scale does not justify a full verification gate).

### Beneficiary Validation Mechanism (Layer 3 Primitive)

The Beneficiary Validation Mechanism primitive specifies that the FROM state, population definition, or need claim of an applying entity is independently validated by parties drawn from or bound by obligation directions to the affected population at the entry specification gate. ENS DAO Grants partially satisfies this through Working Group steward elections: stewards are elected by ENS token holders, and their domain specialization (public goods, ecosystem, meta-governance) is a form of structural alignment with the type of work they evaluate.

However, the formal Beneficiary Validation Mechanism is stronger than steward election. The primitive requires that named parties from the affected population assess the applying entity's characterization of the population, the need, and the FROM state. ENS DAO operates primarily on output-production and ecosystem-shift public benefit mechanism types, where the affected population is diffuse and the validation mechanism is correspondingly indirect.

For Strategic Grants funding population-anchored work (e.g., Decentralization Research Center's policy advocacy, ICANN Engagement's naming-policy representation), a CROSS-conformant ENS DAO Grants would add a structured beneficiary validation step that names the affected population, the validating parties drawn from or bound to it, and the validation procedure.

### Pre-Award Indicator Confirmation Stage (Layer 3 Primitive)

The Pre-Award Indicator Confirmation Stage primitive specifies a structured stage between funder selection and disbursement where indicator definitions, milestone bindings, and evidence form specifications are finalized. ENS DAO Grants' Large Grants and Strategic Grants partially satisfy this through milestone-tied disbursement structure: "If selected, applicants work on the milestones outlined in their submission, and while withdrawals do not require approval, each grant stage and its milestones are reviewed by the stewards."

The milestone definition occurs in the application submission and is operationalized by steward review. This is closer to a Pre-Award Indicator Confirmation Stage than to a bare application gate, but it is not formalized: there is no documented stage where the funder and the selected applicant converge on the indicator definitions and evidence forms before disbursement begins. The milestone structure substitutes for the formal confirmation stage.

A CROSS-conformant ENS DAO Grants would add a Pre-Award Indicator Confirmation Stage for Strategic and Large Grants, producing a written confirmation that becomes the operative specification for subsequent steward gate determinations.

## Compatibility Findings

### Strong alignments

- Pre-commitment at the budget envelope layer (Discourse-to-Snapshot-to-Executable flow with 2-day timelock; Constitution as deeper pre-commitment ratified November 2021)
- Determination Body Separation at macro DAO decision-making and Working Group steward election layers
- Attestation Corpus structurally present across on-chain Executable Proposal records, Snapshot IPFS records, on-chain treasury movements, Karpatkey Endowment reporting, Arweave-archived Small Grants submissions, Dune dashboards, and the Discourse forum
- Independent Verifiability at on-chain decision-making and disbursement layers
- Inter-cycle Reflection Stage structurally satisfied retroactively by the Metagov retrospective contract (Phase 1: 23 interviews, ~30 hours)
- Adverse Signal Engagement structurally present at the DAO-portfolio level via the Metagov retrospective and the concurrent restructuring temp checks
- Modularity Preservation: three Working Groups operating independently with separate multisigs and steward elections
- Format Agnosticism at the application layer (no required proposal template for Small Grants)
- Continuity Capacity supported by 12-month staggered steward elections rather than single-person dependency

### Partial alignments

- Format Agnosticism at the cross-track layer (variance in application content requirements across Small/Large/Strategic/Builder tracks)
- Independent Verifiability at the milestone verification layer (steward-internal review rather than independently re-derivable rubric)
- Beneficiary Validation Mechanism approximated through steward domain election but not per-grant validation
- Pre-Award Indicator Confirmation Stage approximated through milestone structure but not formalized as a stage

### Compatibility gaps requiring program adjustment for full conformance

- Grant track criteria should be published at CROSS Part VIII granularity for Strategic, Large, Builder, and discretionary tracks (current "usefulness and impact" formulation is narrative)
- Standing Adverse Signal Engagement discipline should replace the one-time Metagov retrospective contract (per-term adverse signal logs at each Working Group term close)
- Affected Population Verification Gate should be added at completion for Strategic and Large Grants whose declared public benefit mechanism is condition change or access provision
- Concurrent funding disclosure should be added to grantee profiles at CROSS Part II Dimension 4 specificity (currently the co-funding compatibility framing is informal, e.g., Vyper "$50,000 matched by Ethereum Foundation")
- Determination Body charter for the Working Group multisigs and the Foundation operations layer should be published at the body-composition-and-removal-mechanism specificity the primitive requires

### Structural compatibilities of historical interest

The ENS DAO Grants architecture sits between Gitcoin Grants and Arbitrum DAO Grants in the CROSS+WALKRI-mapped web3 corpus. Like Gitcoin Grants, ENS operates a community-voted micro-grant track (Small Grants) using token-weighted voting on Snapshot. Like Arbitrum DAO Grants, ENS operates a multi-track portfolio of programs with elected stewards making discretionary determinations within DAO-approved budget envelopes. Like both, ENS is constitutionally constrained (the ENS Constitution Article 3 sets the public goods funding rationale; the Arbitrum DAO operates under its own constitution; Gitcoin Foundation operates under a published 2025 strategy).

The Metagov-led retrospective is the closest analog in the web3 corpus to Arbitrum's ARDC assessment work. Both are independent third-party research outputs feeding adverse signals back into the program design. The structural opening is the same: a multi-cycle, multi-program DAO grants ecosystem produces enough data after several years of operation that a structured retrospective becomes possible. The Arbitrum ARDC was internal-research-collective; the ENS retrospective is an external Metagov contract. Both are structurally adjacent to a standing Inter-cycle Reflection Stage discipline; neither has yet become standing.

The in-progress restructuring temp checks (Coordination Layer, Working Group Restructure, Admin Panel) place ENS DAO at a structural inflection point. Whichever path the DAO chooses, the post-restructuring architecture will need to re-specify the Determination Body composition and the grant-track criteria. CROSS+WALKRI compatibility is preserved through the restructuring if the new architecture preserves the pre-commitment discipline (on-chain Executable Proposal as the binding instrument), the Determination Body Separation (whoever ends up making grant decisions is structurally separate from applicants), and the Attestation Corpus (treasury flows remain on-chain and forum records remain publicly accessible).

## Calibration Tier Assessment

ENS DAO Grants 2024-2026 sits at a mixed calibration tier in the CROSS+WALKRI Lenses Framework:

- **Tier 3 (Outcome Specified, Self-Reported)** at the Large Grants milestone-tied disbursement layer for grantees with named deliverables and milestone review by stewards
- **Tier 2 (Process Conformant)** at the decision-making layer (Discourse-to-Snapshot-to-Executable flow is publicly documented and conforms to its own published process; the Constitution is ratified and amended only through its own published procedure)
- **Tier 1 (Impressionistic)** at the Strategic Grants, Builder Grants, and discretionary bounty layers where steward judgment operates against narrative criteria; also at the Small Grants outcome-interpretation layer where the Snapshot tally itself is the determination without an outcome-evidence requirement

Aggregating, the program operates at Tier 2 (Process Conformant) overall, with elements at Tier 1 and Tier 3. The in-progress Metagov retrospective points toward Tier 4 trajectory through formal independent evaluation of past delivery.

**Current+target trajectory:**

- Current: Tier 2 aggregate as described above
- Next achievable target (within current architecture, post-Metagov retrospective publication and post-restructuring): Tier 3 across all major grant tracks via published criteria for Strategic and Large Grants and structured completion-stage evidence
- Long-range target (within 2-3 years if Metagov recommendations are adopted as standing discipline): Tier 4 (Independently Verified) via standing Inter-cycle Reflection Stage publications per term, formal Determination Body charter for the post-restructuring decision-making body, and independent verification of completion outcomes for Strategic Grants

## Mapping Table

| ENS DAO Grants Element | CROSS Provision | WALKRI Provision |
| :-- | :-- | :-- |
| Discourse forum proposal publication | Entry specification gate (criteria fixed before applications) | Pre-publication field requirements |
| Snapshot Social Proposal voting | Pre-commitment as structural posture; Independent Verifiability via IPFS-stored votes | Integrity standard (5.2): evidence independent of applicant |
| On-chain Executable Proposal voting at vote.ensdao.org | Pre-commitment as structural posture; Independent Verifiability at on-chain voting layer | Integrity standard (5.2) |
| 2-day timelock before execution | Adverse Signal Engagement Principle structurally supported (community can flag issues before execution) | Not applicable at field level |
| Tenderly simulation before Executable Proposal submission | Independent Verifiability at the pre-execution simulation layer | Evidence form for code execution |
| Working Group steward elections (12-month terms) | Determination Body Separation at the vertical layer; Continuity Capacity at the decision-making body | Not applicable at field level |
| 3-of-4 Working Group multisig | Disbursement Authority (Layer 2: collective type) | Not applicable at field level |
| ENS Foundation Cayman Islands wrapper | Disbursement Authority structural anchor; Funder-Side Obligation Architecture | Not applicable at field level |
| Constitution Article 3 (Treasury Allocation) | External Standard Identifier (the Constitution is the named declared rule); Format Agnosticism content-vs-format anchor | Conformance threshold (5.0): the constitutional condition |
| Strategic Grants up to 150k USDC | Mixed obligation mode (Build + Change for population-anchored work) | Gap: criterion specification not at CROSS Part VIII granularity |
| Large Grants up to 50k USDC with milestone-tied disbursement | Progress Verification Gate configurations | Evidence form for milestone verification (steward-internal) |
| Small Grants token-weighted quarterly Snapshot vote | Determination Body Separation at the allocation layer (token holders are the determinator) | Evidence form: Snapshot vote tally at IPFS access path |
| Builder Grants at hackathons | Build obligation at small scale; Coordination Scaling Standard | Not applicable at field level |
| Karpatkey Endowment quarterly forum reviews | Attestation Corpus structurally present; Inter-cycle Reflection Stage at the treasury layer | Evidence form with forum URL access path |
| ensgrants.xyz Arweave-archived submissions | Attestation Corpus structurally present | Evidence form with Arweave hash access path |
| Metagov retrospective (in-progress) | Inter-cycle Reflection Stage (retroactive); Adverse Signal Engagement Principle structurally aligned | Pre-publication audit pattern |
| Restructuring temp checks (Coordination Layer, Admin Panel) | Structural opening for Determination Body charter publication post-restructuring | Not applicable at field level |
| No published per-grant criterion rubric | Gap: CROSS Part VIII criterion specification absent for steward-discretionary tracks | Gap: criterion specification elements absent |
| No standing Inter-cycle Reflection Stage | Gap: Metagov retrospective is a one-time contract, not a continuing discipline | Gap: pre-commitment to inter-cycle publication absent |

## Pre-Funding Specification Layer

A CROSS+WALKRI-conformant ENS DAO Grants term produces something the current architecture approximates at the decision-making layer but does not formalize at the grant-track layer: a pre-funding specification layer that publishes (per term, per Working Group, per grant track) the Determination Body charter, the criterion intent for each track, the operational definition of "usefulness and impact," the milestone evidence form specifications, the Adverse Signal Engagement plan, and the Inter-cycle Reflection Stage commitment. The Metagov retrospective effectively prescribes parts of this specification layer through its synthesis of "main governance challenges and systemic patterns" (the Phase 1 framing); full conformance requires the retrospective findings to move from research output to standing discipline at the term level.

The post-restructuring architecture (whichever of Coordination Layer, Working Group Restructure, or Admin Panel paths the DAO adopts) is an opportunity to specify this layer rather than inheriting the current narrative-criteria pattern. Pre-Funding Specification Layer publication is the structural counterpart to the Falsifiability commitment, applied at the term-configuration layer.

## Compatibility Statement Maturity

This is a Tier 2 compatibility statement under the CROSS+WALKRI primitives framework index: the source framework is a structurally significant exemplar of a multi-track DAO grants ecosystem with elected Working Group stewards, a published Constitution, and an in-progress independent retrospective evaluation. It warrants a full statement rather than a Tier 2 index entry.

The statement will be revised as the Metagov retrospective Phases 2 and 3 publish, as the restructuring decisions (Coordination Layer, Working Group Restructure, or Admin Panel) resolve, and as the post-restructuring architecture matures. The structural inflection point ENS DAO is at in mid-2026 is itself analytically significant for the CROSS+WALKRI corpus: it documents what a DAO grants ecosystem looks like when it pauses to evaluate its own multi-year operation before continuing.

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

ENS Documentation: docs.ens.domains/dao

ENS DAO Basics: basics.ensdao.org

ENS DAO Governance Forum: discuss.ens.domains

ENS Small Grants: ensgrants.xyz

ENS On-chain Voting: vote.ensdao.org

ENS Snapshot Space: snapshot.org (search for ens.eth)

Metagov: metagov.org

License: CC0

## Changelog

- **0.1.1 (2026-06-08):** Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only.
- **0.1.0 (2026-05-23):** Initial compatibility statement covering the ENS DAO Grants ecosystem (2024-2026). Maps the Discourse-to-Snapshot-to-Executable decision-making flow, the three Working Groups (Public Goods, Ecosystem, Meta-Governance), the four Public Goods grant tracks (Strategic, Large, Small, Builder), the ENS Foundation Cayman wrapper, the Karpatkey Endowment treasury architecture, and the in-progress Metagov-led retrospective evaluation. Identifies strong alignments at pre-commitment (Discourse-to-Snapshot-to-Executable with 2-day timelock and Constitution as deeper pre-commitment), Determination Body Separation (macro DAO and steward election layers), Attestation Corpus (on-chain proposals and treasury, Snapshot IPFS, Arweave Small Grants, Karpatkey reviews, Discourse forum), Inter-cycle Reflection Stage (Metagov retrospective retroactively), Adverse Signal Engagement (Metagov plus concurrent restructuring temp checks), and Modularity Preservation (three independent Working Group multisigs). Identifies gaps at published criterion rubric (Strategic, Large, Builder, discretionary tracks operate against narrative criteria), standing Adverse Signal Engagement (one-time Metagov contract rather than continuing discipline), Affected Population Verification Gate (no formal completion-stage affected-population engagement), Determination Body charter publication (Working Group multisig and Foundation operations layer specificity), and Pre-Award Indicator Confirmation Stage (milestone structure substitutes for formal stage). Lens-tagged: Tier 2 aggregate with Tier 1 steward-discretion layer and Tier 3 milestone-tied Large Grants layer, Tier 4 trajectory via Metagov retrospective adoption as standing discipline; Voluntary Published authority; Western institutional with DAO decision-making hybrid lineage; DAO or protocol funder typology; Allocator process primary scope. Conforms to Primitives Foundation v0.1.7 (uses Continuity Capacity and Affected Population Verification Gate names per v0.1.7 rename).

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri. For the source framework, see docs.ens.domains/dao.*
