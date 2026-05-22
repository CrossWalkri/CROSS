---
title: JICA and Japan's ODA Evaluation System Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.2 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - https://www.jica.go.jp/english/our_work/evaluation/tech_and_grant/guides/guideline.html
  - https://www.mofa.go.jp/policy/oda/evaluation/basic_documents/pdfs/guidelines11th.pdf
  - https://www.mofa.go.jp/policy/oda/evaluation/basic_documents/pdfs/handbook2024.pdf
---

# JICA and Japan's ODA Evaluation System

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

Japan's official development assistance evaluation system, administered through JICA and governed by Japan's Ministry of Foreign Affairs ODA Evaluation Guidelines (11th edition), operates through six OECD DAC criteria applied across a continuous PDCA (Plan-Do-Check-Act) cycle. JICA's distinctive requirements, including mandatory ex-ante evaluation, lifecycle-stage PDCA documentation, a uniform project rating system, and mandatory ex-post evaluation three to five years after project completion, map directly onto CROSS gate architecture. WALKRI's instrument-level field specification requirements satisfy the accuracy standards on which JICA's rating system depends.

---

## The JICA/ODA Framework's Approach

JICA is one of the world's five largest bilateral donors, operating a grant and technical assistance portfolio spanning more than 150 countries. Its evaluation system is formally governed by two instruments: the JICA "Guideline for Project Evaluation" and Japan's Ministry of Foreign Affairs "ODA Evaluation Guidelines" (now in its 11th edition). Both instruments apply the six OECD DAC criteria (relevance, coherence, effectiveness, efficiency, impact, sustainability) across all evaluations, establishing a common baseline with the rest of the international development evaluation community.

What distinguishes JICA's system from a standard DAC application is its mandatory PDCA cycle structure. JICA requires that evaluation not be treated as a terminal event conducted after project close; instead, Plan-Do-Check-Act cycles must be documented at every lifecycle stage. This transforms evaluation from an accountability instrument applied retrospectively into a continuous improvement loop woven through project design, implementation, monitoring, and closure. The PDCA mandate is not optional or aspirational: projects that cannot demonstrate cycle documentation at each stage fail to meet JICA's procedural requirements.

A second distinctive requirement is mandatory ex-ante evaluation. Before any JICA-supported project receives approval, a standard-format ex-ante evaluation must be completed and documented. This requirement is structural: it gates project authorization. Ex-ante evaluation documents what the project intends to achieve, what evidence supports the design, what indicators will measure progress, and what rating will constitute success. The completion of this documentation before the project commences creates an independent pre-commitment record that survives the project's implementation phase intact.

The third distinctive element is JICA's uniform project rating system. All evaluations across the JICA portfolio apply a common rating scale. This means that quality of evaluation evidence, including the precision of baseline measurements and the completeness of indicator documentation, directly affects how projects are rated and, by extension, how funding decisions are made for follow-on activities. The rating system creates a structural incentive for measurement quality that goes beyond general DAC criterion compliance.

Finally, JICA's mandatory ex-post evaluation requirement, applied three to five years after project completion, means that project records must remain retrievable and verifiable long after a project closes. This creates a longitudinal record-keeping obligation that typical grant management systems are not designed to satisfy.

---

## How CROSS Satisfies the JICA/ODA Framework

CROSS gate architecture satisfies JICA's PDCA mandate at a structural level. The four CROSS operational gates correspond directly to the four phases of JICA's required cycle.

**Plan phase (CROSS Entry Specification Gate).** The entry gate requires that indicator specifications, gate criteria, and Theory of Change be complete and recorded before any applications open. This is an ex-ante documentation requirement by definition: the program's measurement design is committed to record before any implementation activity (the Do phase) begins. JICA's mandatory ex-ante evaluation format asks for the same categories of information: intended outcomes, indicator definitions, evidence basis for program design, and criteria by which success will be assessed.

**Do phase (CROSS Progress Verification Gate).** The progress gate establishes what implementation-phase evidence is required during active project execution. Its documentation becomes the "Do" record in the PDCA loop.

**Check phase (CROSS Completion Gate).** The completion gate requires evidence review: what actually occurred relative to the specifications committed at entry. This is the formal Check function, conducted against pre-committed criteria rather than post-hoc standards.

**Act phase (CROSS Continuation Gate).** The continuation gate requires that programs document what was learned and specify how obligations will change in the next cycle before future rounds open. This is the Act function: findings must demonstrably inform subsequent planning.

| JICA/ODA Requirement | CROSS Structural Element |
|---|---|
| Mandatory ex-ante evaluation | Entry gate pre-commitment record |
| PDCA Plan phase documentation | Entry specification gate |
| PDCA Do phase documentation | Progress verification gate |
| PDCA Check phase documentation | Completion gate evidence review |
| PDCA Act phase documentation | Continuation gate obligation specification |
| Mandatory ex-post evaluation (3-5 yr) | Attestation Corpus retains verifiable gate records for future review |
| Uniform project rating system | Completion gate evidence against pre-committed indicator specs |

The CROSS pre-commitment record is particularly significant for JICA's ex-ante requirement because it is generated before applications open, not assembled retrospectively. This means the Plan phase documentation precedes the Do phase by design, satisfying JICA's gating requirement at the system level rather than relying on individual program administrators to maintain procedural discipline.

For ex-post evaluation, the CROSS Attestation Corpus provides the longitudinal record. Gate documentation retained in the Corpus is verifiable against original specifications years after a program closes, satisfying the evidentiary requirements that JICA's three-to-five-year post-completion evaluation window demands.

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication field requirements address the accuracy standards on which JICA's uniform rating system depends. A rating applied consistently across a portfolio is only as meaningful as the measurement instruments underlying the evidence being rated. WALKRI requires that each measurement field be specified with instrument type, unit of measure, collection method, verification pathway, and access information before applications open. This level of instrument-level specification provides the methodological precision that JICA's rating system presupposes but that most grant application formats do not structurally enforce.

For programs seeking to satisfy both JICA's evaluation requirements and CROSS+WALKRI standards simultaneously, the practical implication is that WALKRI-compliant intake fields double as the measurement instrument documentation that a JICA ex-ante evaluation must contain. Programs operating in JICA-funded contexts therefore gain dual compliance from a single documentation effort: WALKRI fields satisfy JICA's ex-ante instrument documentation requirements, while CROSS gates satisfy JICA's PDCA lifecycle documentation requirements.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
