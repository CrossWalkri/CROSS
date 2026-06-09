---
title: SBIR/STTR Cross-Agency Commercialization Benchmarks Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.5 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - Small Business Innovation Research Program Reauthorization Act (15 U.S.C. § 638)
  - SBA SBIR/STTR Policy Directive (sbir.gov/policy-directive)
  - SBIR/STTR awards and commercialization database (sbir.gov)
lens_tags:
  calibration_tier: outcome_specified_self_reported
  authority_source: statutory
  cultural_methodological_lineage: western_institutional
  funder_typology: government_non_aid
  framework_scope_type: grantee_outcome_measurement
  # Small Business Innovation Research / Small Business Technology Transfer commercialization benchmarks under Small Business Act
---

# SBIR/STTR Cross-Agency Commercialization Benchmarks

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Small Business Innovation Research (SBIR) and Small Business Technology Transfer (STTR) programs are mandated by statute (15 U.S.C. § 638) and administered across eleven federal agencies. Two cross-agency performance benchmarks are legally binding and published in the Federal Register: a Phase I-to-Phase II transition rate minimum of 0.25, and an average commercialization revenue benchmark of at least $100,000 per Phase II award. These benchmarks are not agency-discretionary; they are statutory minimums reported to Congress annually. Neither benchmark applies to individual grantees: both apply to the agency's entire SBIR/STTR portfolio. This portfolio-level obligation-measurement structure, in which the funder's grant portfolio as a whole must meet a published performance threshold, is a new primitive in CROSS+WALKRI's coverage. CROSS can express both benchmarks through its portfolio aggregation mechanism, and WALKRI applies to the Phase I and Phase II reporting instruments where the quality of commercialization evidence is determined before any award cycle opens.

---

## The SBIR/STTR Statutory Benchmark Framework

The SBIR and STTR programs operate under the Small Business Innovation Research Program Reauthorization Act (15 U.S.C. § 638), with implementing guidance in the SBA SBIR/STTR Policy Directive. The programs are administered across eleven federal agencies, each of which runs its own SBIR/STTR competitions within the statutory framework. The SBIR/STTR database (sbir.gov) is the public registry of all awards and reported commercialization outcomes.

Two cross-agency benchmarks are statutory rather than agency-discretionary. The Phase I-to-Phase II transition rate minimum requires that at least 25% of a participating agency's Phase I awardees advance to Phase II. Agencies falling below this floor face compliance review. The commercialization benchmark requires an average of at least $100,000 in commercialization revenue per Phase II award, drawn from sales, licenses, and further investment in commercialized technologies. Both benchmarks are reported to Congress annually through SBA.

These benchmarks have a structural property that distinguishes them from every other federal grant framework in CROSS+WALKRI's coverage: they do not apply to individual grantees. Individual SBIR/STTR awardees have no statutory obligation to transition from Phase I to Phase II, and no individual Phase II awardee must achieve $100,000 in commercialization revenue. The benchmarks are portfolio-level obligation-measurement instruments applied to the agency's total SBIR/STTR program. An agency's portfolio of Phase I awards must achieve at least 25% forward progression; the agency's portfolio of Phase II awards must achieve at least $100,000 in commercialization revenue per award on average. The unit of reporting obligation is the funding agency's portfolio, not the individual grantee.

No other federal grant program currently has statutory minimum outcome benchmarks at the portfolio level that agencies must meet or face compliance consequences. This is the structural innovation that requires dedicated coverage in CROSS+WALKRI.

---

## How CROSS Satisfies the SBIR/STTR Framework

CROSS addresses the SBIR/STTR framework at two levels: the individual grantee level, where the four-gate sequence applies in its standard form, and the portfolio level, where the statutory benchmarks introduce a new primitive that CROSS's current architecture does not yet fully formalize.

**Individual grantee gate sequence:** At the individual award level, Phase I awards correspond to CROSS's entry specification gate: the award is conditioned on a specified scope of research and a go/no-go decision point at Phase I completion. Phase II awards correspond to the application gate, in which the grantee has passed the Phase I gate and entered full program execution. Phase II completion and commercialization reporting correspond to CROSS's completion gate. Any follow-on reporting or validation of commercialization outcomes corresponds to the attestation gate.

**Phase I-to-Phase II transition rate and CROSS's portfolio aggregation:** The Phase I-to-Phase II transition rate benchmark is CROSS's continuation gate applied at the portfolio level. CROSS's continuation gate (within the four-gate sequence) assesses whether an individual program should proceed from one phase to the next. The SBIR/STTR framework applies the equivalent logic to the agency's entire portfolio: the rate at which the agency's Phase I cohort advances to Phase II is itself a portfolio-level verification metric for the agency, not only for individual grantees. CROSS's portfolio aggregation mechanism can express this: the proportion of programs in a funded cohort that pass the continuation gate is a portfolio-level output of the gate sequence. Making this aggregation a statutory minimum with compliance consequences is the structural innovation that CROSS does not yet formalize as a named component. This statement proposes the name portfolio-level continuation benchmark for the archetype.

**Commercialization revenue benchmark and CROSS's completion gate aggregated:** The $100,000 per Phase II award commercialization benchmark is a portfolio-level outcome indicator. At the individual grantee level, it corresponds to the completion gate: the evidence review confirming that the Phase II award produced the commercialization outcomes it was funded to produce. At the portfolio level, it is the aggregate of individual completion gate outcomes expressed as an average: the sum of reported commercialization revenue across all Phase II awards in the agency's portfolio, divided by the number of awards, must meet or exceed $100,000. CROSS's portfolio aggregation mechanism can model this directly, with the portfolio-level benchmark serving as the funder-facing verification metric above the individual grantee's completion gate.

**Build obligation mode:** SBIR/STTR Phase I and Phase II awards operate in CROSS's Build obligation mode: the funded work is a new technology development, and the gate sequence is prospective, specifying what will be built and evaluated.

| SBIR/STTR Framework Element | CROSS Provision |
|:--|:--|
| Phase I award and go/no-go decision point | Entry specification gate (scope declared; Phase I completion is the gate determination) |
| Phase II award (full execution phase) | Application gate (continuation after passing Phase I gate) |
| Phase II completion and commercialization reporting | Completion gate (evidence review against pre-specified commercialization criteria) |
| Phase I-to-Phase II transition rate minimum (0.25) | New primitive: portfolio-level continuation benchmark (not yet formalized in CROSS architecture) |
| Commercialization revenue benchmark ($100K per Phase II) | Portfolio aggregation of completion gate outcomes; funder-level verification metric |
| Annual SBA reporting to Congress | Attestation gate at portfolio level (public record of agency SBIR/STTR portfolio performance) |
| sbir.gov public awards database | Attestation gate (public registry of individual award conformance records) |

---

## How WALKRI Complements This Alignment

WALKRI's pre-publication requirements apply to the Phase I and Phase II reporting instruments, where the quality of commercialization evidence is determined. The statutory benchmarks create strong pressure on commercialization data quality: an agency's compliance status depends on the aggregate of its grantees' reported commercialization figures, making the consistency and verifiability of individual reports a portfolio-level concern.

For each commercialization reporting field in a Phase II reporting instrument, WALKRI requires: criterion intent (what type of commercial activity the field is designed to capture), operational definition (exactly what counts as commercialization revenue, covering sales versus license fees versus third-party investment committed to the technology), response form (how the revenue figure is calculated and reported, including currency, period, and attribution scope), evidence form (what documentation is required to substantiate the reported figure, distinguishing binding contracts from letters of intent from informal commitments), and conformance threshold (the minimum documentation standard a reported figure must meet to be included in the agency's portfolio aggregate). Without this specification level, the $100,000 benchmark is mathematically precise but operationally ambiguous: a binding product sale and an unsigned letter of intent may receive equivalent treatment in the aggregate if the reporting instrument does not distinguish them.

The Phase I-to-Phase II transition rate creates an analogous WALKRI obligation for the Phase I completion instrument: the criteria by which a Phase I report is reviewed and a go/no-go decision is made must be specified before any Phase I award is made. WALKRI applied to Phase I completion review instruments means that before the award cycle opens, agencies specify what evidence form satisfies the go/no-go gate, what constitutes a valid feasibility demonstration, and what documentation threshold is required for the transition decision. This makes the transition rate benchmark meaningful as a compliance measure rather than an artifact of variable review standards across program officers.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
