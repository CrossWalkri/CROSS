---
title: UNDP IRRF and ISO/UNDP 53001 Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - UNDP Integrated Results and Resources Framework (IRRF 2023, undp.org)
  - ISO/UNDP PAS 53002:2024 (free guidance document, iso.org/standard/53001)
  - ISO/UNDP 53001 Management Systems for SDG Contributions (forthcoming mid-2026)
---

# UNDP IRRF and ISO/UNDP 53001 Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS-conformant program satisfies the indicator documentation requirements of the UNDP Integrated Results and Resources Framework (IRRF) as a structural consequence of conformance. CROSS's eleven-field indicator specification covers every required IRRF indicator element, and CROSS's Theory of Change architecture maps to the IRRF's output-outcome-goal hierarchy without additional documentation.

For ISO/UNDP 53001, the forthcoming international certifiable standard for SDG contribution claims, CROSS's Change obligation mode and attribution claim strength dimension directly implement the causal specificity requirements that the standard will certify. A forward-looking compatibility note is provided here because the PAS 53002:2024 guidance document (available now) makes the mapping auditable before the full standard is finalized.

---

## What the UNDP IRRF Is

The UNDP Integrated Results and Resources Framework (IRRF) is UNDP's corporate results reporting architecture. All UNDP country offices report annual results against SDG-linked output and outcome indicators using the IRRF structure. Programs administered by UNDP, including Global Fund and GEF grants, require IRRF-aligned indicator frameworks at the program level, with grantee-level reporting feeding into Results-Oriented Annual Reports (ROARs).

The IRRF organizes indicators at two levels. PDO-level (Programme Development Outcome) indicators measure outcomes: measurable changes in the state of affairs that the program is designed to produce. IR-level (Intermediate Results) indicators measure outputs: the deliverables and activities that contribute to the outcome. Every indicator at both levels requires: a name, a definition, a unit of measure, a baseline, a target, a data source, a collection method, a reporting frequency, and a responsible party.

The IRRF does not specify what makes a field a measurement instrument before data is collected. WALKRI fills that gap.

---

## What ISO/UNDP 53001 Is

ISO/UNDP 53001 is a forthcoming international management systems standard specifying requirements for any organization seeking to certify that its activities demonstrably contribute to the UN Sustainable Development Goals. The accompanying guidance document, ISO/UNDP PAS 53002:2024, is available now as a free download.

The standard distinguishes between SDG claims that are asserted and SDG contributions that are demonstrated. To demonstrate contribution rather than assert it, an organization must: specify the SDG target to which it contributes, define a measurable indicator tracking progress toward that target, establish a baseline, set a target value, document the causal mechanism connecting its activities to the SDG outcome, state its attribution claim (full attribution vs contribution), and provide independently verifiable evidence.

These requirements are structurally identical to CROSS's Change obligation mode applied at the SDG indicator level.

---

## How CROSS Satisfies the UNDP IRRF

CROSS's eleven-field indicator specification satisfies all IRRF indicator documentation requirements at both PDO and IR levels.

| UNDP IRRF element | CROSS field(s) |
|:--|:--|
| Indicator name | Field 1: Indicator name |
| Definition | Field 2: Definition |
| Unit of measure | Field 3: Unit of measure |
| Baseline value | Field 4: Baseline value |
| Target value | Field 5: Target value |
| Disaggregation / population scope | Field 6: Population scope |
| Data source | Field 7: Data source |
| Collection method | Field 8: Collection frequency |
| Responsible party | Field 9: Responsible party |
| PDO-level (outcome) indicator designation | CROSS ToC architecture outcome level |
| IR-level (output) indicator designation | CROSS ToC architecture output level |

The PDO/IR level distinction is expressed in CROSS through the Theory of Change architecture's causal hierarchy. Outcome-level indicators in the CROSS ToC registry correspond to PDO indicators in the IRRF. Output-level indicators in the CROSS ToC registry correspond to IR indicators. The same indicator specification fields apply at both levels; the level is determined by the causal position in the ToC, which CROSS requires to be declared.

A program reporting to a UNDP-administered grant that implements CROSS does not produce IRRF indicator documentation separately. The CROSS round specification produces it as a structural output.

---

## How CROSS Satisfies ISO/UNDP 53001 Requirements

The ISO/UNDP PAS 53002:2024 guidance document specifies six demonstration requirements for a credible SDG contribution claim. CROSS's Change obligation mode satisfies all six.

| ISO/UNDP 53001 requirement | CROSS provision |
|:--|:--|
| Named SDG target | Field 10: Institutional framework alignment (SDG target reference) |
| Measurable indicator linked to SDG target | Fields 1-3: Indicator name, definition, unit |
| Documented baseline | Field 4: Baseline value |
| Stated target | Field 5: Target value |
| Causal mechanism connecting activities to outcome | CROSS ToC architecture, causal link documentation |
| Attribution claim (full vs contribution) | Field 11: Causality stance |

The causality stance field is the most critical alignment point. ISO/UNDP 53001 distinguishes between programs that claim full attribution for an SDG outcome (the program caused the change) and programs that claim contribution (the program contributed to a change that also had other causes). CROSS's attribution claim strength dimension, configurable per round, encodes exactly this distinction and requires it to be declared in the round specification before any applicant submits. Programs that make unsupported attribution claims fail the entry specification gate; programs that correctly distinguish contribution from attribution pass it.

---

## How WALKRI Complements This Alignment

The IRRF and ISO/UNDP 53001 specify what indicators must document. Neither specifies what makes the intake fields collecting that documentation into measurement instruments. WALKRI addresses that gap.

A WALKRI-conformant field collecting baseline data for an IRRF indicator must specify: the criterion intent (what the baseline field measures), the operational definition (the unit of analysis and qualifying counting rules), the response form (why the field type matches the criterion), the evidence form (the artifact type and access path proving the baseline value), and the compliance threshold (if the baseline draws from a defined external standard or registry).

A label version of "baseline value" collects any number the applicant chooses to enter. A WALKRI-conformant version of the same field specifies the unit, the counting rule, the time period, the population, and the evidence the reviewer must verify before the baseline is accepted. The IRRF requires that baseline data be verifiable; WALKRI provides the field architecture that makes verifiability structural rather than aspirational.

---

## Forward Note on ISO/UNDP 53001 Finalization

ISO/UNDP 53001 is expected to be finalized in mid-2026. This compatibility statement is based on the PAS 53002:2024 guidance document, which is the authoritative pre-publication reference. When the full standard is published, this statement will be reviewed and updated to confirm alignment with the final text. The structural compatibility described here is based on the requirements as specified in PAS 53002:2024 and is expected to hold without modification.

The most material change between PAS 53002:2024 and the final ISO/UNDP 53001 standard, if any, is likely to be in certification procedure requirements rather than in the substantive content requirements that CROSS satisfies. CROSS adoption does not need to wait for the final standard.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
