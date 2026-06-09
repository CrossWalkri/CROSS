---
title: Innovate UK and UKRI Evaluation Framework and Impact Management Framework Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - UK Research and Innovation (ukri.org)
  - Innovate UK Evaluation Framework: How we assess our impact on business and the economy (https://www.ukri.org/publications/evaluation-framework/)
  - Innovate UK Evaluation Framework PDF (https://www.ukri.org/wp-content/uploads/2021/12/IUK-061221-EvaluationFrameworkV2FinalWeb.pdf)
  - Innovate UK Impact Management Framework (https://iuk-business-connect.org.uk/perspectives/introducing-our-impact-management-framework/)
  - Project Impact guidance for applicants (https://www.ukri.org/councils/innovate-uk/guidance-for-applicants/project-impact-guidance/)
  - What the Project Impact questions cover (https://www.ukri.org/councils/innovate-uk/guidance-for-applicants/project-impact-guidance/what-the-project-impact-questions-cover/)
  - HM Treasury Magenta Book (evaluation guidance for UK government)
  - HM Treasury Green Book (ROAMEF policy cycle)
lens_tags:
  calibration_tier: outcome_specified_self_reported
  authority_source: statutory
  cultural_methodological_lineage: western_institutional
  funder_typology: government_non_aid
  framework_scope_type: grantee_outcome_measurement
  # UK Research and Innovation under Higher Education and Research Act 2017
---

# Innovate UK and UKRI Evaluation Framework and Impact Management Framework

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

Innovate UK, the business-facing arm of UK Research and Innovation (UKRI), operates two paired but distinguishable documentation regimes. The Impact Management Framework is the grantee-facing component: it requires funded partners to answer the Project Impact questions annually throughout the project's lifespan and to continue answering them after project completion, with a universal set of metrics applied across all Innovate UK programs (full-time equivalent employees, turnover generated as a result of the support, new patents, designs, trademarks, copyrights, and related innovation and collaboration indicators) alongside per-program metrics tailored to specific funding schemes. The UKRI Evaluation Framework (published as "How we assess our impact on business and the economy") wraps around the Impact Management Framework as the institution-level evaluation methodology: it specifies how Innovate UK assesses itself, structured around the HM Treasury ROAMEF policy cycle (rationale, objectives, appraisal, monitoring, evaluation, feedback), the three evaluation types from the Magenta Book (process, impact, economic), a logic model template (inputs, activities, outputs, outcomes, impacts), and proportionate evaluation tiering based on budget and risk. CROSS+WALKRI satisfies both layers structurally, with three specific accommodations: the universal Project Impact metric set fits CROSS's pre-specified indicator architecture directly, the institution-level ROAMEF cycle maps to CROSS's gate architecture and obligation maturation tracking, and the Magenta Book's process/impact/economic evaluation typology requires a CROSS gate configuration that distinguishes deliverable verification from impact attribution. This compatibility statement is distinct from the Research Funder DMP Standards compatibility statement already in CROSS+WALKRI's coverage. The DMP standards address data management plans for academic research outputs. The Innovate UK regime addresses impact management for business and economic outcomes from publicly funded innovation support. The two regimes operate on different artifacts, target different beneficiary populations, and run on different reporting cadences.

---

## The Innovate UK and UKRI Framework Architecture

Innovate UK distributes public funding to businesses (predominantly small and medium enterprises) for research and development and innovation projects. Its evaluation and impact documentation regime has two named, formally published components, and the distinction between them matters for compatibility analysis.

The Impact Management Framework is the grantee-facing component. Its operative mechanism is the Project Impact questions, which are completed by applicants at application and by funded partners annually thereafter, with reporting continuing after project completion. The questions cover three domains: organizational metrics (employee numbers and changes), financial performance (turnover, profit, funding raised), and innovation and collaboration (research and development activity, new products, partnerships, patents, designs, trademarks, copyrights). A subset of the questions is universal: every Innovate UK funded partner answers the same metrics (notably full-time equivalent employee count and turnover generated as a result of the support), producing portfolio-level data that is commensurable across programs. A further subset is program-specific: tailored metrics activated by the funding scheme. The Impact Management Framework operates on a four-step cycle: planning and design, data collection, monitoring and reporting and evaluation, and innovating the approach.

The UKRI Evaluation Framework is the institution-level evaluation methodology. Its operative document is the published PDF "How we assess our impact on business and the economy," which sets out the guiding principles Innovate UK uses to design and commission evaluations of its own programs. It builds on HM Treasury's Magenta Book and Green Book, the European Commission's evaluation guidance, and the evaluation strategy of the Department for Business, Energy and Industrial Strategy. The framework specifies three evaluation types (process, impact, economic), each with a defined scope: process evaluations cover how a program was delivered, impact evaluations cover what difference the program made and to whom (including unintended outcomes), and economic evaluations (cost-effectiveness analysis and cost-benefit analysis) cover whether the benefits justify the costs. It situates evaluation within the ROAMEF policy cycle (rationale, objectives, appraisal, monitoring, evaluation, feedback) and recommends a proportionate evaluation tiering matrix that calibrates evaluation depth against budget and risk (Level 1: light-touch internal evaluation, Level 2: externally commissioned with appropriate budget, Level 3: detailed externally commissioned evaluation with 1 to 5 percent of total program budget). The framework explicitly recognizes the methodological challenges specific to evaluating innovation support: data paucity, heterogeneity across beneficiary firms, low observability of knowledge spillovers, fluidity of company structures, long-tailed and lagged effects, attribution difficulty in a complex science and innovation system, endogeneity in econometric models, and strategic behavior by firms responding to program incentives.

The two frameworks are not redundant. The Impact Management Framework collects the data the Evaluation Framework analyzes. The Evaluation Framework specifies the methodology Innovate UK applies to that data when it commissions an evaluation of one of its own programs. A funded partner interacts directly with the Impact Management Framework (by completing Project Impact questions); the Evaluation Framework operates at the institutional level and is the standard against which Innovate UK demonstrates accountability for public funding to UK taxpayers and to its parent department.

The logic model template in the UKRI Evaluation Framework is worth noting separately. It specifies five stages for an R&D grant program: inputs (public funding), activities (R&D projects), outputs (technological development), outcomes (new products sold), and impacts (economic growth). This is the inputs/activities/outputs/outcomes/impacts variant of the standard logic model vocabulary, with attribution intent at each stage made explicit by the framework's discussion of additionality, deadweight, displacement, substitution, leakage, and knowledge diffusion.

---

## How CROSS Satisfies the Innovate UK and UKRI Framework

CROSS satisfies both the grantee-facing Impact Management Framework and the institution-level UKRI Evaluation Framework, with explicit accommodations for the specific structural features of each.

**Universal Project Impact metrics and the pre-specified indicator set.** The Impact Management Framework's universal Project Impact metrics correspond directly to CROSS's pre-specified indicator set declared at the entry specification gate. The universal metrics (full-time equivalent employee count, turnover generated as a result of the support, new innovation and collaboration outputs) are established by Innovate UK before any application is submitted and apply uniformly across all funded partners. This is precisely what CROSS's entry specification gate requires: the indicator set is funder-published, not applicant-proposed, and the applicant's obligation at the completion and continuation gates is to produce evidence against those pre-specified indicators. Program-specific metrics added on top of the universal set correspond to CROSS's gate configuration mechanism for activating dimension-specific indicators by round configuration.

**Annual reporting throughout and after project lifespan.** The Impact Management Framework's requirement that funded partners answer Project Impact questions annually throughout the project and continue after project completion corresponds to CROSS's progress verification gate and attestation corpus provisions. CROSS's progress verification gate structure applies during the project: at each annual reporting interval, evidence against the pre-specified indicator set is submitted before the next reporting period proceeds. The continued post-completion reporting corresponds to CROSS's attestation corpus concept extended beyond the grant period, with a pre-declared long-tail attestation schedule that reflects the multi-year tail of innovation impacts. CROSS's attestation corpus provisions, applied to Innovate UK programs, require that the post-completion reporting horizon be documented at the entry gate as a known post-grant obligation to the funder and the funder's parent department under the funder's Part XI declarations.

**Logic model template and CROSS's Theory of Change hierarchy.** The UKRI Evaluation Framework's logic model (inputs, activities, outputs, outcomes, impacts) maps onto CROSS's output, outcome, and impact tiers. CROSS's output tier corresponds to outputs in the logic model (technological development, deliverables produced). CROSS's outcome tier corresponds to outcomes in the logic model (new products sold, increased business performance). CROSS's impact tier corresponds to impacts in the logic model (economic growth attributable to the program). The inputs and activities stages of the logic model are upstream of CROSS's gate architecture: they specify what the funder commits and what the funded partner does, which CROSS handles through the sufficiency architecture declaration (resources at the declared scope) and the development stage declaration (what the funded work consists of).

**ROAMEF cycle and CROSS's gate architecture.** The HM Treasury ROAMEF policy cycle (rationale, objectives, appraisal, monitoring, evaluation, feedback) within which the UKRI Evaluation Framework sits maps onto CROSS's gate architecture and obligation maturation tracking. Rationale and objectives correspond to the entry specification gate's published gate configuration: the funder declares what the program is for and what it must demonstrate before any applicant submits. Appraisal corresponds to gate assessment at entry: the funder evaluates applications against the published criteria. Monitoring corresponds to CROSS's progress verification gates. Evaluation corresponds to CROSS's completion verification gate, with the Evaluation Framework's three evaluation types (process, impact, economic) configuring the evidence scope and evidence strength at the completion gate. Feedback corresponds to CROSS's obligation maturation tracking: a funder operating across rounds records gate configurations and learnings, producing a versioned record of funder learning visible to the field over time.

**Proportionate evaluation tiering and CROSS's gate configuration calibration.** The Evaluation Framework's three-level proportionate evaluation tiering (Level 1 light-touch, Level 2 externally commissioned, Level 3 detailed externally commissioned with 1 to 5 percent of program budget) corresponds to CROSS's gate configuration calibration: the evidence strength required at each gate is set by the funder before the round opens, calibrated to the scale and public impact claim of the program. CROSS's Coordination Scaling Standard provides this calibration. A small Innovate UK Smart award and a large Catapult center are not subject to the same evaluation rigor; CROSS encodes this proportionality through evidence strength tiering rather than through evaluation level designation, but the structural intent is the same.

**Process, impact, and economic evaluation typology.** The Magenta Book's three evaluation types are operative within the Evaluation Framework. Process evaluation corresponds to CROSS's completion gate evidence at output strength (deliverables exist, were delivered as specified). Impact evaluation corresponds to CROSS's completion gate evidence at outcome strength (measured changes in the affected population) with attribution methodology specified at the gate configuration. Economic evaluation corresponds to CROSS's completion gate evidence at impact strength (verifiable causal link between the funded work and the measured change, supported by named methodology sufficient to support causal inference, including monetized cost-benefit assessment). CROSS's gate configuration must distinguish between these three evidence scopes at the time of round publication; the Evaluation Framework's evaluation type designation is the practical instrument by which Innovate UK selects which scope applies to a given program.

**Additionality, deadweight, and CROSS's additionality delineation.** The Evaluation Framework's treatment of additionality (the difference an intervention made against what would have happened anyway, with deadweight, displacement, substitution, and leakage as the wider effects to be measured) corresponds to CROSS's additionality delineation requirement in the sufficiency architecture declaration (Part IV) and in Part VI-A's concurrent funding attribution. The Evaluation Framework's recognition that partial additionality will be common, and that evaluations should enable partial additionality to be captured and quantified, is consistent with CROSS's treatment of additionality as a declared and assessed dimension rather than a binary qualifier.

| Innovate UK and UKRI Provision | CROSS Provision |
|:--|:--|
| Universal Project Impact metrics applied across all programs (FTE, turnover, patents, designs, trademarks, copyrights) | Pre-specified indicator set declared by funder at entry specification gate |
| Program-specific Project Impact metrics tailored to funding scheme | Gate configuration mechanism for dimension-specific indicators activated by round configuration |
| Annual reporting by funded partners throughout project lifespan | Progress verification gates with evidence submitted at each annual reporting interval |
| Reporting continuing after project completion | Attestation corpus with pre-declared long-tail post-grant schedule documented at entry gate |
| Logic model (inputs, activities, outputs, outcomes, impacts) | CROSS output, outcome, and impact tiers; inputs and activities handled through sufficiency architecture and development stage declarations |
| ROAMEF policy cycle (rationale, objectives, appraisal, monitoring, evaluation, feedback) | Gate architecture (entry specification, progress verification, completion verification, continuation specification) with obligation maturation tracking |
| Proportionate evaluation tiering (Level 1, Level 2, Level 3) | Gate configuration calibration via evidence strength tiering and Coordination Scaling Standard |
| Process evaluation (how the program was delivered) | Completion gate evidence at output strength |
| Impact evaluation (what difference the program made and to whom) | Completion gate evidence at outcome strength with attribution methodology specified in gate configuration |
| Economic evaluation (cost-effectiveness, cost-benefit) | Completion gate evidence at impact strength with causal inference methodology specified in gate configuration |
| Additionality, deadweight, displacement, substitution, leakage, knowledge diffusion | Additionality delineation in sufficiency architecture declaration (Part IV) and concurrent funding attribution (Part VI-A) |
| Innovation-specific evaluation challenges (data paucity, heterogeneity, low observability, lagged effects, endogeneity) | Acknowledged in gate configuration as constraints on evidence strength; addressed through development stage declaration and proportionate evidence requirements |

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication field requirements address the operational definition problem that arises at the intersection of the Impact Management Framework and the UKRI Evaluation Framework. The universal Project Impact metrics are named at the category level by Innovate UK (FTE, turnover, patents, designs, trademarks, copyrights), but the field-level operational definitions vary across funded partners in ways that produce data quality issues that the Evaluation Framework itself acknowledges (data paucity, heterogeneity, and the difficulty of attributing observed performance changes to the funded work). A funded partner answering "turnover generated as a result of this support" is making an attribution judgment whose operational definition is not specified at the field level: does "as a result of" mean direct attribution to a single product, partial attribution across a portfolio, or causal attribution net of counterfactual performance? Different partners reasonably answer this question differently.

WALKRI's five requirements applied to each universal Project Impact metric before any funded partner encounters the question would resolve this at source. The criterion intent field establishes what Innovate UK is trying to measure with the metric and why. The operational definition field specifies exactly what counts: what is the time window for turnover attribution, what counts as a direct attribution versus a partial attribution, and what counts as a sufficiently demonstrated causal link. The response form field specifies what the partner records and in what format (numeric value, attribution percentage, narrative). The evidence form field specifies what documentation supports the recorded value (audited accounts, product launch records, customer attribution surveys). The conformance threshold field specifies what level of attribution constitutes a reportable claim, distinguishing substantive program-attributable turnover from incidental revenue growth.

WALKRI applied at the program-specific metric layer (the Impact Management Framework's per-program metrics) is equally important. Innovate UK runs many programs with different focal outcomes; if each program adds its own metrics to the universal set, the field-level definitions of those program-specific metrics must be specified before funded partners encounter them, or the same operational ambiguity that affects the universal metrics will be reproduced at greater scale. WALKRI's pre-publication requirements applied at both layers produce an Impact Management Framework dataset that is commensurable both within programs and across the Innovate UK portfolio, supporting the cross-program analysis that the Evaluation Framework is designed to enable when it commissions impact evaluations of innovation support.

WALKRI also addresses the logic model fields directly. The UKRI Evaluation Framework's logic model lists inputs, activities, outputs, outcomes, and impacts as the path along which monitoring and evaluation data must be captured. WALKRI requires that the construct, metric, unit, baseline, and evidence threshold be specified for every field at every stage of that path before any partner encounters the field. This converts the logic model from a graphic that illustrates expected program logic into a measurement instrument that produces commensurable data, which is the transformation the Evaluation Framework's discussion of monitoring requirements (page 15 of the published PDF) implicitly requires but does not specify at the field level.

---

## Distinction from Research Funder DMP Standards Compatibility

This compatibility statement is independent of CROSS+WALKRI's existing alignment with Research Funder Data Management Plan (DMP) standards. The two regimes are not substitutes.

Research Funder DMP standards (covering the seven UK Research Councils' DMP requirements and equivalent standards at NIH, NSF, the European Research Council, and other research funders) address how academic research data is stored, curated, made findable, and shared. The artifact is the data management plan, submitted at application and updated through the grant. The affected population is the scholarly community and downstream researchers who reuse the data.

The Innovate UK and UKRI evaluation and impact regime addresses how publicly funded business innovation support produces measurable economic outcomes. The artifact is the Project Impact submission and the institutional evaluation commissioned against it. The affected population is UK businesses and the UK economy as a whole. Innovate UK funds businesses rather than academic researchers; the outputs being measured are turnover, employment, patents, and product launches rather than datasets, publications, and research methods.

A program that satisfies one regime does not thereby satisfy the other. A research council program that funds academic research with strong DMP requirements does not have to operate the Impact Management Framework. An Innovate UK program that requires Project Impact answers from a small business does not have to operate the Research Funder DMP standards. The two regimes coexist within UKRI but operate on different artifacts, target different affected populations, and run on different reporting cadences.

CROSS+WALKRI covers both regimes through its modular gate architecture: a program adopting CROSS specifies in its gate configuration which external standards it incorporates as gate criteria. A research council program incorporates the relevant DMP standard. An Innovate UK program incorporates the Impact Management Framework's universal and program-specific Project Impact metrics. The two configurations are independently conformant with CROSS without either standard subsuming the other.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
