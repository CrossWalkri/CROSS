---
title: Impact Management Norms Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.3.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - Impact Management Norms (impactmanagementnorms.com)
  - Impact Management Project - Five Dimensions of Impact
  - GIIN IRIS+ v5.3c (iris.thegiin.org)
  - Impact Frontiers - Contribution Thesis
lens_tags:
  calibration_tier: outcome_specified_self_reported
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: pooled_fund_or_intermediary
  framework_scope_type: grantee_outcome_measurement
  # Impact Management Project / Norms is a coalition-built voluntary framework; pooled_fund_or_intermediary as primary; alternative: civil_society_advisory authority
---

# Impact Management Norms Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS+WALKRI-conformant program addresses all five dimensions of the Impact Management Norms (IMN) as a structural consequence of conformance. Programs that implement CROSS for obligation architecture and WALKRI for field specification quality produce IMN-compatible impact evidence without additional documentation work.

The Impact Management Norms are a shared conceptual framework developed collaboratively by GIIN, SASB, GRI, PRI, and other impact measurement organizations to establish common language for what it means to manage impact rigorously. They organize impact evidence around five dimensions: What, Who, How Much, Contribution, and Risk. CROSS+WALKRI addresses each dimension through specific provisions that are more operationally precise than the IMN framework requires.

---

## What the Impact Management Norms Are

The Impact Management Norms (formerly the Impact Management Project, or IMP) emerged from a multi-year collaborative process among impact measurement organizations to establish shared definitions for what counts as managing impact. They are not a reporting standard or a certification; they are a conceptual framework that defines what an organization must be doing to genuinely manage its impact rather than merely reporting on it.

The IMN framework organizes impact evidence and management around five dimensions:

**What**: What outcomes occur for people or the planet, and how important are they? This dimension asks funders and implementers to specify: what specific outcomes are being targeted, in what domain, and whether those outcomes matter to the people or systems experiencing them.

**Who**: Who experiences the outcomes? This dimension asks for specificity about the affected population: who they are, how underserved they are relative to available alternatives, and whether they are the intended beneficiaries or affected parties.

**How Much**: How much of the outcome occurs? This dimension addresses scale (how many people), depth (how significant the change is for each person), and duration (how long the change lasts).

**Contribution**: Would this change have happened anyway? This dimension asks whether the investor's or funder's contribution made a material difference to whether the outcome occurred, relative to what would have happened without their involvement.

**Risk**: What is the risk that impact is different from expected? This dimension asks about the probability and severity of impact not occurring as planned, including unintended negative consequences.

---

## CROSS Mapping to the Five Dimensions

### What

The IMN "What" dimension requires specifying: which outcomes are targeted, in which impact category, and whether those outcomes are important to the affected population.

CROSS addresses the "What" dimension through:

- **Obligation mode**: specifies whether the program targets output-level outcomes (build-obligation) or condition-level outcomes (change-obligation), making the level of the "What" claim explicit.
- **Indicator name and rationale** (Fields 1 and 2): specifies which outcome is being measured and why that indicator was chosen as the appropriate representation of the targeted outcome.
- **Criterion intent** (WALKRI Section 3.1): specifies what the collection field actually measures, ensuring the "What" is defined at the instrument level rather than only at the reporting level.
- **Domain tags from sufficiency architecture declaration**: places the "What" within a thematic context using controlled vocabulary from the declared measurement framework (IRIS+, OECD DAC sector codes, or custom).
- **ToC hierarchy level** (Part IX-B): specifies whether the targeted outcome is a short-term, intermediate, or long-term outcome, addressing the IMN's distinction between outcomes that matter directly to beneficiaries and outcomes that matter at the systemic level.

### Who

The IMN "Who" dimension requires specifying: who the affected population is, how underserved they are, and whether they are the direct beneficiaries or others affected by the intervention.

CROSS addresses the "Who" dimension through:

- **FROM state population specification** (Part IV, change-obligation entry): the FROM state must name a specific measurable condition in a defined population. The population is a required element of the FROM state, not an optional qualifier.
- **Disaggregation specification** (Field 7): specifies which population breakdowns are tracked and applies a disaggregation ratchet so that reporting cannot become less specific over time.
- **WALKRI operational definition** (Section 3.2): for fields collecting data about affected-population members, the operational definition specifies who counts as within the population and who does not.
- **Unintended outcomes disclosure** (Part IV): requires identification of populations affected by the intervention that were not specified in the entry gate, addressing the IMN's concern about affected parties beyond the intended beneficiaries.

### How Much

The IMN "How Much" dimension requires addressing scale (how many), depth (how significant the change is per person), and duration (how long the change persists).

CROSS addresses the "How Much" dimension through:

- **Scale**: disaggregation (Field 7) specifies the population count; the TO state (Field 11) specifies the aggregate target value.
- **Depth**: the operational definition (WALKRI Section 3.2) specifies the unit and counting rule that determines what counts as a meaningful change for each person. A field that counts any engagement is measuring a different depth than a field that counts engagement meeting a specified threshold of substantive change.
- **Duration**: the sustainability stance declaration (Part IV, continuation gate) requires the grantee to declare whether the "How Much" achieved is sustained, conditional, or dependent on continued intervention. This is the operational form of the IMN's duration requirement.
- **Cumulative vs. non-cumulative designation** (Field 6): specifies whether the reported "How Much" accumulates across reporting periods or represents the current state, which determines how the duration dimension is computed.

### Contribution

The IMN "Contribution" dimension requires assessing: would this change have happened anyway without this intervention, and does the funder's involvement make a material difference?

CROSS addresses the "Contribution" dimension through the causality stance primitive (Part IV), which is a direct and precise operationalization of the IMN's contribution dimension:

- **Attribution stance**: requires counterfactual methodology demonstrating that the intervention produced change above the level expected without it. This is the IMN's strong contribution claim.
- **Contribution stance**: requires a documented causal pathway, acknowledgment of co-factors, and a materiality argument explaining why this funder's involvement made a meaningful difference. This is the IMN's standard contribution claim.

The IMN also recognizes the concept of a "contribution thesis" (developed by Impact Frontiers): a stated theory of how a specific investor or funder contributes to an outcome beyond providing capital. CROSS's causality stance and concurrent funding disclosure requirements together produce the structural basis for a contribution thesis: the funder declares their mode of contribution (attribution or contribution stance), acknowledges other contributors (co-factors and concurrent funders), and documents the causal pathway.

The concurrent funding disclosure requirement (Part VI) is additionally relevant here: it surfaces whether other funders are contributing to the same outcome, which is material to the IMN's contribution dimension. A program with multiple concurrent funders must document how each funder's contribution is distinct and material.

### Risk

The IMN "Risk" dimension requires identifying: the probability that impact is different from expected, including the risk of unintended negative consequences.

CROSS addresses the "Risk" dimension through:

- **Critical assumptions list in pathway registry** (Part IX-B, Section 3): each pathway declares the conditions that must hold for its causal mechanism to operate. These assumptions are the structural form of impact risk: if an assumption fails, the pathway's expected impact will not occur.
- **External risk list** (Part IX-B, Section 3): each pathway declares conditions external to the funder's control that could disrupt the pathway. This is the IMN's risk dimension at the causal architecture level.
- **Unintended outcomes disclosure** (Part IV, completion gate): surfaces both positive and negative unintended consequences, addressing the IMN's concern about impact that is different from expected in either direction.
- **Adverse Signal Engagement Principle** (ASEP, referenced from CROSS Part I): requires applicants to surface signals that contradict their self-presentation, including evidence of prior failures or contradictory findings. This is the IMN's risk transparency requirement applied at the application stage.

---

## The ABC Spectrum and CROSS Obligation Modes

The IMN (via the Impact Management Project) classifies impact-oriented activity along an "ABC" spectrum:

**Act to avoid harm (A)**: interventions designed to prevent or reduce negative outcomes. These are harm-reduction oriented: the primary obligation is to demonstrate that a harmful condition did not occur or was reduced.

**Benefit stakeholders (B)**: interventions designed to produce positive outcomes for specific people or communities. These are the standard outcome-oriented grants: the primary obligation is to demonstrate that a condition improved.

**Contribute to solutions (C)**: interventions designed to address systemic conditions or catalyze broader change beyond the direct beneficiaries. These are systemic-change oriented: the primary obligation is to demonstrate contribution to a long-term or systemic outcome.

This ABC spectrum maps to CROSS's ToC hierarchy:

| IMN Class | CROSS ToC Level | CROSS Obligation Mode |
| :-- | :-- | :-- |
| A (avoid harm) | Output level | Build-obligation: the deliverable prevents or reduces harm |
| B (benefit stakeholders) | Short-term or Intermediate Outcome | Change-obligation targeting measurable population-level change |
| C (contribute to solutions) | Long-term Outcome or Goal | Change-obligation with contribution stance; ToC pathway targeting systemic change |

This mapping enables programs to declare their IMN classification explicitly within their CROSS obligation mode configuration, making the class of impact claim visible to reviewers, analysts, and institutional funders at the round configuration level rather than requiring interpretation of project narratives.

---

## IRIS+ Integration

The Impact Management Norms are explicitly aligned with IRIS+ (the GIIN Impact Reporting and Investment Standards). IRIS+ provides the indicator catalog from which programs select specific indicators to populate the IMN's "What" and "How Much" dimensions.

CROSS's 11-field indicator specification is a strict superset of IRIS+ metadata requirements (see IRIS+ compatibility statement). The IMN, IRIS+, and CROSS are therefore fully compatible at the indicator level: a CROSS indicator specification that references an IRIS+ indicator ID satisfies both IRIS+ metadata requirements and IMN "What" and "How Much" dimension requirements simultaneously.

WALKRI's field specifications produce IRIS+ metadata as a structural consequence of conformance. A WALKRI-conformant field collecting IRIS+ indicator data satisfies IMN's collection instrument quality expectations without additional work.

---

## Who Should Declare IMN Compatibility

**Impact investors and investment vehicles**: Family offices, development finance institutions, and impact-first investment funds that use IMN as their primary impact management framework. CROSS+WALKRI provides the grants program equivalent of the investment-side IMN practice: a structured obligation architecture for grantees that produces IMN-compatible evidence.

**Programs seeking B Corp or GIIN membership alignment**: Both B Corp and GIIN use IMN-aligned frameworks as part of their assessment and membership requirements. CROSS+WALKRI-conformant programs produce IMN-compatible impact documentation that supports these assessments.

**Programs bridging grant-making and impact investment**: Development finance programs that combine grant-making with concessional loans or equity investments increasingly need a common impact framework across all instruments. IMN provides that common language; CROSS+WALKRI provides the structural implementation for the grants component.

---

## Adoption Guidance

Programs that currently use the IMN framework and are adopting CROSS+WALKRI should:

1. Map their IMN "What" dimension to CROSS obligation mode and indicator specification. The IMN impact category and outcome description translate directly to the CROSS indicator name, rationale, and domain tags.

2. Map their IMN "Who" dimension to the CROSS FROM state population specification and disaggregation fields. The affected population described in the IMN "Who" dimension is the population in the CROSS FROM state.

3. Map their IMN "How Much" dimension to the CROSS TO state, disaggregation specification, and sustainability stance. Scale maps to the aggregate TO state value; depth maps to the operational definition's threshold; duration maps to the sustainability stance at the continuation gate.

4. Declare a causality stance in CROSS that matches the IMN contribution claim. Attribution stance programs configure the completion gate at counterfactual reference level. Contribution stance programs require a causal pathway, co-factor acknowledgment, and materiality argument.

5. Use CROSS's pathway registry critical assumptions list and external risk list as the structured form of the IMN "Risk" dimension. Each assumption is an identified risk; each external risk list entry is an acknowledged external factor.

Programs that have not previously used the IMN framework will produce IMN-compatible impact documentation as a structural consequence of CROSS+WALKRI conformance. The five dimensions are fully addressed by the provisions listed above; no additional IMN-specific documentation is required.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

Impact Management Norms: impactmanagementnorms.com

IRIS+: iris.thegiin.org

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
