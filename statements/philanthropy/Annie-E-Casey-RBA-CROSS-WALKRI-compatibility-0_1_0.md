---
title: Annie E. Casey Foundation and Results-Based Accountability (RBA) Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.4 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - https://www.aecf.org/resources/a-road-to-results-a-performance-measurement-guidebook
  - https://www.aecf.org/resources/a-road-to-results-results-based-accountability-in-the-annie-e-casey-founda/
lens_tags:
  calibration_tier: outcome_specified_self_reported
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: private_foundation
  framework_scope_type: grantee_outcome_measurement
  # Annie E. Casey Foundation Results-Based Accountability
---

# Annie E. Casey Foundation and Results-Based Accountability (RBA) Compatibility - CROSS+WALKRI

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

This statement documents structural alignment between the Annie E. Casey Foundation's formally adopted Results-Based Accountability (RBA) framework and the CROSS+WALKRI specification standards. The Annie E. Casey Foundation incorporated RBA, developed by Mark Friedman, as its grantee measurement model and formalized it in Letters of Agreement with grantees. RBA's three performance metrics (quantity, quality, and effect) and its distinction between population accountability and performance accountability map directly to CROSS's Theory of Change hierarchy and obligation modes. WALKRI ensures that intake fields collecting RBA metric data are measurement instruments before any applicant encounters them.

---

## The RBA Framework and Annie E. Casey Foundation's Adoption

Results-Based Accountability was developed by Mark Friedman and described in the foundational text "Trying Hard Is Not Good Enough." The framework distinguishes two fundamentally different accountability domains, and this distinction is its most analytically significant contribution relative to standard logic model approaches.

The first domain is population accountability: measuring community-level conditions of well-being, independent of any specific program or intervention. Population accountability asks whether things are getting better for a defined community, regardless of who is responsible or what programs are operating. It requires population-level indicators, baselines, and trend data. The question is not whether a program worked; the question is whether the underlying condition in the community is improving.

The second domain is performance accountability: measuring how well a specific program or service is performing. Within performance accountability, RBA defines three metrics. Quantity asks how much the program did: how many people were served, how many activities were conducted, how many sessions were delivered. Quality asks how well the program did it: whether services were delivered with fidelity, whether clients found the services useful, whether the program met its own standards for delivery. Effect asks whether anyone is better off: whether participants experienced measurable changes in knowledge, skills, attitudes, behaviors, or conditions as a result of the program.

The Annie E. Casey Foundation's two published framework documents, "A Road to Results: A Performance Measurement Guidebook" and "A Road to Results: Results-Based Accountability in the Annie E. Casey Foundation's Education Program," formalized this model as the Foundation's grantee measurement standard. Grantees were required to develop and report against all three performance metrics, and the accountability framework was incorporated into Letters of Agreement. The quantity/quality/effect structure is a named, distinct methodology; it is not reducible to standard logic model vocabulary, even though logic models cover overlapping territory.

RBA is widely adopted beyond AECF. Local governments in the United States and the United Kingdom have used it to structure public service accountability. The What Works Centres in the UK have referenced its vocabulary. The framework's durability reflects the analytical clarity of the population/performance distinction and the operational tractability of the quantity/quality/effect metric structure.

---

## How CROSS Satisfies the RBA Framework

CROSS's Theory of Change hierarchy and obligation modes implement the full RBA obligation-and-verification structure. The mapping is detailed below.

The RBA quantity metric corresponds to CROSS's output tier. Outputs are the activities conducted and the deliverables produced: sessions held, participants served, materials distributed, systems deployed. CROSS's Build obligation mode is the operative mode for programs where quantity measurement is the primary reporting obligation. The completion gate in Build mode requires deliverable specification: what outputs were committed, what evidence constitutes output completion, and what counts as a served participant. This is precisely what the RBA quantity metric requires to be answerable.

The RBA quality metric corresponds to CROSS's completion gate evidence quality specifications and CROSS's evidence strength taxonomy. Quality in RBA is about how well the output was produced, which requires evidence that goes beyond counting outputs; it requires evidence that the delivery met specified standards. CROSS's completion gate requires that evidence type and evidence strength be declared before applications open, and it requires that the evidence specification distinguish between delivery completion (quantity) and delivery quality. The evidence strength taxonomy provides the vocabulary for distinguishing anecdotal quality reports from systematic quality monitoring.

The RBA effect metric corresponds to CROSS's outcome tier and Change obligation indicators, specifically Fields 7 through 11 in the CROSS indicator specification. Effect in RBA asks whether anyone is better off, which is a question about measurable condition changes in participants or communities. CROSS's Change obligation mode is the operative mode for programs where effect measurement is required. Fields 7-11 require that target condition, baseline measurement, target threshold, measurement timing, and comparison group specification all be declared before the round opens. These fields operationalize the RBA effect question as a pre-specified measurement commitment rather than a post-hoc reporting exercise.

The RBA population accountability domain corresponds to CROSS's coherence disclosure and population scope declaration. CROSS requires that every round specification declare the population whose conditions the program is intended to affect and how the program's outcomes relate to broader population-level trends. This is functionally equivalent to the population accountability frame: it situates program-level performance within the community-level condition the program contributes to, without claiming that program-level outcomes determine population-level trends.

The following table summarizes the core mappings.

| RBA Domain or Metric | CROSS Mechanism |
|---|---|
| Quantity: how much did we do? | CROSS output tier; Build obligation completion gate deliverable specification |
| Quality: how well did we do it? | CROSS evidence quality specifications at completion gate; evidence strength taxonomy |
| Effect: is anyone better off? | CROSS outcome tier; Change obligation Fields 7-11 (target condition, baseline, threshold, timing, comparison group) |
| Population accountability: community conditions | CROSS coherence disclosure + population scope declaration |

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication field requirements ensure that intake fields collecting RBA metric data are measurement instruments before any applicant encounters them. An intake field that asks "how many participants will you serve?" is not a quantity measurement instrument unless it specifies what counts as a participant, what counts as a service unit, and over what time period the count applies. WALKRI requires that the construct, metric, unit, baseline, and evidence threshold be specified for every field before the field is presented to applicants. This ensures that the three RBA metrics are operationally defined before the intake process begins, not after data have been collected.

WALKRI also ensures that the population accountability frame is implemented as a measurement instrument rather than a rhetorical commitment. A round specification that describes the population and the community conditions being addressed must, under WALKRI, specify what population data source provides the baseline, what indicator tracks the community condition, and what change in that indicator would be considered relevant to the program's population-level contribution. This prevents the population accountability frame from functioning as a narrative framing device without measurement substance, which is the failure mode WALKRI is designed to prevent.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
