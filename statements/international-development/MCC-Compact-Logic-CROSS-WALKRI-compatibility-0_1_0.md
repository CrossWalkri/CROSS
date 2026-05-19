---
title: MCC Compact Logic Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/cross-walkri/CROSS), WALKRI v0.1.6 (github.com/cross-walkri/WALKRI)
references:
  - MCC Policy for Monitoring and Evaluation (mcc.gov/resources/doc/policy-for-monitoring-and-evaluation)
  - MCC Compact Logic hierarchy and Results Framework requirements
  - USAID ADS 201 Program Cycle Policy
---

# MCC Compact Logic Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

CROSS's Theory of Change architecture is structurally identical to the MCC Compact Logic hierarchy. This is not an approximation or a post-hoc alignment: CROSS adopted the MCC four-level hierarchy directly as its ToC architecture. A CROSS-conformant program produces MCC Compact Logic documentation as a structural output of conformance, without requiring translation or additional documentation.

WALKRI complements this by ensuring the intake fields collecting indicator data at each Compact Logic level are measurement instruments. The MCC M&E Policy's requirements for pre-implementation results frameworks, quantitative benchmarks, and baselines before activities start are each addressed by specific CROSS and WALKRI provisions.

---

## What the MCC Compact Logic Is

The Millennium Challenge Corporation uses a four-level logic hierarchy to organize the causal architecture of all compacts and threshold programs. MCC calls this hierarchy the Compact Logic:

**Activity**: The specific actions, investments, and interventions funded by the compact. Activities produce outputs.

**Output**: The direct products of activities: the deliverables, infrastructure, services, or trained individuals that activities produce. Outputs are fully within the implementing entity's control.

**Objective**: The near-term results that outputs are expected to contribute to: the changes in behavior, access, capacity, or conditions that follow from outputs. MCC's Objective level corresponds to what other frameworks call intermediate outcomes or short-term outcomes.

**Goal**: The long-term development outcome the compact is designed to contribute to: usually expressed in terms of poverty reduction, economic growth, or improved welfare at the population level.

The MCC M&E Policy requires a results framework at each level before implementation begins. It requires quantitative benchmarks for each indicator, baselines collected before activities start, targets with explicit assumptions documented, and independent evaluation separated from performance monitoring. These requirements apply to both compact M&E systems and threshold program M&E systems.

---

## How CROSS Satisfies the MCC Compact Logic

### Structural Identity of the Hierarchy

CROSS's Theory of Change architecture (Part IX-B) uses a four-level causal hierarchy: Activity, Output, Outcome, Goal. This is the same hierarchy as MCC's Compact Logic, with one terminological difference at the third level (CROSS uses "Outcome" where MCC uses "Objective").

The CROSS README states this relationship explicitly: "The architecture follows the Compact Logic hierarchy used by MCC and USAID, making CROSS ToC declarations natively compatible with those frameworks without requiring separate documentation."

The level correspondence is direct:

| MCC Compact Logic Level | CROSS ToC Level | Notes |
|:--|:--|:--|
| Activity | Activity | Identical |
| Output | Output | Identical |
| Objective | Outcome | CROSS uses "Outcome"; meaning and causal position are identical |
| Goal | Goal | Identical |

Because the hierarchy is identical, a CROSS ToC declaration is a Compact Logic declaration. Programs do not need to produce a separate Compact Logic document; the CROSS ToC declaration is that document.

### Pre-Implementation Results Framework

The MCC M&E Policy requires that a results framework be finalized before implementation begins: every indicator must be specified at its appropriate Compact Logic level with baseline, target, and data source documented in advance.

CROSS addresses this through its gate architecture. The pre-application gates (Parts III through V) require that the full indicator specification be completed before the round opens and before any applicant submits a proposal. The eleven-field indicator specification (Part V) requires: indicator name, definition, unit, baseline, target, population scope, data source, collection frequency, responsible party, institutional framework alignment, and causality stance. This specification is completed at the program configuration stage, which corresponds to the MCC pre-implementation stage.

Because CROSS indicators are declared at a specific ToC level (output or outcome), the results framework structure maps directly to the Compact Logic level structure: output-level indicators are Output indicators in MCC terms; outcome-level indicators are Objective indicators in MCC terms.

### Quantitative Benchmarks

The MCC M&E Policy requires quantitative benchmarks for each indicator. In MCC usage, benchmarks are intermediate milestones between baseline and final target: they allow the M&E system to assess whether a program is on track before the compact ends.

CROSS's progress verification gate architecture (Part IV, Section 4.2) requires the program to specify evidence scope and strength thresholds at each gate. These thresholds are the operational form of MCC's quantitative benchmarks: they define what evidence is required at each stage of the program to demonstrate progress toward the final target. A gate configured at a specific evidence strength level is a structured benchmark rather than an ad hoc check.

### Baselines Before Activities Start

The MCC M&E Policy explicitly requires that baseline values be collected before activities start. Baseline data collected after activities begin is inadmissible as a baseline under MCC M&E standards.

CROSS enforces this requirement through the indicator specification's temporal architecture. Field 4 (baseline value) in the CROSS eleven-field specification is a pre-commitment field: it must be populated before the round opens and before any grantee activity begins. The CROSS gate sequence does not permit a round to open with unspecified baselines.

WALKRI strengthens this. A WALKRI-conformant baseline field specifies the counting rule, population boundary, time period, and the evidence artifact that must be produced to verify the baseline value. This means a baseline cannot be entered as a number without an evidence trail establishing when it was collected and what method produced it. The temporal integrity of the baseline is built into the field specification, not dependent on reviewer vigilance.

### Targets with Explicit Assumptions

The MCC M&E Policy requires that targets be accompanied by documented assumptions: the conditions that must hold for the program to achieve the target from the baseline. These assumptions are treated as testable claims rather than background context.

CROSS addresses this through two provisions. Field 5 (target value) specifies the TO state, and the pathway registry's critical assumptions list (Part IX-B, Section 3) specifies the conditions that must hold for each causal pathway to produce the expected result. The assumptions list is a mandatory component of the pathway declaration, not an optional annotation. A CROSS-conformant program produces a documented set of pathway assumptions for every outcome it claims to target.

### Independent Evaluation

The MCC M&E Policy requires that independent evaluation be separated from performance monitoring. Performance monitoring (tracking against pre-defined indicators) is the responsibility of the implementing entity; independent evaluation (assessing whether the compact caused the observed change) requires a methodology that does not depend on the implementing entity's self-reported data.

CROSS's causality stance primitive (Part IV) provides the structural basis for this distinction. A gate configured at contribution stance corresponds to performance monitoring: evidence that activities contributed to outcomes, with co-factors acknowledged. A gate configured at attribution stance corresponds to independent evaluation: evidence that the intervention produced change above the level expected without it, typically requiring counterfactual reference data.

Programs implementing MCC-aligned compacts can configure their performance monitoring gates at contribution stance and designate specific evaluation gates at attribution stance, producing the separation of monitoring and evaluation that MCC's M&E Policy requires within the CROSS gate architecture.

---

## MCC M&E Policy Requirements vs CROSS Provisions

| MCC M&E Policy Requirement | CROSS Field or Procedure |
|:--|:--|
| Results framework finalized before implementation | Parts III-V: indicator specification completed before round opens |
| Indicator name and definition | Field 1: Indicator name; Field 2: Definition |
| Unit of measure | Field 3: Unit (embedded in specification) |
| Baseline value before activities start | Field 4: Baseline value (required pre-commitment) |
| Quantitative benchmark milestones | Progress verification gates with evidence scope and strength thresholds (Part IV, Section 4.2) |
| Final target with documented assumptions | Field 5: Target value; pathway registry critical assumptions list (Part IX-B) |
| Data source and collection methodology | Field 7: Data source; Field 8: Collection frequency |
| Responsible party for data collection | Field 9: Responsible party |
| Institutional framework alignment | Field 10: Institutional framework alignment |
| Performance monitoring vs independent evaluation | Contribution stance (monitoring) vs attribution stance (evaluation), set at gate level (Part IV) |
| Baselines verified before implementation | WALKRI evidence form requirement for baseline fields |

---

## WALKRI and MCC Data Quality Standards

MCC's M&E Policy requires that data quality be assessed for all performance indicators and that the assessment be documented before data are used for reporting. Data quality criteria in MCC guidance align with the standard five-criteria set: validity, reliability, precision, integrity, and timeliness.

These five criteria are identical to WALKRI's five data quality standards (Sections 5.1 through 5.5). A WALKRI-conformant field specification addresses all five criteria at the instrument design stage: before data collection begins, the field specification documents how the field produces valid, reliable, precise, integral, and timely data. This converts MCC's retrospective data quality assessment requirement into a prospective design requirement, which is a stronger position: a program that designs quality into its fields does not need to discover and remediate quality problems after collection.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
