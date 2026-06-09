---
title: CROSS - Common Reporting Outcome Standards Schema - Worked Examples
version: 0.3.1
date: 2026-06-08
license: CC0
status: Working draft. Companion worked examples synced to CROSS-common-reporting-outcome-standards-schema-0_5_0.md. Supersedes version 0.2.0.
---

# CROSS - Common Reporting Outcome Standards Schema - Worked Examples

Version 0.3.1 | 2026-06-08 | CC0

---

## Changelog

**0.3.1 (2026-06-08).** Frame Language own-voice pass. Own-voice watchlist terms were replaced with the structural act each names (the six "What a Compliant Approach Would Have Looked Like" example headers became "Conformant"; the integrity standard became the data quality standard; "Partnership claim integrity" became "Partnership claim verification"; "attribution statement governs the evidential basis" became "covers"; own-voice beneficiary population became affected population). Real program names, quoted applicant material, the WALKRI Integrity dimension, the canonical Beneficiary Validation Mechanism, the Institutional Capacity dimension name, and the changelog rows were preserved. Em-dash sweep clean. No worked example or determination changed; vocabulary and naming only.

**0.3.0 (2026-06-05).** Synced to the 0.5.0 specification. Added seven worked examples (Cases 7 through 13) for requirements the specification introduced since the 0.2.0 baseline: organizational identity non-disclosure through serial rebranding and affiliated-entity omission (Case 7); sufficiency architecture incoherence where corroborating evidence contradicts the declared position (Case 8); public benefit mechanism and access condition mismatch where an all-rights-reserved copyright is claimed under an output production mechanism (Case 9); development stage mismatch where the declared stage is contradicted by the evidence (Case 10); obligation fulfillment non-disclosure where a discovered prior failure was not disclosed (Case 11); prior work attribution failure where a track record is built on work performed under a different entity (Case 12); and the served-population risk-bearer floor applied at the completion gate, with a determination record that does and one that does not show the served population's exposure was considered (Case 13). Existing Cases 1 through 6 are unchanged. Summary table and key distinctions extended to cover the new cases.

**0.2.0 (2026-05-14).** Six worked examples drawn from Octant Epoch 12 evaluations. Supersedes 0.1.0.

---

## Introduction

These examples illustrate CROSS criteria through real grant evaluation cases. Each case identifies the criterion illustrated, states the finding from evaluation, specifies the CROSS assessment, and shows what a conformant approach would have looked like. Cases are drawn from Octant Epoch 12 grant evaluations conducted in May 2026.

All six cases in this edition are drawn from rounds operating in change-obligation mode or from the boundary between build and change obligation. Cases illustrating build-obligation and retroactive obligation rounds will be added as examples from those program types are evaluated and documented. The entry specification gate findings in these cases use the change-obligation vocabulary (FROM state classification) unless otherwise noted.

Each case can be read independently. The recommendation vocabulary throughout is: Fund / Fund with conditions / Do not fund.

---

## Case 1: Beneficiary Validation Failure

**Project:** Mushee Allocate
**Ask:** \$6,330
**Outcome:** Do not fund
**Criterion Illustrated:** Coordinating party engagement and beneficiary validation; entry specification gate

### The Application

Mushee Allocate was proposed as a claim-and-allocation portal for Ethereum and Ethereum Virtual Machine-compatible chains. The stated workflow: a grant administrator creates a campaign, adds recipient wallet addresses, sets individual allocations, and publishes a claim page. Recipients visit the page, connect their wallet, and pull their tokens. The application framed the problem as grant distribution coordination requiring manual spreadsheets with no transparent on-chain record. The ask was \$6,330.

### The CROSS Finding

The FROM state named in the application is internally coherent: grant teams routinely distribute tokens in batches and the mechanics of moving tokens from a multisig to dozens of recipients is error-prone. A specific problem is visible. At that level, the entry specification gate passes: a condition is named in a defined operational context.

The application fails at the beneficiary validation dimension. Beneficiary validation requires that the FROM state be confirmed by parties outside the applicant's control, and that the applicant have named existing alternatives and explained why those alternatives do not address the stated population's specific need.

An independent check found that Hedgey Finance already addresses the stated problem: administrators upload a comma-separated values file of recipient addresses and allocations, Hedgey Finance generates a Merkle-tree-based claim, recipients connect a wallet and claim from a custom link, and a dashboard tracks participation rates and token volumes in real time. Hedgey Finance is deployed, audited, used by Arbitrum and other protocols, and free to use. Splits, Coordinape, and Drips Network fill adjacent parts of the same workflow.

The application did not name Hedgey Finance or any of these tools. This is a beneficiary validation failure in its most direct form: the applicant proposed a solution without first establishing that existing solutions do not serve the stated population. The FROM state exists as a claim but was not validated against the competitive landscape, and the tools that already fill the described gap are production-grade.

A second dimension failed: product readiness. The closest analogue to Mushee Allocate found in any public repository was ClaimFlowOS, committed in a single upload on April 12, 2026, two days after the Octant Epoch 12 application window opened. The repository's own README states: "This is a polished frontend demo with interactive mock workflows for product presentation, grant applications, and investor demos." The repository contains no smart contract code, no wallet connection logic, and no backend. The demo was produced to support the grant application rather than to represent genuine product progress. No Ethereum testnet deployment was found, no smart contract exists in any public repository, and the Mushee Allocate domain was unreachable at time of evaluation.

### CROSS Assessment

Entry specification gate: passes (a specific condition is named in a defined context).

Beneficiary validation: fails. The FROM state was not validated with intended beneficiaries and the applicant did not name existing alternatives, which is a required step under the coordinating party engagement and beneficiary validation dimension.

Product readiness: the single-commit demo explicitly self-described as built for grant applications does not constitute evidence of a working product. This is an institutional capacity finding, not a gate finding, but it reinforces the do not fund recommendation.

### What a Conformant Approach Would Have Looked Like

A conformant application would have named Hedgey Finance, Splits, and Coordinape, explained specifically why each does not address the applicant's stated population's need, and cited at least one source outside the applicant's control confirming that a gap remains. For example: evaluation results from grant programs using Hedgey Finance identifying specific limitations, interviews with grant administrators conducted before writing the application, or documentation of a problem that Hedgey Finance's architecture cannot accommodate.

The conformant application would then have specified what Mushee Allocate does that Hedgey Finance cannot, in the same operational terms used to describe the FROM state. If no such differentiation exists, the gap does not exist and the application should not proceed.

---

## Case 2: Indicator Specification Failure

**Project:** mev-commit (Primev)
**Ask:** \$100,000
**Outcome:** Do not fund
**Criterion Illustrated:** Operational definition; Integrity

### The Application

mev-commit is a peer-to-peer network where block builders on Ethereum issue cryptoeconomic commitments ("preconfirmations") before a block is proposed. When a builder commits to including a transaction in the next block, the commitment is backed by slashable stake: if the builder breaks it, they lose collateral. Validators opt into this system by agreeing to accept only blocks from mev-commit builders. The protocol is live on Ethereum mainnet with 7,835 opted-in validators and \$116.5M in economic security across Symbiotic vaults. The application asked for \$100,000 toward an encrypted mempool milestone using the LUCID design and Shutter Network cryptography. The application's headline block coverage claim was "10-20% of Ethereum blocks."

### The CROSS Finding

The headline outcome indicator, "10-20% of Ethereum blocks," is an indicator name, not an operational definition. The claim does not specify which blocks count (mainnet only? testnets? any time window?), the measurement methodology, how partial inclusion is handled, or what data source an independent reviewer would use to replicate the figure.

An independent check using MEV-Boost relay data and a September 2025 research paper showed: single-day peak block coverage of 11.33% on August 20, 2025; a 5% sustained 24-hour figure documented in that period; and a February 2026 Dune dashboard showing 3.13% block value captured. The application presents "10-20%" as the current state of coverage; it is a cherry-picked range anchored to a single-day peak from nine months before the application date. Sustained coverage at time of application was 3-5%. The claim overstates current coverage by a factor of 3-6x.

This is an indicator specification failure under two sub-requirements. First, no operational definition exists: the indicator as stated does not meet the CROSS requirement for inclusion criteria, exclusion criteria, unit of analysis, or edge case determination. Second, no construction and aggregation methodology was provided: there is no named data source, no time window, and no replication path for an independent reviewer.

The integrity dimension also fails. All performance metrics in the application are sourced from applicant-controlled systems: the Primev validator dashboard, the Primev documentation, and the KarmaGAP profile created the same day as the application. No named independent corroboration was provided for the headline coverage claim. For a claim of this magnitude in a live infrastructure context, applicant-controlled data without independent corroboration does not satisfy the data quality standard.

A third legibility failure reinforces the finding: venture capital backing from a16z CSX, HashKey Capital, and Figment Capital was not disclosed in the application, despite concurrent funding disclosure being a required field for all CROSS-conformant applications.

### CROSS Assessment

Indicator specification: fails. The headline indicator is a name without an operational definition, a construction methodology, or a replication path.

Integrity: fails. All performance evidence is sourced from applicant-controlled systems. The independent data that exists contradicts the headline claim.

Concurrent funding disclosure: incomplete. Venture capital backing from named investors was not disclosed.

Entry specification gate: passes on the encrypted mempool milestone specifically (the FROM state for that milestone is that Ethereum's pre-consensus layer lacks a privacy-preserving transaction ordering mechanism, which is a specific, verifiable condition). The gate failure is not at the entry specification level; it is at the indicator specification and integrity levels, which are rigor-tier concerns.

### What a Conformant Operational Definition Would Have Looked Like

A conformant operational definition for the "blocks" indicator would specify:

Indicator name: Proportion of Ethereum mainnet blocks per calendar week with at least one mev-commit preconfirmation included.

Inclusion criteria: a block counts if it was proposed on Ethereum mainnet (chain ID 1) in the specified time window and contains at least one transaction whose inclusion was secured through a verified mev-commit preconfirmation commitment, as evidenced by a slashing record in the mev-commit settlement chain (chain ID 8855).

Exclusion criteria: testnet blocks, Ethereum testnets, blocks on other Ethereum Virtual Machine chains, and blocks containing transactions routed through mev-commit relays but without a recorded commitment are excluded.

Unit of analysis: individual Ethereum mainnet block.

Construction methodology: weekly block count sourced from a named public MEV-Boost relay data application programming interface (such as Relayscan or MEV-Boost.org), with preconfirmation matches verified against the mev-commit settlement chain. The data source and query are named so an independent reviewer can replicate them.

Baseline: as of February 2026, 3.13% of weekly Ethereum mainnet block value captured (source: named Dune dashboard uniform resource locator, accessed date).

Target: 10% of weekly Ethereum mainnet blocks with at least one preconfirmation by end of grant period.

Time window: 12-week rolling average at the time of each milestone report.

---

## Case 3: Privacy-Sensitive Context Accommodation

**Project:** MoaV (Mother of All VPNs)
**Ask:** \$30,000
**Outcome:** Fund with conditions
**Criterion Illustrated:** Privacy and data sensitivity accommodation

### The Application

MoaV is a self-hosted censorship circumvention stack that deploys 16 or more distinct anti-censorship protocols from a single Docker Compose command. A server operator runs one installation script and the stack comes up with protocols spanning fundamentally different technical approaches: stealth Transport Layer Security proxies, QUIC-based tunneling, WireGuard variants, Domain Name System tunneling, content delivery network-fronted routing, and Telegram MTProxy. The protocol diversity is the core design argument: no single protocol survives every censorship environment. The project integrates with MahsaNet, which distributes operator-donated configurations to approximately 2 million users in Iran, Russia, and Myanmar. MoaV was built by Shayan Eskandari, a former ConsenSys Diligence security engineer with a 32-audit career in Ethereum smart contract security. The project launched January 28, 2026, weeks after Iran's January 8 shutdown.

### The CROSS Finding

MoaV ships with zero telemetry by design. This is the correct architectural choice for a tool serving users in high-risk jurisdictions: any telemetry collection that identifies user location, usage patterns, or protocol preferences creates data that an adversary could use to surveil, identify, or arrest the people the tool exists to protect. The absence of telemetry is a safety property, not a reporting gap.

Standard outcome measurement requirements for a public goods grant would typically ask for user counts, geographic breakdown, and usage frequency. Applied to MoaV without modification, these requirements would create a harm: satisfying them would require collecting the same data that, if obtained by Iranian or Russian authorities, would expose users to adversarial surveillance, detention, or worse.

CROSS specifies that when standard measurement would compromise the safety of the affected population, privacy-preserving measurement methodologies are required in lieu of standard analytics. The accommodation is not an exemption from obligation; it requires specifying which obligation mechanisms are appropriate to the context.

The application partially addressed this: the zero-telemetry design is documented, the privacy rationale is implicit in the tool's architecture, and the Digital Public Goods Standard self-assessment correctly identifies telemetry absence as a design property rather than a gap. However, the application did not formally invoke the privacy-sensitive accommodation. It did not name the specific harm that standard measurement would create, did not name the alternative methodology that would be used instead, and did not identify an institutional partner who could validate the alternative methodology through an ethics-reviewed process.

The evaluation recommends funding with conditions, including that the applicant name the specific measurement harm and specify the alternative methodology before disbursement.

### CROSS Assessment

Privacy-sensitive accommodation: invoked implicitly through architectural design but not formally declared. The invocation is incomplete because it names the design property (zero telemetry) but not the harm avoided by that design, and names no alternative measurement methodology.

Entry specification gate: passes. The FROM state is specific and externally verifiable: Open Observatory of Network Interference probe data and multiple independent sources document that Iranian internet connectivity dropped to 1-4% of normal levels during February-March 2026. A specific measurable condition in a defined population exists.

Institutional capacity: mixed. The founder's background is directly relevant; the solo contributor structure and absence of independent security review are the primary risks.

### What a Conformant Accommodation Request Would Have Looked Like

A conformant formal invocation of the privacy-sensitive accommodation would do four things.

First, it would name the specific harm. "Standard outcome measurement for this grant would require collecting data on the number, geographic distribution, and usage patterns of users in Iran, Russia, and Myanmar. This data, if obtained by authorities in those jurisdictions through server seizure, subpoena of a hosting provider, or interception, would identify individuals who circumvented government-imposed internet restrictions. This constitutes a direct physical safety risk to the affected population."

Second, it would name the alternative methodology. For example: "Impact will be assessed through aggregate, non-attributable measurement using Open Observatory of Network Interference probe data to confirm that the protocols MoaV deploys remain unblocked in the relevant networks. This is the same methodology used by Tor Project and Psiphon to assess protocol effectiveness without exposing users. The methodology produces a binary indicator (protocol reachable or not) rather than a user count. An ethics-reviewed study with a named institutional partner, such as the Citizen Lab at the University of Toronto or the Open Observatory of Network Interference, will be pursued during the grant period to provide independent validation."

Third, it would name the specific measurement harm the alternative avoids: user identification, location attribution, and usage fingerprinting.

Fourth, it would commit to at minimum one piece of independent validation that does not require user identification: a GitHub release changelog confirming protocol updates in response to documented blocking events, with timestamps cross-referenceable to Open Observatory of Network Interference measurement data showing those events.

---

## Case 4: Concurrent Funding Disclosure Failure

**Project:** The Interfold (formerly Enclave)
**Ask:** \$100,000
**Outcome:** Fund with conditions
**Criterion Illustrated:** Concurrent funding disclosure; Adverse signal disclosure

### The Application

The Interfold is a protocol and distributed network that uses threshold Fully Homomorphic Encryption to compute over encrypted inputs and produce publicly verifiable outputs, without any single operator ever seeing the raw data. The cryptographic work is technically serious: BFV encryption allows arithmetic operations over ciphertexts; a threshold committee of independent nodes generates a joint key through Publicly Verifiable Secret Sharing; computation happens over encrypted inputs; outputs are decrypted only when a threshold of nodes cooperate; and recursive proof aggregation lets the final state be verified by a single proof on Ethereum. The project was previously known as Enclave, rebranded in March 2026. The ask of \$100,000 was directed primarily at an external security audit (approximately \$70,000) with the remainder as runway while the audit proceeds. The application listed Session and Taiko as organizations that had committed to using the protocol.

### The CROSS Finding

The application did not disclose a \$1M venture capital round recorded in KarmaGAP. It did not disclose a \$3.82M GnosisDAO treasury allocation under Gnosis Improvement Proposal 78, which covered the Gnosis Guild guild-wide operations including the Enclave project. It did not disclose a Zcash Community Grant application for \$130,000 for a CRISP-based coordinating instrument called Zecret Ballots, which was rejected by the Zcash Community Grants committee in April 2026, approximately one month before this application.

These are three independent disclosure failures under CROSS's concurrent funding disclosure requirement. The venture capital round and the GnosisDAO allocation together represent more than \$4.8M in related prior funding, none of which appeared in the application. The Zcash rejection is an adverse signal for a closely related CRISP application in an adjacent ecosystem, which must be disclosed under the Adverse-Signal Engagement Principle.

The application also misrepresented two claimed partnerships. The application stated that Session had "committed to using the protocol for aggregated user analytics." No Session-side corroboration exists: Session's blog post on user analytics makes no mention of The Interfold, fully homomorphic encryption, or any privacy-preserving analytics integration. The only evidence of a relationship is a co-marketing X Space appearance, which is not a technical commitment. The application stated that Taiko had "committed to using CRISP for program decisions on their existing Aragon mainnet instance." The Interfold's own blog post on the Taiko collaboration uses entirely aspirational language ("can be deployed," "can operate," "can rely on"), and CRISP is not named in the Taiko collaboration post. No Taiko-side publication confirms a commitment to deploy.

The core protocol work is genuine. The cryptographic implementation is real: Sepolia deployments are confirmed, 90% of protocol circuits were complete as of April 2026, and the Aragon integration is corroborated from Aragon's side. The disclosure failures are process failures, not fabrications about the technology itself.

### CROSS Assessment

Concurrent funding disclosure: incomplete. The \$1M venture capital round and the GnosisDAO Gnosis Improvement Proposal 78 allocation are both related to the scope of the application and both fall within the 24-month disclosure window. Neither appears in the application.

Adverse signal disclosure: incomplete. The April 2026 Zcash Community Grant rejection for Zecret Ballots, a CRISP-based coordinating instrument closely related to the application's scope, was not disclosed.

Partnership claim verification: two claimed commitments (Session and Taiko) are contradicted by the available evidence. This is a rigor-tier finding rather than a gate failure; the gate passes on the strength of the Aragon integration and the cryptographic work. But the two uncorroborated "commitment" claims constitute material misrepresentation that must be corrected before disbursement.

Recommendation: Fund with conditions, not Do not fund, because the disclosure failures are addressable and the underlying work is real. But no disbursement occurs until all four concurrent funding sources are disclosed, the Zcash rejection is disclosed with explanation, and written confirmation from Session and Taiko replaces the uncorroborated "commitment" language.

### What Conformant Disclosure Would Have Looked Like

A conformant application would have listed in the concurrent funding disclosure field:

(1) Venture capital round: approximately \$1,000,000, investor not publicly named, closed prior to this application, no program decision rights over the protocol granted to investors. Relationship to this application: this funded the engineering work that produced the protocol now seeking audit funding.

(2) GnosisDAO Gnosis Improvement Proposal 78 allocation: approximately \$3,820,000 to Gnosis Guild operations guild-wide, covering Zodiac, Enclave, and other tooling. Portion attributable to Enclave/The Interfold is approximately [amount]. Relationship to this application: prior operating funding that has been substantially deployed; current request is for audit funding not covered by prior allocations.

(3) Zcash Community Grant: \$130,000 requested for Zecret Ballots, a CRISP-based secret ballot application for the Zcash ecosystem. Rejected by Zcash Community Grants committee, April 2026. Rejection rationale as provided by the committee: [summary]. Relationship to this application: the CRISP protocol being evaluated here is the same protocol proposed for Zecret Ballots. The rejection did not concern protocol soundness but [specific rationale].

With these disclosures complete, the evaluation would have proceeded directly to assessing whether the audit ask is appropriately scoped and whether the partnership claims are adequately corroborated, rather than surfacing the omissions through independent research.

---

## Case 5: Well-Specified Application with Hard Gates

**Project:** Gean (Go Lean Ethereum Consensus Client)
**Ask:** \$30,000
**Outcome:** Fund with conditions
**Criterion Illustrated:** Entry specification gate passage; Institutional capacity; Conditional funding

### The Application

Gean is a Go implementation of the Lean Ethereum consensus client, targeting the Lean Consensus devnet infrastructure initiated by Ethereum Foundation researcher Justin Drake. The Lean Ethereum initiative, announced July 2025, proposes replacing Bonnet-Lynn-Shacham signatures with hash-based post-quantum signatures and compressing thousands of signatures into a single short proof via a recursive zero-knowledge virtual machine. A new consensus client implementation is the primary way teams contribute to this initiative's interoperability goals. Gean is the only Go client in the ecosystem; the other implementations are Rust, Zig, C++, C, and Rust fork variants. The project is MIT-licensed, targets Go 1.25+, passes 49 current leanSpec test fixtures, and integrates with the lean-quickstart multi-client devnet tooling. The \$30,000 ask covers approximately 6-8 months of additional runway, expanded contributor capacity, and continuous integration infrastructure. The application references an Ethereum Foundation Ecosystem Support Program grant identified as FY26-2432.

### The CROSS Finding

The entry specification gate passes on this application, and passes clearly. The FROM state is specific and externally verifiable: the Ethereum network has effectively zero production Go execution clients other than the reference client (go-ethereum/geth) following the deprecation of prior clients; the post-quantum Lean Ethereum initiative requires multiple independent consensus client implementations to achieve the interoperability testing that prevents a monoculture risk; and Go is underrepresented in the current Lean Ethereum client landscape (Rust, Zig, C++, C are all represented; Go is not). This condition is named in Ethereum ecosystem research and in the Lean Ethereum initiative documentation, not only in the applicant's own materials.

The evaluation confirmed: 344 commits on the main branch with activity through April 2026; 49 passing leanSpec spec fixtures; active devnet-4 migration work (Issue 208, filed April 12, 2026); inclusion in the lean-quickstart multi-client devnet tool alongside 9 other implementations; and leanroadmap.org listing of Gean as the Go implementation.

Two hard gate conditions apply before disbursement.

The first is the Ethereum Foundation Ecosystem Support Program grant FY26-2432. The grant identifier appears in Gean's own KarmaGAP profile and nowhere else in any searchable public source. The Ethereum Foundation Q1 2026 and Q4 2025 allocation reports do not name Gean individually. The KarmaGAP profile recording the grant was created on the same day as this evaluation. This is consistent with how the Ethereum Foundation handles individual Ecosystem Support Program grants (grant identifiers are not published in allocation reports), but it means the only external validation of the grant is the applicant's own filing. One email to grants-admin@ethereum.org resolves this, but it must happen before any funds move.

The second is devnet participation. Gean is listed in the lean-quickstart tool but does not appear in the pq-devnet-3 planning document or in the two most recent post-quantum Interop meeting notes (numbers 36 and 37), which name Ream, Zeam, Qlean, Lantern, and Lighthouse as the active cross-client participants. Whether Gean is running nodes in official Ethereum Foundation-coordinated cross-client devnets or only in the lean-quickstart local environment is a meaningful distinction for the milestone assessment. Direct confirmation from Thomas Coratger (the facilitator of the weekly post-quantum Interop calls at the Ethereum Foundation) resolves this.

### CROSS Assessment

Entry specification gate: passes. The FROM state is specific, externally corroborated, and names a real gap.

Institutional capacity: mixed. The project has a genuine development track record (344 commits, 49 passing fixtures, active devnet migration), a named Ethereum Foundation funding relationship, and multiple named contributors. The lead active contributor (dimka90) has no independently verifiable public profile beyond the GitHub username, which is a legibility gap for a three-person team. The legal status discrepancy (the application claims registered organization; the KarmaGAP profile describes an unincorporated working group) should be resolved.

Conditional funding: how it works in CROSS. The conditions are specific, verifiable, and time-bounded. Each has a named verification method: the Ethereum Foundation grant is confirmed by emailing grants-admin@ethereum.org; devnet participation is confirmed by contacting Thomas Coratger at thomas.coratger@ethereum.org. Both are verifiable within days, not months. If either check fails, the recommendation changes to Do not fund. This is the structure of conditional funding under CROSS: conditions are not aspirational guidance; they are binary gates with named verification paths that must be cleared before disbursement.

### What the Conditional Funding Structure Demonstrates

This case illustrates the distinction between a project that passes the entry specification gate and a project that is ready for unconditional disbursement. Gean passes the gate; the FROM state is real, the work is real, and the public goods character is unambiguous. The conditions exist not because the project is weak but because two specific factual claims (the Ethereum Foundation grant and the devnet participation) cannot be verified from public sources alone. The conditions protect the funder without punishing the applicant: if the claims are true, both conditions clear in less than a week.

---

## Case 6: Conditional Funding with Security Disclosure Requirement

**Project:** poidh ("pics or it didn't happen")
**Ask:** \$20,000
**Outcome:** Fund with conditions
**Criterion Illustrated:** Adverse signal disclosure; Conditional funding

### The Application

poidh is an open-source, non-custodial, immutable bounty protocol deployed across Arbitrum, Base, and Degen Chain. Anyone can post a bounty, anyone can add funds to it, and anyone can claim it by submitting photo, video, or text proof minted as a non-fungible token. When the bounty creator selects a winning claim, contributors vote to approve or veto based on their proportional stake. Smart contracts handle escrow and automatic payout on approval. There is no coordinating token and no central treasury. The protocol charges a 2.5% fee on completed bounties. In September 2025, a crowdsourced poidh bounty of approximately 10 million DEGEN tokens (worth \$28,000-\$35,000 at peak) funded a successful attempt to break the Guinness World Record for most kickflips in one minute, independently corroborated by Decrypt and video documentation. The v3 contract is deployed at a consistent address across Arbitrum and Base. The \$20,000 ask, the smallest in this evaluation cycle, covers resumed development and promotional public goods bounties.

### The CROSS Finding

The application did not disclose a v2 protocol exploit that occurred on December 8, 2025. The v3 internal security report documents two reentrancy vulnerabilities that were exploited: a claim acceptance reentrancy, where safeTransfer callbacks invoked onERC721Received before bounty state was finalized, allowing re-entry while balances remained nonzero; and a refund-loop reentrancy, where Ether was pushed to participants via call{value} loops while participant accounting was not finalized, enabling double-refund attacks. The v3 rebuild addresses both through ReentrancyGuard, strict Checks-Effects-Interactions patterns, and pull-based payments. The amount drained in the exploit has not been publicly disclosed.

The application mentioned the exploit only as an explanation for where a prior Base Builder Grant was spent on the rebuild. It did not name the exploit date, the exploit vectors, the amount drained, whether affected users were compensated, or how the Base Builder Grant was spent on remediation. This is an incomplete adverse signal disclosure under the Adverse-Signal Engagement Principle.

A separate safety issue is the beginner guide at words.poidh.xyz/poidh-beginner-guide, last updated August 2024. At time of evaluation, the guide still listed the old v2 contract addresses on Arbitrum, Base, and Degen Chain. These are the addresses from the exploited version. A user following the guide would interact with the compromised v2 contracts. This is a live documentation safety hazard for protocol users.

The protocol's merits are genuine and independently corroborated. The Guinness World Record attempt is documented in third-party press. The public goods bounties album shows completed real-world civic actions globally: road mark repairs, community garden documentation, utility hazard reporting, public space cleanup. The 30 GitHub contributors and 1,966 commits reflect a real development community. The v3 fix is technically appropriate.

Under the Adverse-Signal Engagement Principle Core Standard, an adverse signal that can be disclosed and addressed is not automatically a disqualifier. The question is whether the conditions are addressable. They are.

### CROSS Assessment

Adverse signal disclosure: incomplete. The v2 exploit was referenced but not disclosed. Required disclosures include the date (December 8, 2025), the exploit vectors, the approximate funds at risk, whether affected users were made whole, and how the Base Builder Grant was spent on the rebuild.

Safety condition: the beginner guide still references exploited v2 contract addresses, creating a live hazard for users who follow it. This is not an adverse signal issue; it is a separate condition requiring documentation correction before disbursement.

Entry specification gate: passes. The FROM state for a deployed bounty protocol is specific and verifiable: existing onchain bounty coordination lacks a non-custodial, proof-verified mechanism where funders and claimants can coordinate without trusting a single operator.

Recommendation: Fund with conditions because the protocol's merits are real, the ask is modest, the conditions are addressable within days, and adverse signal disclosure failure with a clear remedy is a process error, not a disqualifier.

### What a Conformant Adverse Signal Disclosure Would Have Looked Like

The concurrent funding and adverse signal section of the application should have contained an entry along the following lines:

"On December 8, 2025, the v2 poidh contracts on Arbitrum and Base were exploited via two reentrancy vulnerabilities: claim acceptance reentrancy and refund-loop reentrancy. Approximately [amount] was drained. Affected users [were / were not] compensated [explain approach]. The Base Builder Grant of approximately \$15,000 received in November 2025 was directed entirely to the v3 rebuild, which addresses both vulnerabilities through ReentrancyGuard, Checks-Effects-Interactions patterns, and pull-based payment mechanics. The v3 contracts were deployed in January 2026. The v2 contracts remain deployed but are no longer promoted by the team. The beginner guide requires updating to remove v2 contract addresses."

This disclosure does not eliminate the grant application's eligibility. It demonstrates that the team understands what happened, what was done to address it, and what remains to be done. That is the information the committee needs to make a sound funding decision.

### The Conditions Before Disbursement

Under CROSS conditional funding, the conditions are:

Written disclosure of the v2 exploit by the applicant, including the date, the vectors, the approximate funds at risk, whether affected users were made whole, and the basis for the Base Builder Grant allocation. This replaces the incomplete reference in the application.

The beginner guide at words.poidh.xyz/poidh-beginner-guide must be updated to replace the v2 contract addresses with the correct v3 addresses before the allocation window opens.

KarmaGAP registration with specific milestones mapped to the stated development deliverables.

The embedded wallet milestone language must be revised to reflect the v3 contract's externally owned account constraint (the msg.sender == tx.origin requirement), which blocks standard ERC-4337 account abstraction wallets, or the applicant must explain how they intend to resolve that architectural conflict before disbursing funds toward that milestone.

At \$20,000 with clear, time-bounded, binary conditions, this is a high cost-effectiveness grant for a real deployed protocol with documented public goods impact.

---

## Case 7: Organizational Identity Non-Disclosure

**Project:** Cohort Signal (formerly QuadVote, formerly SignalDAO)
**Ask:** \$45,000
**Outcome:** Do not fund
**Criterion Illustrated:** Organizational identity declaration; entry specification gate (pre-condition for assessment)

### The Application

Cohort Signal was proposed as a coordination-signal aggregation tool that collects community sentiment across forum threads, on-chain proposal records, and snapshot votes, then produces a weighted signal score that funders can use to gauge community alignment with a proposal. The application presented Cohort Signal as a new project launched in March 2026, listed a single named contributor, and stated under the prior round history field that the applicant had no prior history with this program. The legal entity name field listed "Cohort Signal" with no jurisdiction. The ask was \$45,000 for a six-month build.

### The CROSS Finding

The organizational identity declaration is a pre-condition for gate assessment, not a scored criterion. An entry gate submission that does not include a complete and truthful declaration is incomplete and is not assessed until the declaration is provided. Two fields in this submission were not truthful, and both are conformance failures rather than scoring deductions.

The prior round history field catches serial rebranding: an applicant who received a prior rejection and returns under a different name claiming no prior history with the program. The Attestation Corpus query against the on-chain identity anchor returned a disbursement-authority wallet address that matched the address listed in two prior submissions to this same program. The first, under the name SignalDAO, was submitted in a round eleven months earlier and rejected at the entry specification gate for an unspecified FROM state. The second, under the name QuadVote, was withdrawn after a reviewer requested the organizational identity declaration that the program had begun requiring. The current submission is the same wallet, the same single contributor, and substantially the same coordination-signal tool, presented as a first-time applicant. The "no prior history" entry in the prior round history field is contradicted by the program's own signed gate records.

The affiliated entity field was also incomplete. The named contributor holds a funded core-contributor role in a separate organization, Quorum Labs, that shares the contributor and a portion of the codebase with Cohort Signal and was itself an applicant in the same round under its own name. The affiliated entity field exists to surface exactly this: personnel overlap where a key team member holds a funded role in another organization applying to the same round. The field was left blank. The Cohort Position assessment for the round independently surfaced the personnel and wallet overlap between the two applications, confirming the omission.

Disclosure of either fact would not have disqualified the application. Non-disclosure of a publicly documentable affiliation is a conformance failure, and non-disclosure of prior round history that the program's own records contradict is treated more seriously than the prior rejection itself.

### CROSS Assessment

Organizational identity declaration: incomplete and contradicted. The prior round history field falsely declares no prior history; the program's own signed gate records show two prior submissions under different names from the same wallet. The affiliated entity field omits a documented personnel and codebase overlap with Quorum Labs, a separate applicant in the same round.

Entry specification gate: not reached. Because the organizational identity declaration is a pre-condition for assessment, the gate is not assessed on its merits. The submission is incomplete, and the non-disclosure converts an incomplete declaration into a material discrepancy under the adverse signal provisions of Part IV.

Cohort Position assessment: confirms the wallet and personnel overlap independently of the applicant's disclosure. Wallet overlap across distinct named entities applying separately is a material discrepancy requiring reconciliation before any disbursement.

Recommendation: Do not fund. The finding is not that the coordination-signal tool lacks merit; it is that the applicant's identity was misrepresented in a field specifically designed to catch serial rebranding, and the misrepresentation was confirmed against the program's own records.

### What a Conformant Declaration Would Have Looked Like

A conformant prior round history field would have read: "This project applied to this program in a prior round under the name SignalDAO (rejected at entry for an unspecified FROM state) and under the name QuadVote (withdrawn). The same disbursement-authority wallet was used in both. The tool has been substantially revised since: [specific changes]. The current submission addresses the prior FROM state deficiency by [specific diagnosis]."

A conformant affiliated entity field would have read: "The named contributor holds a funded core-contributor role at Quorum Labs, which shares this contributor and a portion of the signal-aggregation codebase with Cohort Signal. Quorum Labs is a separate applicant in this round under its own name. The two applications cover distinct scopes: [delineation]."

With both disclosures present, the evaluation would have proceeded to assess the revised tool on its merits, and the Cohort Position assessment would have confirmed rather than discovered the overlap. Disclosure is the difference between a surfaced relationship the committee can weigh and a discovered misrepresentation that bars assessment.

---

## Case 8: Sufficiency Architecture Incoherence

**Project:** Lattice Grants Registry
**Ask:** \$80,000
**Outcome:** Do not fund
**Criterion Illustrated:** Sufficiency architecture declaration; corroborating evidence consistency

### The Application

Lattice Grants Registry was proposed as an open registry that indexes grant programs across web3 ecosystems and exposes a public application programming interface for querying open funding rounds. The applying entity declared its scope as the registry's data-ingestion pipeline and declared a sufficiency position of critical gap: resources cover less than half of full scope requirements, and the program's viability depends on closing this gap. The grant contribution statement asserted that the \$80,000 would move the registry from critical gap to partial sufficiency on the ingestion pipeline. The application listed a public Open Collective as the entity's treasury.

### The CROSS Finding

The sufficiency position declaration requires at least one piece of corroborating evidence from a source outside the applicant's control, and the corroborating evidence provides the factual basis against which the declared position is assessed. The failure here is not an absence of evidence. It is that the evidence the applicant themselves named contradicts the position they declared.

The declared position is critical gap, which is defined as resources covering less than half of full scope requirements. The corroborating evidence offered was the applicant's public Open Collective balance and their KarmaGAP grant history. The Open Collective balance at the time of evaluation was approximately \$210,000. The KarmaGAP record showed three active grants for the registry totaling approximately \$190,000 disbursed in the prior nine months, all attributed to the same ingestion-pipeline scope the application declares. The applicant's own stated full-scope requirement for the ingestion pipeline, given elsewhere in the application, was approximately \$120,000 per year.

A treasury balance of \$210,000 against a stated annual scope requirement of \$120,000, with \$190,000 in recent grants to the same scope, does not corroborate a critical gap position. It corroborates, at the declared scope, a position at or above approaching sufficiency. The declaration and its own corroborating evidence point in opposite directions.

This is a sufficiency architecture incoherence: a declaration whose corroborating evidence contradicts the declared position. It is distinct from a declaration with no corroborating evidence, which the standard accepts at self-report strength only. Here the evidence is present, is from sources outside the applicant's control, and refutes rather than supports the declaration. The portfolio context statement compounded the problem: it was silent about the three active grants to the same scope, which an entity with multiple funding sources for the same scope must explain.

### CROSS Assessment

Sufficiency architecture declaration: incoherent. The declared position (critical gap) is contradicted by the applicant's own named corroborating evidence (a \$210,000 treasury and \$190,000 in recent same-scope grants against a \$120,000 annual scope requirement). The corroborating evidence places the entity at or above approaching sufficiency at the declared scope.

Portfolio context statement: incomplete. The three active grants attributed to the same ingestion-pipeline scope were not disclosed in the portfolio context, and their omission requires explicit explanation under the silence provision.

Revenue architecture declaration: grant-only, consistent with the rest of the application. The incoherence is in the sufficiency position, not the revenue type.

Entry specification gate: the FROM state for an open grants registry is nameable and the public benefit basis is real, but the sufficiency architecture declaration is a required element of the entry gate, and an incoherent declaration that the applicant's own evidence refutes cannot be assessed as submitted.

Recommendation: Do not fund as submitted. A surplus or approaching-sufficiency entity declaring critical gap is either misreading its own position or representing a worse resource position than its evidence shows in order to justify the ask. Either way the additionality argument cannot be assessed until the declaration is reconciled with the evidence.

### What a Coherent Declaration Would Have Looked Like

A coherent declaration would have either matched the position to the evidence or explained the apparent contradiction with specifics. For example: "Sufficiency position: approaching. The Open Collective balance of approximately \$210,000 and three active grants totaling approximately \$190,000 cover current ingestion-pipeline operations. The declared scope for this grant is not the existing ingestion pipeline but a new cross-chain ingestion layer, for which current resources are insufficient. Full scope requirement for the new layer: approximately \$80,000. This grant closes that specific gap."

That declaration would be coherent because the scope of the grant and the scope at which sufficiency is declared would match, and the corroborating evidence would support the declared position at that scope. The error in the submitted application was declaring critical gap at a scope where the applicant's own evidence showed resources already covering the stated requirement.

---

## Case 9: Public Benefit Mechanism and Access Condition Mismatch

**Project:** ModelForge
**Ask:** \$60,000
**Outcome:** Do not fund
**Criterion Illustrated:** Public benefit mechanism and access condition declaration; mechanism-evidence consistency

### The Application

ModelForge was proposed as a fine-tuned language model and an accompanying dataset for classifying smart-contract audit findings by severity. The applicant declared a public benefit mechanism of output production: the public good is the model and dataset themselves, made openly available. The access condition statement named a repository where the model weights and dataset would be hosted. The application's eligibility rested entirely on a public goods claim, which makes the public benefit mechanism dimension active and the declaration a pre-condition for assessment. The ask was \$60,000 for compute and annotation labor.

### The CROSS Finding

The mechanism type declared at entry constrains the evidence scope required at the completion gate, and the access condition for an output production mechanism is specific: it must include the SPDX license identifier and the location of the license file. A copyright notice that permits free viewing without granting modification or redistribution rights does not satisfy the output production access condition.

The repository named in the access condition statement carried a LICENSE file containing an all-rights-reserved copyright notice. The notice permitted viewing the weights and dataset but reserved all rights to copy, modify, redistribute, or build upon them. The applicant's mechanism declaration (output production) and the artifact's actual access condition (all rights reserved) are direct opposites. The access condition for output production requires an open license; all-rights-reserved copyright is the opposite of an open license.

This is the most common contradiction pattern the standard names: an applicant describes work produced under a standard all-rights-reserved copyright while claiming an output production mechanism. The standard is explicit that this contradiction cannot be resolved by reviewer judgment. A reviewer cannot decide on the applicant's behalf that the public benefit is real enough to overlook the license, because the public benefit claim for an output production mechanism is the open license. Remove the open license and the declared mechanism has no object. The contradiction must be surfaced as a material discrepancy requiring Block J investigation, and the applicant must address it before gate assessment proceeds.

A second-order problem confirmed the mismatch. The declared mechanism commits the applicant to output evidence at the completion gate, and the output evidence for an open output is the openly licensed artifact. With an all-rights-reserved license in place, the evidence scope the applicant committed to cannot be satisfied: the artifact at the completion gate would still be closed. A declared mechanism that cannot be supported by the evidence scope available at the completion gate is a misrepresentation in the entry specification.

### CROSS Assessment

Public benefit mechanism and access condition declaration: present but internally contradicted. The declared mechanism (output production) requires an open license with an SPDX identifier; the artifact carries an all-rights-reserved copyright, which is the opposite. The mechanism declaration and the access condition do not describe the same thing.

Mechanism-evidence consistency: fails. The output production mechanism commits the applicant to openly licensed output evidence at the completion gate. The all-rights-reserved license means that evidence scope cannot be satisfied. This is a misrepresentation in the entry specification, not a curable documentation gap, unless the applicant changes the license.

Entry specification gate: not completed. The public benefit mechanism declaration is a pre-condition for assessment in a public goods program, and a declaration contradicted by its own named artifact must be surfaced under Block J before assessment proceeds.

Recommendation: Do not fund as submitted. The recommendation is not a judgment that a closed model has no value; it is that the application claims an open-output public good while the named artifact is closed, and the two cannot both be true.

### What a Conformant Declaration Would Have Looked Like

There are two conformant paths, and the applicant must choose one before assessment.

The first path keeps the output production mechanism and fixes the artifact: "Mechanism type: output production. Access condition: the model weights and dataset are released under Apache-2.0 (SPDX identifier Apache-2.0), with the LICENSE file at the repository root. The license is applied at the time of application." This makes the declared mechanism and the artifact consistent, and the open license is the public good the mechanism rests on.

The second path keeps the closed license and changes the mechanism to one the artifact can support: "Mechanism type: access provision. The model is offered as a hosted classification service. Access mechanism: a public application programming interface. Cost structure: free below a stated rate limit. Non-excludability mechanism: no allowlist; any party may query." Under an access provision mechanism the public good is usage of the service rather than the open artifact, and the completion gate would require usage evidence rather than an open-license artifact. A closed license is compatible with an access provision claim in a way it is not compatible with an output production claim.

What is not conformant is the submitted combination: an output production claim over an all-rights-reserved artifact.

---

## Case 10: Development Stage Mismatch

**Project:** ChainProbe
**Ask:** \$50,000
**Outcome:** Do not fund
**Criterion Illustrated:** Development stage declaration; stage-evidence consistency

### The Application

ChainProbe was proposed as a monitoring service that watches deployed contracts for anomalous state transitions and alerts operators. The applicant declared development stage 4, established infrastructure, and selected a change-obligation mode with an indicator framed around reducing operator response time to on-chain incidents. The development stage dimension is active in all rounds, so the declaration was required, and a stage 4 declaration carries a specific evidence requirement: 12 months of sustained usage data from sources outside the team. The ask was \$50,000 to expand alert coverage to additional chains.

### The CROSS Finding

The declared development stage must be consistent with the evidence provided elsewhere in the entry submission, and a declared stage that is not supported by the provided evidence is a material discrepancy requiring Block J investigation. Stage 4, established infrastructure, requires 12 months of sustained usage data from sources outside the team. The evidence in the submission did not meet that bar, and the gap was not marginal.

The earliest public commit to the ChainProbe repository was dated five months before the application. The service's public status page, the only usage-adjacent artifact offered, had recorded data for four months. The application named two external users; one was a testnet-only integration with no production traffic, and the other was an organization whose own public materials described a pilot begun two months before the application. No source outside the team showed 12 months of sustained usage, because the service had not existed for 12 months. The stage 4 declaration was contradicted by the project's own timeline.

The mismatch also propagated into the obligation mode. A stage 4 applicant whose evidence actually shows early adoption is, on the evidence, a stage 2 project: early adoption applications must provide usage evidence from at least one named external user, which ChainProbe could arguably meet for the single production pilot. A stage 2 project selecting a change obligation framed around population-level response-time reduction is committing to outcome evidence against a baseline it does not yet have, because the service has not been deployed long enough to establish one. The stage misdeclaration is what made the obligation-mode selection look coherent; corrected to the stage the evidence supports, the change-obligation framing is premature.

The standard is explicit that this is not a reviewer judgment call. A stage 4 declaration paired with no 12-month independently verifiable usage data is a discrepancy requiring Block J investigation. The applicant must address the discrepancy before gate assessment proceeds.

### CROSS Assessment

Development stage declaration: contradicted by the evidence. Stage 4 requires 12 months of sustained external usage data; the project is five months old by its own repository history, and the usage artifacts cover at most four months, with one production pilot two months in.

Stage-evidence consistency: fails. The provided evidence supports stage 2, early adoption, at most. The declared stage 4 overstates maturity by a category that the program's stage targeting may have relied on.

Obligation mode coherence: the change-obligation selection depends on the stage 4 claim. At the stage the evidence supports, there is no established baseline for the response-time indicator, and the change obligation is premature. A build obligation, or a change obligation deferred to a later stage, would fit the actual evidence.

Entry specification gate: not completed on the declared terms. The stage discrepancy must be resolved under Block J before the gate is assessed, because the declared stage constrains which obligation modes are coherent and which evidence scopes are achievable.

Recommendation: Do not fund as submitted. The service may be a sound early-adoption project; it is not the established infrastructure the application declared, and the obligation mode was selected against the overstated stage.

### What a Conformant Declaration Would Have Looked Like

A conformant declaration would have matched the stage to the evidence and selected an obligation mode the stage supports: "Development stage: 2, early adoption. Evidence: one production integration (named organization, pilot begun [date], public materials confirm), plus a testnet integration. The service has been deployed for five months; we do not claim the 12 months of sustained external usage that stage 4 requires. Obligation mode: build, with the deliverable being multi-chain alert coverage and completion criteria [specified]. We will establish a response-time baseline during this grant and propose a change obligation at a subsequent stage once 12 months of usage data exist."

That declaration is coherent because the stage, the evidence, and the obligation mode agree. The submitted application's error was declaring a stage the timeline could not support and then selecting an obligation mode that only the overstated stage made coherent.

---

## Case 11: Obligation Fulfillment Non-Disclosure

**Project:** Relay Mesh
**Ask:** \$70,000
**Outcome:** Do not fund
**Criterion Illustrated:** Obligation fulfillment record; non-disclosure of a prior failure

### The Application

Relay Mesh was proposed as a continuation grant to extend a cross-chain message-relay library the applicant had built under a prior grant from this same funder. The applicant had received \$40,000 from this funder in a round nine months earlier. Because the applicant received a prior grant from this funder and cited that prior work as evidence of capability, an obligation fulfillment record was required before gate assessment could proceed. The applicant submitted an obligation fulfillment record stating that the prior grant's milestones had been fulfilled and the relay library shipped. The ask was \$70,000 to extend the library to additional message formats.

### The CROSS Finding

The obligation fulfillment record documents, for each prior grant from this funder, what was committed, what was produced, and whether the commitment was fulfilled, partially fulfilled, or unfulfilled, with the applicant's explanation where fulfillment was not complete. An unfulfilled prior obligation is not automatically disqualifying. It is a disclosed fact that affects the track record assessment and may be addressed through a written explanation. The decisive distinction the standard draws is that non-disclosure of a prior failure is treated more seriously than the failure itself.

The submitted record stated full fulfillment. The Attestation Corpus query against the applicant's on-chain identity anchor returned the prior grant's KarmaGAP milestone record, which the standard requires the program to consult where prior round history includes unresolved milestones. Of the prior grant's three committed milestones, the KarmaGAP record showed one marked complete, one marked partial, and one still open with no submission against it nine months after the grant period. The prior grant's completion gate determination, a signed record from the funder, documented that final disbursement had been held pending the open milestone and never released. The relay library that the application cited as shipped corresponded to the one completed milestone; the two message-format deliverables that the current ask proposes to extend were the partial and open milestones from the prior grant.

The obligation fulfillment record claimed full fulfillment of an obligation the funder's own signed records showed as partially fulfilled and partly unfulfilled, with final payment withheld. Had the applicant disclosed the partial fulfillment and explained what prevented completion, the prior failure would have been a disclosed fact weighed at the continuation gate, not a bar. By stating full fulfillment against records that show otherwise, the applicant converted an addressable prior failure into a material discrepancy under Block J: non-disclosure of a prior obligation that the Attestation Corpus reveals is treated as a material discrepancy under the adverse signal provisions.

### CROSS Assessment

Obligation fulfillment record: false as submitted. The record claims full fulfillment of the prior grant; the funder's signed completion determination and the KarmaGAP milestone record show one complete, one partial, and one open milestone, with final disbursement withheld.

Attestation Corpus query: surfaces the discrepancy independently of the applicant's disclosure. Prior milestones and obligations not disclosed in the obligation fulfillment record, but present in the Corpus, constitute non-disclosure of a prior obligation.

Continuation gate track record: the prior failure itself would not bar a continuation grant if disclosed and explained. The non-disclosure does. The current ask compounds the problem by proposing to fund, as new work, the two deliverables the prior grant left partial and open.

Entry specification gate: not completed. The obligation fulfillment record is a pre-condition for assessment where prior grants from this funder exist, and a record contradicted by the funder's own signed determination must be surfaced under Block J before assessment proceeds.

Recommendation: Do not fund as submitted. The finding is squarely the one the standard singles out: the undisclosed prior failure is treated more seriously than the failure would have been, because non-disclosure removes the funder's ability to weigh it.

### What a Conformant Record Would Have Looked Like

A conformant obligation fulfillment record would have read: "Prior grant from this funder, \$40,000, [round]. Committed: three milestones (core relay library; message-format A; message-format B). Produced: the core relay library shipped and is in use (link). Message-format A reached partial completion (link to partial work). Message-format B was not delivered. Fulfillment status: partially fulfilled. Final disbursement was withheld pending the open milestones. What prevented completion: [specific explanation, for example a dependency change in an upstream protocol]. What has changed since: [specific]. This continuation request includes completing message-formats A and B, which were the unfulfilled milestones, and we disclose that they were previously committed and not delivered."

That record would let the continuation gate weigh a disclosed partial fulfillment on its merits. The submitted record's error was claiming full fulfillment against the funder's own contrary signed record, which is the specific non-disclosure the obligation fulfillment record exists to prevent.

---

## Case 12: Prior Work Attribution Failure

**Project:** Aperture Analytics
**Ask:** \$55,000
**Outcome:** Do not fund
**Criterion Illustrated:** Prior work attribution statement; track record built under a different entity

### The Application

Aperture Analytics was proposed as a retroactive-obligation application. The applicant, an individual, presented as their prior contribution a widely used on-chain analytics dashboard with a large named user base, citing the dashboard's adoption as the evidence of contribution the retroactive round rewards. Because the entire entry submission consisted of prior work cited as evidence of contribution, a prior work attribution statement was required. The applicant's submission described the dashboard as "my project" throughout. The ask was \$55,000 in retroactive recognition.

### The CROSS Finding

Where an applicant cites prior work as evidence of capability, track record, or past contribution, a prior work attribution statement is required, and it must address three questions for each piece of cited work: the entity of performance, the applicant's relationship at the time and now, and current ownership and access. For a retroactive application, the entire submission is prior work, so the attribution statement covers the whole evidential basis.

The dashboard the applicant cited was built while the applicant was an employee of Meridian Data, a company that owns the dashboard, hosts its deployment, and holds the relationship with the cited users. Public records confirmed the applicant's authorship of a substantial portion of the codebase during their employment and confirmed their departure from Meridian Data approximately seven months before the application. Meridian Data continues to operate, maintain, and host the dashboard. The applicant's submission did not name Meridian Data, described the dashboard as their own project, and presented the dashboard's current user base as evidence of the applicant's contribution.

The standard addresses this precisely. An individual who founded or built a project within an organization and has since departed is in a materially different position from an individual who built and controls an independent project. A contributor who wrote part of a codebase held by another entity is in a materially different position from the entity that owns and maintains it. A claim of prior contribution to a project does not confer the right to represent that project's user base or codebase as the applicant's own in a retroactive application. The prior work attribution statement is an adverse signal disclosure requirement: an applicant who cannot truthfully complete it for their cited prior work has surfaced a misrepresentation in the core evidential basis of the application.

The applicant's contribution to the dashboard is real; the prior work attribution failure is not a claim that they did no work. It is that the entry submission claims responsibility for outcomes (the current user base, the maintained deployment) that the applicant did not control and cannot warrant continuing, because Meridian Data owns the deployment, maintains the code, and holds the user relationship. The application's track record is built on work performed under a different entity, presented without that entity's role disclosed.

### CROSS Assessment

Prior work attribution statement: false on all three questions. Entity of performance: the dashboard was built under Meridian Data, not disclosed. Applicant's relationship: employee at the time, departed seven months before application, not disclosed. Current ownership and access: Meridian Data owns the intellectual property, controls the deployment, and holds the user relationship; the applicant holds none of these. The submission described the dashboard as the applicant's own project throughout.

Adverse signal disclosure: the attribution failure is itself the adverse signal. An applicant who cannot truthfully complete the attribution statement has surfaced a misrepresentation in the evidential basis of the application.

Entry specification gate: not completed. For a retroactive application the prior work attribution statement covers the entire evidential basis, and a statement that misrepresents the entity of performance and current ownership cannot support a contribution claim.

Recommendation: Do not fund. The retroactive contribution being claimed belongs, in its current and maintained form, to an entity the applicant has left and did not name. The applicant's partial authorship does not confer the right to claim the dashboard's present user base as their own contribution.

### What a Conformant Statement Would Have Looked Like

A conformant prior work attribution statement would have read: "The dashboard was built while I was an employee of Meridian Data (entity of performance). I authored approximately [portion] of the codebase between [dates]. I left Meridian Data in [month]; Meridian Data currently owns the intellectual property, hosts the deployment, and holds the relationship with the cited users (current ownership and access). I do not control the deployment or the user relationship. What I present for retroactive recognition is my specific authored contribution during my employment, not the dashboard's current user base, which Meridian Data maintains."

Such a statement might still support a narrower retroactive claim scoped to the applicant's actual authored contribution, assessed on its own terms and with Meridian Data's role visible. What the standard bars is the submitted framing: the dashboard's current adoption presented as the applicant's own contribution, with the owning entity unnamed.

---

## Case 13: Served-Population Risk-Bearer Floor at the Completion Gate

**Project:** Two completion-gate determinations (Onboard Bridge; Civic Relay)
**Ask:** Completion gate, not entry
**Outcome:** One determination conformant; one returned for redetermination
**Criterion Illustrated:** Served-population exposure as a named consideration at each gate; completion verification gate determination record

### The Setting

This case differs from the others: it illustrates the completion verification gate rather than the entry specification gate, and it compares two determination records from change-obligation grants whose eligibility rested on serving a defined population. The served population is a risk-bearer of the round's evaluation, named at entry and carried through every gate. At the completion verification gate, the determination and the unintended outcomes disclosure must additionally consider whether the served population bears exposure the round has not surfaced: work recorded as delivered that does not reach them, or effects on them that the declared indicators do not capture. The standard requires that the determination record show this consideration was applied, not merely that the population was named at entry.

Both grants below reported their declared indicators as met. The difference is in the determination records.

### Determination One: Onboard Bridge (conformant)

Onboard Bridge received a change-obligation grant to reduce the time first-time users in a named low-connectivity region take to complete a wallet-onboarding flow. The declared indicator (median completion time for the onboarding flow) was reported as met: median time fell from the entry baseline to below the target.

The completion gate determination record did three things beyond confirming the indicator moved. First, it recorded that the determination considered whether the recorded completion-time improvement reached the served population specifically, rather than a faster-connectivity subset: the grantee disaggregated the median by connection class, and the determination noted that the improvement held within the low-connectivity class the round was scoped to serve, not only in aggregate. Second, the unintended outcomes disclosure named an effect the declared indicator did not capture: a share of low-connectivity users who began the faster flow abandoned it at a new wallet-funding step, an effect on the served population that median completion time alone would have hidden. The determination recorded this as an adverse signal and routed it to the continuation gate assessment. Third, the determination record stated in plain terms that the served population's exposure had been considered and what was found, rather than treating the named-at-entry population as sufficient.

This is the conformant pattern. The determination record shows the served-population consideration was applied at the completion gate: the indicator was checked against the served population specifically, an effect outside the declared indicator was surfaced through the unintended outcomes disclosure, and the consideration was visible in the record.

### Determination Two: Civic Relay (returned for redetermination)

Civic Relay received a structurally similar change-obligation grant to increase the number of civic-information requests served through a relay in a named underserved community. The declared indicator (count of requests served) was reported as met: the request count exceeded the target.

The completion gate determination record confirmed the count and released final payment. It did nothing else. It did not record whether the served requests came from the underserved community the round was scoped to serve or from higher-connectivity users elsewhere who found the relay. The unintended outcomes disclosure field was left blank; the grantee did not state that no unintended outcomes occurred, and the determination did not flag the silence, although the standard requires that grantees who state no unintended outcomes occurred say so explicitly and that silence does not satisfy the disclosure requirement. The determination record named the served population once, at entry, and never returned to it. Work recorded as delivered (requests served) was confirmed in aggregate without any record that the determination considered whether it reached the population the round exists to serve.

This determination is not conformant, and the defect is specifically the one the standard names: the determination record does not show that the served-population consideration was applied. A count of requests served that does not distinguish the served population from incidental higher-connectivity users may record delivery that does not reach the people the round was scoped to serve. The standard requires the determination to consider exactly this exposure and the record to show it. Here the aggregate indicator stood in for the served-population check, which the standard does not permit.

### CROSS Assessment

Onboard Bridge completion gate: conformant. The determination record shows the served-population consideration was applied: the indicator was disaggregated and confirmed within the served class, an effect outside the declared indicator was surfaced through the unintended outcomes disclosure and routed to continuation, and the consideration is visible in the record.

Civic Relay completion gate: not conformant. The determination confirmed the aggregate indicator and released payment without any record that the served population's exposure was considered, and with the unintended outcomes disclosure field left blank and unflagged. The served population was named at entry and not carried to the gate.

Disposition: Onboard Bridge's determination stands. Civic Relay's determination is returned for redetermination before the completion gate can be treated as satisfied. The redetermination must record whether the served requests reached the underserved community the round was scoped to serve, and must resolve the blank unintended outcomes field, either with a disclosure or with an explicit statement that none occurred and the basis for that conclusion.

### What the Redetermination Requires

A conformant Civic Relay determination would disaggregate the served-request count to show what share came from the underserved community the round targeted, rather than from incidental higher-connectivity users, and would record that finding in the determination. It would resolve the unintended outcomes field rather than leave it blank: either a disclosure of effects on the served population the request count does not capture, or an explicit statement that none occurred with the basis for that determination, since the absence of unintended outcomes in a community-facing intervention warrants documented reasoning. The aggregate count being met is necessary but not sufficient; the determination must show that the served population's exposure was considered, which is the floor every gate is checked against.

---

## Summary Table

| Case | Project | Criterion Illustrated | Entry Gate Status | Outcome |
|------|---------|----------------------|-------------------|---------|
| 1 | Mushee Allocate | Beneficiary validation | Passes; fails beneficiary validation dimension | Do not fund |
| 2 | mev-commit | Operational definition; Integrity | Passes (on encrypted mempool milestone); fails rigor tier | Do not fund |
| 3 | MoaV | Privacy-sensitive accommodation | Passes | Fund with conditions |
| 4 | The Interfold | Concurrent funding disclosure; Adverse signal disclosure | Passes | Fund with conditions |
| 5 | Gean | Entry gate passage; Institutional capacity | Passes | Fund with conditions |
| 6 | poidh | Adverse signal disclosure; Conditional funding | Passes | Fund with conditions |
| 7 | Cohort Signal | Organizational identity declaration | Not reached (declaration incomplete; serial rebranding and affiliated-entity omission) | Do not fund |
| 8 | Lattice Grants Registry | Sufficiency architecture declaration | Not completed (declaration contradicted by its own corroborating evidence) | Do not fund |
| 9 | ModelForge | Public benefit mechanism and access condition | Not completed (output production mechanism over an all-rights-reserved artifact) | Do not fund |
| 10 | ChainProbe | Development stage declaration | Not completed (stage 4 declared; evidence supports stage 2) | Do not fund |
| 11 | Relay Mesh | Obligation fulfillment record | Not completed (record claims full fulfillment; signed records show partial and open) | Do not fund |
| 12 | Aperture Analytics | Prior work attribution statement | Not completed (track record built under an undisclosed different entity) | Do not fund |
| 13 | Onboard Bridge; Civic Relay | Served-population risk-bearer floor (completion gate) | Completion gate; one conformant, one returned for redetermination | One stands; one redetermined |

---

## Key Distinctions This Set Illustrates

Five distinctions recur across these cases and are worth naming explicitly for practitioners.

The first is the distinction between an entry specification gate failure and a rigor-tier failure. Cases 1 and 2 both result in Do not fund, but for structurally different reasons. Mushee Allocate fails at the beneficiary validation dimension: the FROM state exists but was not validated against the competitive landscape. mev-commit passes the gate on its encrypted mempool milestone (a specific condition is named) but fails at the rigor tier on indicator specification and integrity. These require different responses from a committee: a gate failure redirects the applicant to do foundational diagnostic work before reapplying; a rigor-tier failure identifies specific documentation deficiencies that could potentially be addressed in a revised application.

The second is the distinction between D1 and D2 failure modes in change-obligation rounds. These are Frame Language diagnostic categories that appear in the CROSS assessment rubric. A D2 failure (values aspiration without conditions) cannot name a FROM state at all; the application produces more values language when pressed for a diagnosis. A D1 failure (canonical vocabulary without structural grounding) can name a FROM state using recognized terminology but cannot support the specific measurable indicators claimed with sourced methodology. Both fail at the entry specification gate, but at different levels and for different reasons, and the appropriate response to each is different. Note that these failure modes apply specifically to change-obligation rounds; the entry specification gate for build-obligation rounds uses different failure vocabulary (direction specification without deliverable; underspecified completion criteria).

The third is the distinction between adverse signal disclosure failure and a disqualifying adverse signal. Cases 4 and 6 both involve incomplete adverse signal disclosure. In neither case does the disclosure failure automatically disqualify the application: The Interfold's cryptographic work is real and the Zcash rejection does not invalidate it; poidh's protocol merits are genuine and the v2 exploit was remediated. The Adverse-Signal Engagement Principle Core Standard requires disclosure; it does not treat disclosed adverse signals as automatic bars. The conditions in both cases are designed to produce the disclosure and allow the evaluation to proceed on complete information.

The fourth is the distinction between a declaration that is missing and a declaration that is present but refuted by its own evidence, and between a curable rigor-tier deficiency and a pre-condition the gate cannot be assessed without. Cases 7 through 12 all turn on a required entry declaration that is a pre-condition for assessment rather than a scored criterion: the organizational identity declaration (Case 7), the sufficiency architecture declaration (Case 8), the public benefit mechanism and access condition declaration (Case 9), the development stage declaration (Case 10), the obligation fulfillment record (Case 11), and the prior work attribution statement (Case 12). A pre-condition declaration that is absent leaves the submission incomplete and unassessed. A pre-condition declaration that is present but contradicted (by its own corroborating evidence in Case 8, by its own named artifact in Case 9, by the project's own timeline in Case 10, by the funder's own signed records in Cases 7 and 11, by public records of the entity of performance in Case 12) is a material discrepancy requiring Block J investigation before assessment proceeds. The recurring structural point is that several of these cases were surfaced not by reading the application alone but by the funder-side procedures the standard requires: the Attestation Corpus query and the Cohort Position assessment turned self-reported declarations against independent records. Non-disclosure, in each, is treated more seriously than the underlying fact would have been if disclosed.

The fifth is that the served population is a risk-bearer of the round's evaluation carried through every gate, not validated only at entry. Case 13 shows this at the completion verification gate: two structurally similar grants both reported their declared indicators as met, and the difference was whether the determination record showed that the served population's exposure had been considered. The conformant determination disaggregated the indicator to confirm it reached the served population and surfaced an effect the indicator did not capture; the non-conformant determination let the aggregate indicator stand in for the served-population check. An aggregate result being met is necessary but not sufficient. The determination record must show the consideration was applied, which is the floor every gate is checked against.
