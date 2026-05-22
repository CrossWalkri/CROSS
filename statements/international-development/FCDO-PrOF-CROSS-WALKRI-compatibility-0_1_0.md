---
title: FCDO Programme Operating Framework Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - FCDO Programme Operating Framework, https://www.gov.uk/government/publications/fcdo-programme-operating-framework
  - IATI Standard v2.03, iatistandard.org
  - OECD DAC Evaluation Criteria, oecd.org/dac/evaluation/daccriteriaforevaluatingdevelopmentassistance.htm
  - CROSS+WALKRI IATI Compatibility Statement v0.1.0
  - CROSS+WALKRI OECD DAC CRS Compatibility Statement v0.1.0
---

# FCDO Programme Operating Framework Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS+WALKRI-conformant program satisfies FCDO Programme Operating Framework (PrOF) requirements through two structural pathways: OECD DAC alignment satisfies the evaluation criteria dimension, and IATI compatibility satisfies the transparency and data publication requirement. These two pathways cover the aspects of PrOF that are most directly relevant to specification-layer compliance.

CROSS is an obligation architecture. PrOF is a programme governance framework. They operate at adjacent layers: PrOF governs programme cycle management, financial accountability, and evidence standards for FCDO-funded spending; CROSS governs what funded interventions must specify, demonstrate, and disclose at each gate. A program using CROSS does not adopt PrOF; rather, a CROSS-conformant program produces the data structures and evidence records that PrOF compliance at the specification layer requires.

This compatibility is relevant for Web3 grants programs receiving FCDO co-financing, implementing partners seeking FCDO contracts, and programs structuring grant documentation for potential engagement with UK development finance.

---

## What PrOF Is

The FCDO Programme Operating Framework governs all FCDO programme spending. Updated in April and October 2025, it defines mandatory processes, evidence standards, and a results chain using OECD DAC criteria as the evaluation framework. PrOF applies to all FCDO programmes above a minimum expenditure threshold, covering bilateral aid, multilateral contributions routed through FCDO trust funds, and commercial contracts.

The PrOF programme cycle has three milestone-bearing stages. The design stage requires completion of a Programme Design Document (PDD) before implementation begins. The PDD must include a logframe or results chain, outcome indicators with baselines and targets, an evidence plan, and a risk register. The annual review stage requires systematic progress assessment against the results framework, with a formal annual review output that informs continuation decisions. The programme completion stage requires a Programme Completion Report (PCR) summarising results, learning, and evidence of achievement against the original targets.

Two cross-cutting requirements apply throughout: all activity data must be published to IATI and to DevTracker (the UK government's aid transparency portal), and OECD DAC evaluation criteria must be applied at review and completion stages.

---

## Two Compatibility Pathways

### Pathway One: OECD DAC Alignment

PrOF uses OECD DAC evaluation criteria as the mandatory evaluation framework. The five criteria are relevance, coherence, effectiveness, efficiency, and impact; sustainability was added as a sixth criterion in the 2019 revision. FCDO's annual review and PCR templates both require programmes to assess performance against these criteria.

CROSS Field 10 (institutional framework alignment) captures the external standards and frameworks to which a program's indicators are aligned. Programs declaring OECD DAC alignment in Field 10 produce documented alignment with the evaluation criteria that PrOF mandates. CROSS's Theory of Change architecture (goal, outcome, output, and activity levels with named causal links and assumptions) is the structural foundation for assessing effectiveness, impact, and sustainability at review. CROSS's causality stance field (contribution versus attribution) addresses the methodological framing that DAC evaluation practice requires when assessing impact in complex systems.

CROSS does not automate DAC criterion assessment. It produces the specification architecture that makes criterion assessment tractable: pre-specified FROM and TO states, pre-specified causal assumptions, and a gate-based evidence record. Evaluators applying DAC criteria to a CROSS-conformant program work from explicit theory of change claims and documented evidence rather than from post-hoc reconstruction.

### Pathway Two: IATI Compatibility

All FCDO activity data must be published to IATI and DevTracker. Any program receiving FCDO co-financing must therefore satisfy IATI reporting requirements. CROSS's IATI compatibility is separately documented in the CROSS+WALKRI IATI Compatibility Statement. Programs conformant with both CROSS and WALKRI produce IATI-compatible data as a structural consequence of the obligation architecture: gate records produce IATI transaction elements, indicator specifications produce IATI result elements, and the organizational identity anchor produces the IATI activity identifier.

Programs that have implemented CROSS under the IATI alignment pathway satisfy the FCDO transparency and data publication requirement without additional reporting workflow changes.

---

## Gate Architecture Mapping to PrOF Programme Cycle

CROSS's four-gate sequence maps directly to PrOF's three milestone-bearing programme cycle stages.

| PrOF Stage | PrOF Requirement | CROSS Gate Equivalent |
| :-- | :-- | :-- |
| Design (pre-implementation) | Programme Design Document: logframe/results chain, indicators with baselines and targets, evidence plan, risk register | Entry specification gate: obligation mode declaration, eleven-field indicator specification, Theory of Change architecture, data cost estimation |
| Annual review | Progress assessment against results framework; formal annual review output | Progress gate(s): gate evidence submission, indicator actuals, continuation specification |
| Programme completion | Programme Completion Report: results summary, learning, evidence of achievement | Completion gate: completion verification record, gate evidence, FROM/TO state comparison |

The entry specification gate is the design-approval equivalent in CROSS. It is the gate at which the obligation architecture is locked: indicators are fully specified through all eleven fields, the ToC is declared with named causal links and assumptions, and the evidence plan is encoded in the obligation record. This is structurally identical to what PrOF requires a Programme Design Document to contain before implementation begins.

Progress gates produce the structured evidence record that annual reviews require. The gate evidence submission, indicator actuals, and continuation specification together constitute the data layer of an annual review; PrOF's annual review output is a narrative layer that draws on this underlying evidence.

The completion gate produces the evidence base for the Programme Completion Report. The FROM/TO state comparison documents whether targets were achieved; the gate evidence record documents what evidence supports the assessment; the causality stance and ToC assumptions document what can and cannot be attributed to the programme.

---

## WALKRI and the PrOF Evidence Plan Requirement

PrOF requires that every Programme Design Document include an evidence plan. The evidence plan specifies how the programme will collect, manage, and use evidence to inform decisions. It is not a data management plan in the technical sense; it is a forward-looking specification of how measurement will work in practice.

WALKRI's five pre-publication field requirements are the specification-layer expression of an evidence plan at the instrument level. The criterion intent requirement specifies what each field measures. The operational definition requirement specifies what counts and what does not. The response form justification requires that the collection method be explained and matched to the measurement goal. The evidence form requirement specifies what artifact independently verifies each claimed measurement. The compliance threshold requirement specifies when a response is sufficient.

A programme whose collection instruments satisfy WALKRI's five requirements has, at the field level, addressed the core questions an evidence plan must answer: what is being measured, how, with what instrument, through what verification pathway, and under what sufficiency criteria. This does not replace the narrative evidence plan that PrOF requires; it satisfies the specification content that the evidence plan must document.

WALKRI's three data quality standards of particular relevance to PrOF evidence plans are validity (the field measures what it claims to measure), integrity (evidence is independent of the beneficiary's self-report), and reliability (the measurement produces consistent results across reporting periods and data collectors). These three standards address the most common evidence quality failures that FCDO annual reviews have identified in programme reporting.

---

## Mapping Table

| PrOF PDD Requirement | CROSS/WALKRI Provision | Gap or Note |
| :-- | :-- | :-- |
| Logframe or results chain | Theory of Change architecture (goal, outcome, output, activity with causal links) | CROSS ToC is a superset of a standard logframe; it includes named assumptions and a causality stance field. |
| Outcome indicators with baselines | Eleven-field indicator specification (Fields 1-11), FROM state (baseline) | CROSS requires all eleven fields; PrOF requires at minimum a name, unit, baseline, and target. CROSS exceeds this. |
| Targets | TO state specification (change-obligation) or completion criteria (build-obligation) | Direct correspondence. |
| Evidence plan | WALKRI five field requirements; gate evidence submission requirements | WALKRI covers the instrument-level evidence plan. Narrative evidence plan is separately produced by programme management. |
| Risk register | No CROSS equivalent | CROSS's assumption documentation in the ToC covers assumption risk, but a PrOF risk register is a separate operational document outside specification scope. |
| IATI publication | CROSS IATI alignment (see IATI Compatibility Statement) | Full correspondence via IATI pathway. |
| OECD DAC evaluation | Field 10 DAC alignment declaration; ToC causal architecture; causality stance | CROSS produces the specification architecture for DAC assessment; evaluator judgment applies the criteria. |
| Annual review | Progress gates with indicator actuals and gate evidence | Direct structural correspondence. |
| Programme Completion Report | Completion gate record with FROM/TO comparison and gate evidence | Direct structural correspondence. |

---

## Adoption Guidance

Programs seeking FCDO co-financing or operating under FCDO contracts that adopt CROSS+WALKRI should:

1. Declare OECD DAC alignment in Field 10 for each indicator cluster relevant to the programme's evaluation criteria. This produces documented DAC alignment within the obligation record rather than requiring post-hoc reconstruction at review.

2. Configure the entry specification gate to produce the PDD-equivalent documentation before implementation begins. The eleven-field indicator specification, ToC architecture, and WALKRI-conformant collection instruments together constitute the specification content of the PDD evidence and results chain sections.

3. Apply WALKRI's five field requirements to all collection instruments before the entry gate. This satisfies the evidence plan requirement at the instrument level and ensures that annual review indicator actuals are produced by specified, auditable instruments.

4. Implement IATI export from the CROSS gate record structure. Programs receiving FCDO co-financing must publish to IATI; CROSS conformance produces the data required for IATI publication without additional data collection.

5. Use the completion gate record as the evidence base for the Programme Completion Report. The FROM/TO state comparison, gate evidence submissions, and causality stance documentation constitute the structured evidence layer of the PCR narrative.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

FCDO Programme Operating Framework: https://www.gov.uk/government/publications/fcdo-programme-operating-framework

IATI Standard v2.03: iatistandard.org

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. Two compatibility pathways (OECD DAC and IATI) documented. Gate architecture mapped to PrOF programme cycle milestones. WALKRI evidence plan alignment documented. Full PDD mapping table. Adoption guidance. |
