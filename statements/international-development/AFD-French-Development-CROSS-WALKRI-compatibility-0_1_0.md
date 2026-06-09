---
title: AFD French Development Cooperation Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.2 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - https://www.afd.fr/en/ressources/afd-group-monitoring-and-evaluation-policy
  - https://www.oecd.org/derec/france/AFD-evaluation-policy-eng.pdf
lens_tags:
  calibration_tier: independently_verified
  authority_source: statutory
  cultural_methodological_lineage: western_institutional
  funder_typology: bilateral_aid_agency
  framework_scope_type: grantee_outcome_measurement
  # Agence Francaise de Developpement French bilateral aid agency; statutory establishment under French law
---

# AFD French Development Cooperation

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

France's Agence Française de Développement (AFD) published a revised Group Monitoring and Evaluation Policy in 2024, notable as the first policy applying across the entire AFD Group including Proparco, its private sector arm. Beyond standard OECD DAC criteria (addressed in CROSS Part XII coverage), AFD's policy adds three structural requirements: M+E systems must be built into project design documents before implementation begins, an AFD Group-wide Impact Portal is to publish impact data across the full portfolio, and a group-wide learning loop requires evaluation findings to feed back into programming decisions in a documented, trackable way. CROSS gate architecture satisfies all three additions directly; WALKRI satisfies AFD's design-stage M+E integration requirement at the data collection instrument level.

---

## The AFD Framework's Approach

AFD is France's primary development finance institution, operating across grants, concessional loans, guarantees, and equity investments in more than 100 countries. The 2024 AFD Group Monitoring and Evaluation Policy is significant for two reasons beyond its content: it is the first M+E policy to formally encompass Proparco (AFD's private sector subsidiary) within a unified framework, and it represents an explicit step toward portfolio-level impact transparency rather than project-level reporting only.

The foundation of AFD's M+E system is the OECD DAC criteria, applied through AFD's CRI (Results and Impact Framework), which organizes 22 indicators across AFD Group entities. Because CROSS Part XII addresses OECD DAC compatibility directly, that baseline is not the focus of this statement. What requires separate treatment are the three structural additions that distinguish the 2024 AFD policy from a standard DAC application.

The first addition is the design-stage M+E integration requirement. AFD's policy requires that M+E systems be built into project design documents before implementation begins. This is architecturally different from requiring that programs conduct evaluations during or after implementation. It means the measurement infrastructure, including the indicators, data collection methods, and reporting obligations, must be specified as part of the project design rather than developed after a project is approved and funded. The practical implication is that programs cannot submit an application with vague outcome statements and promise to develop measurement systems later; the measurement system is a constitutive element of the project design itself.

The second addition is the AFD Group-wide Impact Portal. AFD describes this as an operational system by end 2025, designed to publish impact data across the full AFD Group portfolio. A portfolio-level transparency commitment of this kind creates a documentation consistency requirement that flows back to individual projects: if impact data is to be aggregated and published coherently at the group level, individual project impact documentation must be expressed in compatible formats. Projects whose impact evidence is idiosyncratically structured cannot contribute to a coherent portfolio-level publication.

The third addition is the group-wide learning loop mechanism. AFD's 2024 policy requires that evaluation findings feed back into programming decisions in a way that is documented and trackable. This goes beyond the common aspiration that evaluations should inform future programming; it requires a traceable record of how specific findings influenced specific decisions. The learning loop is not satisfied by a narrative summary of lessons learned; it requires a documented pathway from evidence to programming change.

---

## How CROSS Satisfies the AFD Framework

Because CROSS Part XII covers OECD DAC compatibility, this statement focuses on the three structural additions in AFD's 2024 policy: design-stage M+E integration, Impact Portal transparency, and the learning loop mechanism.

**Design-stage M+E integration and the CROSS entry gate.** The CROSS entry specification gate requires that indicator specifications, gate criteria, and Theory of Change be fully documented before any applications open. This is structurally identical to AFD's design-stage M+E integration requirement: the measurement system is not developed after projects are selected but is constitutive of the program design to which applicants respond. A CROSS-conformant program has its M+E architecture in place before any funding decision is made. AFD's policy requirement is satisfied at the system level: programs built on CROSS architecture cannot, by design, defer M+E system development until after project approval.

**Impact Portal transparency and the CROSS Attestation Corpus.** AFD's Impact Portal commitment requires that impact data be published across the full AFD Group portfolio in a coherent, aggregable form. The CROSS Attestation Corpus serves the same architectural function: it is a publication-ready record of gate documentation across all CROSS-conformant programs and rounds, structured consistently by the CROSS gate schema. Programs that satisfy CROSS gate documentation requirements automatically produce impact evidence in the consistent format that portfolio-level publication demands. The Attestation Corpus is CROSS's structural equivalent of AFD's Impact Portal from the program-side documentation perspective.

**Learning loop mechanism and the CROSS continuation gate.** The CROSS continuation gate is the direct structural equivalent of AFD's learning loop requirement. The continuation gate requires that programs document what was learned in a completed cycle and specify how that learning changes the next round's obligations before a new round opens. This creates exactly the documented, trackable pathway from evaluation findings to programming decisions that AFD requires. The continuation gate record is not a narrative summary; it is a structured gate document that must specify which findings informed which obligation changes, creating the traceable learning-to-decision record AFD's policy demands.

| AFD 2024 Policy Addition | CROSS Structural Element |
|---|---|
| Design-stage M+E integration | Entry gate (indicator specs and gate criteria complete before applications open) |
| Group-wide Impact Portal publication | Attestation Corpus publication requirement |
| Learning loop (findings feed back into programming, documented and trackable) | Continuation gate (learning documented before next round opens) |
| OECD DAC criteria (baseline) | CROSS Part XII coverage (addressed separately) |

The relationship between AFD's three additions and CROSS gate architecture is direct and functional at each point. This is not a case where CROSS satisfies a framework's requirements through adjacent documentation; each AFD addition corresponds to a gate function designed to address the same underlying problem: that measurement systems designed too late produce evidence that cannot inform the decisions that matter, and that learning loops without a named response to non-conformance remain aspirational rather than operational.

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication field requirements satisfy AFD's design-stage M+E integration requirement at the data collection instrument level, one level more granular than CROSS's gate architecture operates. CROSS ensures that an M+E system is built into program design before implementation; WALKRI ensures that the individual measurement instruments comprising that M+E system are specified at the level of precision required to produce reliable, comparable evidence.

For AFD's Impact Portal to publish coherent portfolio-level impact data, individual program M+E systems must not only exist at design stage but must be methodologically compatible across programs. WALKRI's uniform field specification requirements (instrument type, unit, collection method, verification pathway, access path) create the methodological consistency across programs that enables AFD's portfolio-level aggregation. Without this instrument-level consistency, projects might each have design-stage M+E systems that satisfy AFD's procedural requirement while producing incompatible evidence that cannot be coherently published at the portfolio level.

Programs operating within AFD-funded contexts that adopt CROSS+WALKRI standards therefore satisfy AFD's design-stage integration requirement at both the program design level (CROSS) and the measurement instrument level (WALKRI), while simultaneously producing evidence in the consistent format that AFD's Impact Portal and portfolio-level learning loop require.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
