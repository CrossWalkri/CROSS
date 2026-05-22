---
title: ARPA-H Payable Milestones and Other Transactions Framework Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.4 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - ARPA-H Other Transactions Authority guidance (arpa-h.gov)
  - ARPA-H Industry Day materials and milestone documentation (arpa-h.gov)
  - DARPA Other Transactions authority (darpa.mil)
  - BARDA Other Transactions for medical countermeasures (medicalcountermeasures.gov)
---

# ARPA-H Payable Milestones and Other Transactions Framework

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Advanced Research Projects Agency for Health (ARPA-H), launched in 2022, funds high-risk biomedical research using Other Transactions (OT) authority. OT authority means that 2 CFR 200 does not apply: the standard federal grant management and cost accounting rules that govern the rest of this compatibility series are largely inapplicable to ARPA-H awards. Instead, the payable milestone structure is the entire evaluation architecture. ARPA-H uses two types of payable milestones: fixed milestones, where payment is triggered by completion of a discrete technical event with pre-specified completion criteria, and expenditure-based milestones, where payment follows spending against a budget checkpoint. CROSS+WALKRI satisfies the ARPA-H milestone framework structurally, and does so more directly than for any standard grant program. The fixed milestone structure with pre-specified completion criteria is the most fully realized implementation of CROSS's Build obligation mode anywhere in the federal landscape. This compatibility mapping applies equally to other federal agencies operating under OT authority, including DARPA and BARDA.

---

## The ARPA-H Other Transactions Milestone Framework

ARPA-H's use of OT authority produces a fundamentally different accountability architecture than any standard federal grant program. Where a standard grant program specifies programmatic requirements and leaves payment largely tied to expenditure compliance, ARPA-H's milestone structure ties payment directly to delivery: no milestone completion, no payment. Non-achievement of a milestone triggers not a remediation process but award termination. This binary accountability structure makes the quality of milestone specification a first-order question: if the completion criteria are underspecified, the determination of whether a milestone has been achieved becomes a judgment call rather than a reviewable technical finding.

Fixed milestones specify an observable technical event (a prototype demonstration, a clinical data readout, a manufacturing process validation) along with completion criteria that articulate the basis for payment: what reports must be submitted, what demonstration must be conducted, what tests must pass, and at what performance levels. ARPA-H Program Managers conduct biweekly to monthly check-ins with performers, and all milestone structures and completion criteria are publicly documented in ARPA-H Industry Day materials. Expenditure-based milestones are simpler in structure: payment follows the spending of a defined budget tranche, without a technical performance requirement attached to that specific payment event.

The milestone-payment architecture makes ARPA-H the federal analog to on-chain milestone-based grant programs in the Web3 ecosystem, with the distinction that ARPA-H's completion criteria are specified in natural language reviewed by Program Managers rather than encoded in smart contract logic. The structural accountability principle is identical: pre-specified observable technical deliverable, pre-specified completion criteria, payment contingent on verified delivery.

---

## How CROSS Satisfies the ARPA-H Milestone Framework

CROSS satisfies the ARPA-H milestone requirements more directly than for any other framework covered in this compatibility series, because the fixed milestone structure is a direct implementation of CROSS's Build obligation mode.

**Build obligation mode and fixed milestone structure:** CROSS's Build obligation mode governs programs where the primary obligation is delivery of a specified output. The program commits to producing a discrete, observable technical artifact, and the completion gate determines whether the artifact has been delivered according to the pre-specified criteria. ARPA-H's fixed milestone structure is precisely this: the technical event is the output, the completion criteria are the gate specification, and payment is contingent on clearing the gate. A CROSS-conformant ARPA-H program specifies each milestone as a Build obligation mode entry in the program's indicator set, with the observable technical event as Field 1 (name) and the completion criteria as Fields 7-11 (timing, data source, collection method, causality stance, evidence threshold).

**Entry specification gate and completion criteria pre-specification:** ARPA-H's requirement that completion criteria be specified before work begins is the regulatory form of CROSS's entry specification gate. The completion criteria for each milestone (what reports, demonstrations, and tests are required) must be established and agreed upon in the award agreement before the performer begins work. This is the OT analog to CROSS's requirement that all indicators be pre-specified before applications open: the performer cannot begin work under conditions of indicator ambiguity. WALKRI's compliance threshold requirement addresses exactly the question that ARPA-H's completion criteria must answer: what does a passing demonstration look like, as distinct from a demonstration that fails to satisfy the milestone?

**Continuation gate and staged funding with termination trigger:** ARPA-H's staged funding structure, where non-achievement of a milestone triggers termination rather than a remediation opportunity, corresponds to CROSS's continuation gate: progress at each stage is assessed against pre-specified criteria before the next disbursement. The termination trigger makes CROSS's continuation gate a hard gate rather than a soft accountability checkpoint: the program cannot continue in the next stage without clearing the criteria of the current stage. This is the strongest implementation of a continuation gate in the federal landscape.

**WALKRI evidence form and completion criteria specification:** The completion criteria for a fixed milestone must specify what form the evidence takes: is it a written report, a live demonstration, a test result from a specified protocol, or a combination? This is WALKRI's evidence form requirement applied to milestone specification. Before any performer begins work, the completion criteria must specify what the evidence looks like at the time of submission, not merely what technical goal must be achieved.

| ARPA-H Milestone Element | CROSS Provision |
|:--|:--|
| Fixed milestone structure (observable technical event + pre-specified completion criteria) | Build obligation mode (program commits to delivering specified output; completion gate criteria defined at entry gate) |
| Completion criteria specify reports, demonstrations, and tests required for payment | Entry specification gate (all indicator criteria pre-specified before work begins) |
| Staged funding contingent on milestone achievement | Continuation gate (progress assessed against pre-specified criteria before next disbursement) |
| Non-achievement triggers award termination | Hard continuation gate (program cannot proceed without clearing current stage criteria) |
| ARPA-H Program Manager review at biweekly to monthly intervals | Interim evidence review within completion gate structure |
| Expenditure-based milestones (payment after budget checkpoint spending) | Build obligation mode at expenditure level, with disbursement gate tied to spending rather than technical performance |
| Public documentation of milestones in Industry Day materials | Entry gate publication requirement (indicator specification published before any performer engages) |
| OT authority removes 2 CFR 200 baseline | CROSS's framework-neutral obligation architecture (compatible with OT authority and standard grant authority alike) |

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication requirements address the completion criteria specification problem that is the central accountability risk in ARPA-H's milestone structure. The milestone framework requires that completion criteria be specified before work begins, but the OT authority guidance does not prescribe how precisely those criteria must be specified. Underspecified completion criteria create a dispute risk: the performer delivers what they understood the milestone to require, and the Program Manager determines that it falls short of what the milestone was intended to require, but neither party can point to a pre-agreed specification that resolves the dispute.

WALKRI's five requirements applied to milestone completion criteria specification resolve this at the pre-award stage. The criterion intent field establishes what the milestone is designed to demonstrate in the context of the program's research hypothesis. The operational definition field specifies what the technical event consists of: not merely "a prototype demonstration" but the specific capabilities the prototype must exhibit, the conditions under which the demonstration will occur, and the performance parameters that must be met. The response form field specifies the format of the submission: what the report must contain, how the demonstration must be documented, which test protocols must be applied. The evidence form field specifies the documentation that constitutes the milestone deliverable package. The compliance threshold field specifies the performance levels that distinguish a passing result from a failing one, producing completion criteria that are reviewable by any technically qualified third party without interpretive ambiguity.

This mapping applies to all OT-based milestone programs, not only ARPA-H. DARPA (the originating OT authority agency) and BARDA (for medical countermeasure development) operate under structurally identical milestone frameworks. CROSS+WALKRI conformance for ARPA-H programs is therefore a template applicable across the federal OT ecosystem.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
