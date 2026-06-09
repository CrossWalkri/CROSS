---
title: CROSS+WALKRI Primitives Framework Index
version: 0.2.0
date: 2026-06-07
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
foundation: CROSS-WALKRI-primitives-foundation-0_1_0.md (internal version 0.2.0, the 146-primitive basis)
---

# CROSS+WALKRI Primitives Framework Index

---

## Purpose

This index maps each measurement primitive in the CROSS+WALKRI Primitives Foundation to the external frameworks that most clearly exemplify it in practice. It serves two functions.

First, classification: when a new external framework is encountered, locate the primitive it most clearly exemplifies before deciding whether a full compatibility statement is needed. If the framework exemplifies a primitive already well-covered by existing statements, a Tier 2 index entry may be sufficient. If the framework exemplifies the primitive in a structurally novel way, a Tier 1 statement is warranted.

Second, architecture: the index shows that CROSS+WALKRI's compatibility claims are not an accumulation of framework-by-framework agreements but a consequence of underlying structural alignment. All 95+ covered frameworks exemplify some combination of the primitives listed here. New frameworks will do the same.

Primitives from the Foundation's methodological layer (Bidirectional Precision, Transclusion, Frame Language) and most identity-layer primitives (Entity Boundary, Scope, Sufficiency, Revenue Architecture, Disbursement Authority, Continuity Capacity, Development Stage, On-chain Identity Anchor) generate CROSS+WALKRI provisions but do not produce distinctive framework exemplars at the level of external compatibility claims. This index covers the primitives that generate the most significant external framework alignments: obligation primitives, gate primitives, measurement primitives, and the cohort-facing WALKRI primitive.

A separate section at the end documents primitives identified during the framework research that are not yet in the Primitives Foundation and are candidates for the next foundation revision.

---

## Obligation Primitives

### Obligation Mode (Build / Change / Retroactive)

**Definition reference:** Primitives Foundation Layer 3.

**What it identifies:** Whether a grant asks grantees to deliver a specified output (Build), achieve a measurable condition change in a population (Change), or document demonstrated prior contribution (Retroactive).

**Framework exemplars by mode:**

*Build obligation most clearly embodied:*
- ARPA-H Payable Milestones (observable technical event with completion criteria; payment contingent on delivery)
- DARPA / BARDA Other Transactions (same OT milestone structure)
- SBIR/STTR Phase I (feasibility deliverable; go/no-go to Phase II)
- Challenge prizes and innovation programs (Nesta Challenge Prizes, EIR Early-Phase)
- 45 CFR Part 1302 Head Start (PIR output delivery and ELOF-aligned assessment)

*Change obligation most clearly embodied:*
- USAID PIRS (outcome indicator specification with FROM/TO condition change)
- WIOA Performance Accountability (six indicators measuring labor market condition changes)
- SAMHSA NOMs/GPRA (condition change across housing, employment, substance use, functioning)
- Ryan White HIV/AIDS HAB Performance Measures (viral suppression as measurable clinical condition change)
- LIHEAP Performance Measures (energy burden reduction; crisis prevention counterfactual)
- UNTF (violence against women outcome indicators)
- SNAP-Ed Evaluation Framework (individual dietary behavior change through ecological levels)

*Retroactive obligation most clearly embodied:*
- Optimism RetroPGF Rounds 1-4 (past impact rewarded retroactively)
- Optimism Retro Funding 2025 (weighted metrics formula on demonstrated past impact)
- Protocol Guild (ongoing retroactive recognition of core Ethereum contributors)
- Gitcoin Retroactive rounds

---

### Allocation Rule

**Definition reference:** Primitives Foundation Layer 3 (Allocation Rule).

**What it identifies:** The combinatory act by which a round resolves its assessment into a distribution of the pool: the function that maps evaluated applications to amounts. It was the basis's one systematic gap, surfaced by an unprimed compose-back over real programs and recomposition-validated across all eight of its configuration values. The configuration a program declares is what distinguishes a quadratic-funding round from a peer-review panel from a lottery, even when the upstream evaluation looks similar.

**Framework exemplars by configuration value:**

*Quadratic funding (matching scaled by breadth of support):*
- Gitcoin Grants (quadratic matching of many small contributions into a matching pool)

*Weighted-metric vote tally:*
- Optimism Retro Funding (badgeholder votes resolved by a published weighted-metric formula)

*Collective decision rule:*
- Participatory grantmaking programs (community panels resolving allocation by consensus or vote)
- Co-Impact (core partners resolving allocation jointly under a declared decision rule)

*Performance-weighted formula:*
- Global Fund allocation methodology (disease burden and national income as the formula inputs)

*Peer-review score with discretion:*
- NSF and traditional research councils (panel scores combined with program-officer discretion)

*Winner-take-pool:*
- MacArthur 100&Change and challenge prizes (one or a few winners take the pool)

*Outcome-contingent function:*
- Social Impact Bonds and Pay for Success (the amount paid is a function of measured outcomes against a locked counterfactual baseline)

*Random draw:*
- New Zealand Health Research Council Explorer Grants (lottery among applicants who clear a quality bar)
- Volkswagen Foundation Experiment! (randomized selection among eligible proposals)

---

### Financing Instrument Type

**Definition reference:** Primitives Foundation Layer 3 (Financing Instrument Type).

**What it identifies:** The declared financial form of the transfer, the property that determines whether and on what terms capital flows back to the funder: a pure grant, a repayable grant, a concessional loan, or a blend. It is selected among by an instrument-selection assessment but exists wherever a program declares its instrument, including programs that offer only grants.

**Framework exemplars:**

*Risk-graded instrument selection (form set by an independent debt analysis):*
- African Development Fund (one hundred percent grants, a fifty-fifty grant and concessional-loan blend, or concessional loans only, by debt-distress risk)
- World Bank International Development Association grant-loan blend under the joint IMF and World Bank Debt Sustainability Framework

*Concessional instrument families:*
- International Development Association concessional instruments (Investment Project Financing, Development Policy Financing, Program-for-Results)

*Repayable-grant form:*
- Recoverable-grant and repayable-grant structures (a grant returned to the funder on a triggering condition rather than on a fixed loan schedule)

---

### Theory of Change Hierarchy

**Definition reference:** Primitives Foundation Layer 6 (Theory of Change Hierarchy, Pathway; the former Theory Layer is folded into Theory of Change Hierarchy as of v0.2.0).

**What it identifies:** The structured causal chain from activities through outputs through outcomes through goals, with each layer requiring distinct evidence.

**Framework exemplars:**

*Most explicit full hierarchy implementation:*
- W.K. Kellogg Foundation Logic Model (resources/inputs, activities, outputs, short-term outcomes, long-term outcomes; exact vocabulary match to CROSS hierarchy)
- IMLS Outcome-Based Evaluation (outcomes defined as "benefits to people" explicitly excluding activities and outputs; forces hierarchy discipline)
- SNAP-Ed Evaluation Framework (four ecological levels: individual, environmental settings, sectors of influence, population results; maps to output through goal tiers)
- Head Start ELOF (five developmental domains as the outcome layer; PIR as the output layer)

*Hierarchy enforced by regulatory exclusion:*
- NED Evaluation Framework (explicit regulatory rejection of activity completion as evaluation evidence; enforces the activity/outcome distinction)
- ESSA Evidence Tiers (Tier 4 requires ongoing study commitment before program begins; Tiers 1-3 escalate causal claim requirements)
- AmeriCorps prescribed output/outcome pairing menu (selecting an output commitment automatically requires a matched outcome commitment)

*Hierarchy expressed across ecological levels:*
- CSBG ROMA Six National Goals (individual economic self-sufficiency through community-level conditions)
- IAF Grassroots Development Framework (individual/household, organizational, community/society)
- HUD Continuum of Care System Performance Measures (program-level exits to housing at outcome tier; system-level flow at goal tier)

---

### Causality Stance

**Definition reference:** Primitives Foundation Layer 4 (Causality Stance, Intended vs. Unintended Effects).

**What it identifies:** Whether a program claims attribution (it caused the measured change) or contribution (it contributed to a change produced by multiple factors); and the specification of the counterfactual baseline against which the claim is assessed.

**Framework exemplars:**

*Attribution claim with published counterfactual methodology:*
- Verra Verified Carbon Standard (additionality as first-order gate; approved baseline methodology required before any project begins)
- REDD+ Warsaw Framework (forest reference emission level as the national-scale counterfactual baseline)
- Gold Standard for Global Goals (dual-track attribution for carbon and SDG co-benefits)
- ESSA Tier 1 (RCT as the institutional form of attribution claim)
- PCORI Methodology Standards (causal inference domain; mandatory pre-registered comparison)

*Contribution claim with structured portfolio context:*
- OECD DAC criteria (relevance, effectiveness without attributing population-level outcomes to individual programs)
- FCDO Programme Operating Framework (portfolio contribution to strategic objectives)
- UN SDG Impact Standards IS-FSD (portfolio-level contribution to SDGs)

*Counterfactual as regulatory requirement:*
- LIHEAP Measure 2 (energy crisis prevention requires a counterfactual determination; one of the few US human services statutory measures to encode this explicitly)
- EU ESIF "EU added value" criterion (what the EU contribution produces that member state action alone would not have; a regulatory additionality requirement)
- ARPA-H / DARPA milestone completion criteria (non-achievement triggers termination, implying the counterfactual of non-completion is defined)

---

### Sustainability Stance

**Definition reference:** Primitives Foundation Layer 6 (Sustainability Stance, Pathway).

**What it identifies:** Whether outcomes are sustained independently, conditional on continued inputs, or dependent on continued grant funding after the grant period ends.

**Framework exemplars:**

*Sustainability as continuation gate criterion:*
- Gates Foundation Evaluation Policy (learning for impact; evaluation designed to inform continuation decisions)
- EIR Program escalating evidence tiers (Mid-Phase-to-Expansion requires sizable, significant impacts; implicitly tests sustainability of effect)
- CGIAR MELIA (systematic learning about what works in agricultural R&D contexts with long sustainability horizons)

*Sustainability as adaptive mechanism:*
- USAID CLA (Collaborating, Learning, and Adapting; adaptive management as the mechanism by which programs course-correct toward sustained impact)
- World Vision LEAP Reflect Stage (inter-cycle reflection as the structural mechanism for learning before next programme begins)
- Developmental Evaluation methodology (evaluation embedded in program development; adaptation is the point)

---

## Gate Primitives

### Entry Specification Gate

**Definition reference:** Primitives Foundation Layer 3 (Gate Type: entry specification).

**What it identifies:** The requirement that all indicators, criteria, and evaluation plans be committed to publicly before any application is received. The pre-commitment makes the gate criteria independent of any funder's post-hoc interest.

**Framework exemplars by governance level:**

*Statutory / regulatory entry gates (criteria fixed by law):*
- WIOA Performance Accountability (six indicators fixed by 20 CFR Part 677)
- Perkins V CTE (indicator categories fixed by statute, 20 USC Chapter 44)
- LIHEAP (three measures established by statute and June 2013 Federal Register notice)
- ESSA Evidence Tiers (four-tier hierarchy codified at 34 CFR 77.1)
- Head Start (ELOF domains required by 45 CFR Part 1302)

*Published framework entry gates (criteria fixed by funder policy):*
- PCORI Methodology Standards (board-adopted; mandatory for all funded research)
- Arnold Ventures Open Science Guidelines (preregistration mandate; PAP required before data collection)
- UK Government Evaluation Registry (mandatory public pre-registration from April 2024)
- AmeriCorps prescribed output/outcome pairing menu
- Optimism Retro Funding 2025 (metrics formula committed before applications open)

*Entry gate as program design requirement (funder commits before applicants see the form):*
- CROSS itself (entry specification gate as the foundational gate type)
- HRSA Title V NPMs (state Block Grant Application before any expenditure)
- SNAP-Ed state Plans (submitted and approved before funding release)
- IMLS OBE (five structural elements required in every grant before any award)
- CSBG ROMA (Six National Goals established nationally before any program year)

---

### Independent Verification Pathway

**Definition reference:** Primitives Foundation Layer 3 (Gate Type: attestation; Attestation Corpus).

**What it identifies:** The structural requirement that outcome claims be verified by an independent party rather than accepted on self-report alone. Independence is structural: the verifier cannot be the entity whose claims are being verified.

**Framework exemplars:**

*Threshold-based mandatory independence:*
- UNTF (grants over USD 150,000: grantee-managed external evaluation; grants under USD 150,000: co-managed with Secretariat)
- AmeriCorps (grants above USD 500,000 average annual: mandatory independent evaluation submitted with reapplication)
- CGIAR MELIA (independent evaluation units embedded in CGIAR centers)

*Registry-based pre-registration as independence mechanism:*
- PCORI (mandatory public protocol registration before any data collection; creates independently accessible pre-commitment)
- Arnold Ventures (OSF Registries, AsPredicted, ClinicalTrials.gov as the verification infrastructure)
- UK GovS 015 Government Evaluation Registry (mandatory public registration of all government evaluations from April 2024)
- Verra VCS (third-party Validation and Verification Body; VCU issuance via public registry)

*OT milestone completion as verification structure:*
- ARPA-H (Program Manager confirms milestone achievement against pre-specified completion criteria)
- DARPA, BARDA (same OT milestone structure)

*Public data release as attestation infrastructure:*
- 360Giving Data Standard (machine-readable grant data published before any independent analysis)
- SBIR/STTR database (sbir.gov as the public attestation corpus for commercialization claims)
- HMIS / HUD CoC (HMIS as mandatory data infrastructure; AHAR as annual public release)

---

### Portfolio Aggregation

**Definition reference:** Primitives Foundation Layer 3 (Portfolio Position, Portfolio Analysis Outputs).

**What it identifies:** The capacity to aggregate individual grant outcomes into portfolio-level findings, enabling funders to assess their overall impact rather than only per-grant compliance.

**Framework exemplars:**

*Statutory portfolio-level benchmarks (funder portfolio must meet threshold):*
- SBIR/STTR (Phase I-to-II transition rate of 0.25 minimum; USD 100,000 commercialization revenue per Phase II award average; applied to the agency's full SBIR/STTR portfolio, not individual grantees)

*Pre-specified portfolio-level indicator sets:*
- HRSA UDS (16 mandatory clinical quality measures aggregated from 1,400+ health centers to national benchmarks)
- SAMHSA NOMs / SPARS (client-level data aggregated across all SAMHSA grantees to national behavioral health indicators)
- WIOA (six indicators aggregated from local boards to state-level and national-level compliance determination)

*EU-style performance framework with portfolio consequences:*
- ESIF / EU Cohesion Policy Performance Framework (mid-term milestones and targets with potential reprogramming consequences for underperforming programs)

*Portfolio learning as explicit program design:*
- Walton Family Foundation SLED (portfolio-level learning agenda across program areas; individual grant measures designed to contribute to portfolio questions)
- CGIAR MELIA (portfolio learning across centers and programs)

---

### Learning Loop / Adaptive Continuation

**Definition reference:** Primitives Foundation Layer 3 (Pathway, Sustainability Stance).

**What it identifies:** A formally structured mechanism by which learning from one grant cycle informs the design of the next, distinct from both the completion gate (which closes the current cycle) and the entry gate (which opens the next).

**Framework exemplars:**

*Formally named inter-cycle learning stages:*
- World Vision LEAP (Reflect stage as a formally required programme cycle stage between close-out and next design)

*Adaptation as the primary mechanism:*
- USAID CLA Framework (Collaborating, Learning, and Adapting; adaptive management embedded in program cycle)
- Developmental Evaluation methodology (evaluation embedded in development; findings used in real time rather than post-hoc)

*Retrospective multi-cycle assessment:*
- NED Cumulative Assessment Report (retrospective evaluation spanning all prior grants in a multi-year grantee relationship; assesses accumulated impact across cycles)

*Learning embedded in portfolio design:*
- Gates Foundation Learning for Impact (evaluation designed to generate lessons applicable across the portfolio, not only to the evaluated program)
- Rockefeller Foundation Strategic Learning Blueprint (learning embedded in strategy, not added after)

---

## Measurement Primitives

### Disaggregation (Data Quality Standards applied to population scope)

**Definition reference:** Primitives Foundation Layer 4 (Data Quality Standards).

**What it identifies:** The requirement that outcome data be broken down by demographic and status categories established at the start of the program, which cannot be removed in later reporting periods.

**Framework exemplars:**

*Statutory disaggregation requirements:*
- Perkins V CTE (eight special population categories fixed by statute: gender, race/ethnicity, disability, English learner, economically disadvantaged, single parent, migrant, youth in foster care)
- WIOA (gender, race/ethnicity, disability, veteran status mandatory at enrollment, carried through exit and outcome measurement)
- ESIF ESF+ Common Indicators Toolbox (participant-level indicators covering age, gender, employment status, education level, household situation; mandatory across all 27 member states)

*Client-level longitudinal linking as the strongest disaggregation form:*
- SAMHSA NOMs / GPRA (client-level interview at baseline, reassessment, discharge; eUCI linking not mandatory but QxQ codebooks enforce field-level consistency)
- Ryan White HIV/AIDS RSR (encrypted unique client identifier linking clients across subrecipients and program years; individual HIV clinical trajectories maintained)
- HMIS / HUD CoC (client-level data required; entry/exit/service records linked by client ID)

*Equity lens as formal disaggregation mandate:*
- SNAP-Ed Evaluation Framework 2024 (explicit equity lens requirement: race, ethnicity, income, geography)
- NCRP Racial Equity Grantmaking Criteria (disaggregation by race and geography as a core criterion)
- Equitable Evaluation Initiative (disaggregation by the populations being served as a pre-publication requirement)

---

### Evidence Form Specification (WALKRI Core Primitive)

**Definition reference:** Primitives Foundation Layer 4 (Criterion Specification Elements, Data Quality Standards).

**What it identifies:** For every intake field, the requirement that what evidence must be submitted to satisfy the field (the evidence form) is specified before any applicant or participant sees the field. Evidence form is distinct from evidence strength: it specifies the format and source of evidence required, not the quality level.

**Framework exemplars by evidence form type:**

*Lab-based evidence forms:*
- Ryan White HIV/AIDS RSR (viral load laboratory report; CD4 count laboratory result)
- PCORI (primary outcome instrument specified in registered study protocol)

*Document-based evidence forms:*
- 2 CFR 200 (financial reports, audit documentation, progress narrative)
- GFGP ARS 1651 (organization-level financial and governance documentation)
- INPAS (grant restriction documentation at recognition)

*Self-report with conformance threshold:*
- LIHEAP (energy burden documentation; utility disconnection notice)
- SAMHSA NOMs (structured client interview; QxQ codebooks)
- IAF Grassroots Development Framework (field observation; documentation to be specified at indicator selection)

*Registry or system submission as evidence form:*
- PCORI (protocol registered in OSF, AsPredicted, or ClinicalTrials.gov)
- Verra VCS (Monitoring Report submitted through Verra registry)
- HMIS (client record submitted through local HMIS system)
- SPARS (SAMHSA Performance Accountability and Reporting System)
- SBIR/STTR database (commercialization outcomes reported through sbir.gov)

---

### Organizational Identity Anchor

**Definition reference:** Primitives Foundation Layer 2 (Entity Boundary, Disbursement Authority, On-chain Identity Anchor).

**What it identifies:** The set of verifiable attributes that establish who the applying organization is, what it controls, and who has authority to act on its behalf. Without an identity anchor, accountability claims have no subject.

**Framework exemplars:**

*Formal organizational standards:*
- GFGP ARS 1651 (African Organisation for Standardisation grant management standard; 300+ requirements covering organizational capacity, governance, financial systems, accountability; ISO submission accepted)
- 2 CFR 200 (Uniform Administrative Requirements, Cost Principles, and Audit Requirements for Federal Awards; organizational identity anchor as baseline for all US federal grants)
- INPAS International Non-Profit Accounting Standard (grant restriction classification at recognition; organizational financial identity)
- NNFS Fiscal Sponsorship Guidelines (fiscal sponsor as identity anchor for sponsored projects without independent legal status)

*On-chain identity:*
- DAOIP-5 (DAO identity specification; wallet-anchored organizational identity for on-chain grant programs)
- Optimism Retro Funding (wallet address as identity anchor; attestation corpus linked to address)

---

### Coherence Disclosure

**Definition reference:** Primitives Foundation Layer 3 (implied by scope and concurrent funding; not yet a named standalone primitive in the Foundation).

**What it identifies:** The declaration of how a program relates to other interventions in the same problem area, preventing duplication and enabling funders to understand the program's position in a broader ecosystem of responses.

**Framework exemplars:**

*Coherence as a formal evaluation criterion:*
- OECD DAC criteria (coherence as one of five evaluation criteria; formally distinct from relevance and effectiveness)
- EU ESIF CPR evaluation framework (coherence criterion: how the program relates to other EU policy instruments)
- Core Humanitarian Standard (CHS Commitment 6: coordinated and complementary humanitarian response)

*Concurrent funding disclosure as coherence mechanism:*
- CROSS Part VI (concurrent funding disclosure; all sources covering the same scope must be declared)
- Gates Foundation Evaluation Policy (portfolio learning includes understanding how programs relate to each other)

*Portfolio coherence at the network level:*
- CGIAR MELIA (system-level evaluation of how CGIAR centers' programs relate to each other and to national agricultural research systems)
- OCHA CBPF (pooled fund coherence with bilateral donor programming in humanitarian contexts)

---

### Affected Population Verification

*Note: this concept is now in the Primitives Foundation as the Affected Population Verification Gate, a configuration of Evidence Strength (Layer 4) as of v0.2.0. It was first added as a standing primitive (the Beneficiary Accountability Gate, renamed Affected Population Verification Gate at v0.1.7) and folded to a configuration in the v0.2.0 demotion pass; the mechanism it names is unchanged.*

**What it identifies:** A formally structured mechanism through which the affected population of a grant program can provide feedback, raise complaints, and receive responses, with the mechanism's design and operation specified before the program begins. This is distinct from outcome measurement (which measures what happened to the affected population) and from stakeholder engagement in research design (which includes the affected population in designing the program). Affected population verification is the ongoing channel through which the affected population can influence the program in real time.

**Framework exemplars:**

*Most formally specified:*
- CRS ProPack II (Community feedback loops and complaint response mechanisms as required MEAL system components; not optional add-ons)
- World Vision LEAP (Community Based Feedback and Response Mechanism integrated across all six programme cycle components)

*Referenced in international humanitarian standards:*
- Core Humanitarian Standard (CHS Commitment 5: communities and people affected by crisis have access to safe and responsive mechanisms to handle complaints)
- Caritas Internationalis CIMS (accountability to communities in the MEAL framework)
- OECD DAC (accountability dimension in evaluation criteria)

---

## Primitives Identified as New - Disposition in the v0.2.0 Reduction

These structural concepts were identified during the framework compatibility research as candidates for a future Foundation revision. The 2026 reduction that produced the v0.2.0 basis has since resolved most of them, and each is marked with its current disposition. Each remains exemplified by at least one covered framework.

**Inter-cycle Reflection Stage**
A formally required stage between the close of one programme cycle and the opening of the next, in which learning from the completed cycle is reviewed and institutionalized before the next design phase begins. Distinct from the completion gate (which closes the current cycle) and the entry gate (which opens the next). Exemplified by: World Vision LEAP Reflect stage. Potentially related to: USAID CLA adaptive management loops; Developmental Evaluation.
**Disposition (v0.2.0):** Seated, as a configuration of Program Learning Architecture (Layer 7); it is the minimum expression of that primitive, declared when only the cumulative-sequence-linkage element is present.

**Multi-cycle Retrospective Assessment**
A formal evaluation spanning all prior grant cycles in a multi-year grantee relationship, assessing accumulated impact across the full history rather than the most recent cycle only. Requires that indicator specifications from all prior cycles be preserved in comparable form. Exemplified by: NED Cumulative Assessment Report (required for renewed multi-year NED grantees). No other covered framework currently exemplifies this primitive.
**Disposition (v0.2.0):** Seated as a standing primitive (Portfolio, Layer 7).

**Portfolio-level Continuation Benchmark**
A published performance threshold applied to a funder's entire grant portfolio rather than to individual grants, where failure of the portfolio to meet the threshold triggers compliance consequences for the funder rather than for individual grantees. Exemplified by: SBIR/STTR Phase I-to-II transition rate minimum (0.25) and commercialization revenue benchmark (USD 100,000 per Phase II award average). No other covered framework currently exemplifies this primitive at the statutory level.
**Disposition (v0.2.0):** Seated as a standing primitive (Portfolio, Layer 7).

**Regulatory Approval Pathway as Terminal Gate**
A terminal evaluation gate defined not by a funder's completion criteria but by an external regulatory body's approval decision. The grant or OT contract is structured so that regulatory approval (e.g., FDA market authorization for a medical countermeasure) constitutes the equivalent of the completion gate outcome evidence. Exemplified by: BARDA OT contracts for medical countermeasure development (FDA approval pathway as terminal evaluation gate). Related to: ARPA-H payable milestone structure, but distinct because the terminal gate is external to both funder and grantee.
**Disposition (v0.2.0):** Open. Not seated in the 146-primitive basis; it sits with the External Outcome Standard Binding Condition in the unratified gap-pass tier the author rules on, the case where the completion gate is defined by an external standard's verdict rather than the funder's own criteria.

---

## How to Use This Index

**Classifying a new framework:** Identify which primitive the framework most clearly exemplifies. Check the exemplars listed under that primitive. If the new framework exemplifies the primitive in a way substantially covered by existing exemplars, a Tier 2 README table entry is sufficient. If it exemplifies the primitive in a structurally novel way (a new governance level, a new evidence form, a new mechanism), a Tier 1 compatibility statement is warranted.

**Building program type bundles:** Each bundle combines CROSS runbook provisions + WALKRI field specifications + compatibility mapping. The compatibility mapping in each bundle can reference this index rather than listing all covered frameworks: "programs of this type typically exemplify the following primitives, which are addressed by CROSS provisions X, Y, Z."

**Identifying gaps:** Frameworks that exemplify primitives not yet listed in this index are candidates for new compatibility statements. Frameworks that exemplify one of the four new candidate primitives at the bottom of this document are particularly valuable, as they would help establish whether those primitives are genuinely generalizable or specific to their current exemplar.

---

## Changelog

- **0.2.0 (2026-06-07):** Refreshed to the Primitives Foundation v0.2.0, the 146-primitive basis. Front matter foundation reference updated from 0.1.3. Added two exemplar-rich obligation primitives the v0.2.0 reduction produced: the Allocation Rule (the combinatory allocation act, with framework exemplars across its eight configuration values from quadratic funding to lottery) and Financing Instrument Type (pure grant, repayable grant, concessional loan, blend). Corrected stale classifications: Theory of Change Hierarchy now references Layer 6 and the folded Theory Layer; Sustainability Stance moved to Layer 6; the Affected Population Verification note now records that the concept was seated as a primitive and then folded to a configuration of Evidence Strength. Reframed the candidates section as a disposition record: Inter-cycle Reflection Stage (now a configuration of Program Learning Architecture), Multi-cycle Retrospective Assessment, and Portfolio-level Continuation Benchmark are seated, while Regulatory Approval Pathway as Terminal Gate remains open in the unratified gap-pass tier. The index stays selective by design, covering the primitives that generate the most significant external framework alignments rather than all 146.
- **0.1.0 (2026-05-19):** Initial release. Selective framework-exemplar index mapping obligation, gate, measurement, and cohort-facing primitives to the external frameworks that most clearly exemplify them, with a candidates-for-revision section and usage guidance.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
