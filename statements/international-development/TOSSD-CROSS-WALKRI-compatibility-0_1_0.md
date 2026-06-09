---
title: TOSSD Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - TOSSD Framework, https://tossd.online/about
  - TOSSD Reporting Instructions, tossd.online
  - UN Statistical Commission, TOSSD endorsement, 2019
  - IATI Standard v2.03, iatistandard.org
  - Bridging Data Systems for Financing for Development initiative, IATI/TOSSD co-development documentation
  - CROSS+WALKRI IATI Compatibility Statement v0.1.0
lens_tags:
  calibration_tier: process_conformant
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: multilateral_bank_or_fund
  framework_scope_type: accounting_financial
  # Total Official Support for Sustainable Development statistical framework; OECD-led but reporting universe includes multilaterals and non-DAC providers; accounting/disclosure scope
---

# TOSSD Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

CROSS-conformant programs operating in the Web3 public goods or open-source infrastructure space fall under TOSSD Pillar II (global and international public goods). CROSS Field 10 (institutional framework alignment) accommodates TOSSD pillar and sector category declarations. CROSS's Theory of Change architecture maps to TOSSD's causal logic requirements for SDG contribution claims. The organizational identity fields cover provider and activity identification requirements. A structural bridge exists through IATI: because TOSSD and IATI were co-developed in the "Bridging Data Systems for Financing for Development" initiative, IATI-compatible CROSS data is structurally compatible with TOSSD reporting.

TOSSD is a measurement framework for tracking total official support for the 2030 Agenda, including flows that fall outside traditional ODA reporting. CROSS is an obligation architecture for funded interventions. They operate at different layers and are complementary: CROSS produces the obligation records and evidence architecture that TOSSD requires as substantive input for provider reporting.

---

## What TOSSD Is

The Total Official Support for Sustainable Development (TOSSD) framework is the UN Statistical Commission-endorsed measurement system for tracking all official support mobilized for the 2030 Agenda. As of March 2026, 128 providers are reporting to TOSSD. The framework was developed by the OECD and the UN Statistical Commission and formally endorsed in 2019.

TOSSD has two pillars. Pillar I covers cross-border flows to developing countries: official support provided by governments, multilateral institutions, and private finance mobilized by official action that flows to recipient countries. Pillar II covers global public goods and international public goods: support for activities whose benefits are not confined to a single recipient country but contribute to the international system that makes the 2030 Agenda achievable. Pillar II is the pillar most directly relevant to Web3 public goods and open-source infrastructure grants, where the outputs are non-excludable, non-rival, and globally accessible.

TOSSD reporting requires providers to submit: a provider identifier, an activity description, sector classification using the TOSSD sector vocabulary (which aligns with OECD DAC CRS codes), geographic coverage or scope designation, SDG alignment, and the amount of support. For Pillar II activities, providers must additionally document why the supported activity qualifies as a global or international public good and how it contributes to the SDGs.

TOSSD and IATI were co-developed in the "Bridging Data Systems for Financing for Development" initiative. IATI activity data can be submitted as TOSSD-compatible input through a structured mapping; IATI-reporting providers satisfy TOSSD data format requirements through this bridge.

---

## Why Pillar II Is the Relevant Frame for Web3 Public Goods

Open-source software infrastructure, shared digital public goods, and Web3 protocol development are Pillar II activities under TOSSD's categorization framework. They are not cross-border flows to a specific developing country recipient; they are contributions to a shared global resource base whose benefits are structurally available to all countries and populations.

This categorization has practical consequences. Pillar II activities must satisfy a public goods qualification test: the activity must be shown to produce benefits that are non-excludable in nature or are made non-excludable by design, and that contribute to one or more SDG targets. CROSS's Theory of Change architecture, applied to a Pillar II program, produces the documentation needed to satisfy this test: the goal level specifies the SDG contribution claim, the outcome level specifies the population-level change the activity enables, the output level specifies the deliverable, and the causal link and assumption documentation specifies why the output plausibly produces the outcome.

CROSS's causality stance field (contribution versus attribution) is particularly relevant for Pillar II claims. TOSSD does not require programs to prove direct causation between their activity and an SDG outcome; it requires that the contribution pathway be documented and verifiable. CROSS's causality stance field encodes this methodological position formally, making the claim auditable.

---

## CROSS Field Mapping to TOSSD Required Fields

| TOSSD Required Field | CROSS/WALKRI Provision | Notes |
| :-- | :-- | :-- |
| Provider identification | On-chain identity anchor (Field 6); organizational identity declaration | CROSS requires a canonical organizational identity declaration. The on-chain identity anchor produces a stable, verifiable provider identifier. |
| Activity description | Theory of Change declaration (goal, outcome, output, activity levels); obligation mode and entry specification narrative | The CROSS ToC produces a structured activity description that exceeds the depth of a standard TOSSD activity description. The goal and outcome levels correspond to the TOSSD activity description requirement. |
| Sector classification (TOSSD vocabulary, CRS-aligned) | Indicator Field 10 (institutional framework alignment) | Programs declaring TOSSD sector category and CRS sector code alignment in Field 10 produce the sector classification TOSSD requires. The declaration is explicit, not inferred. |
| Geographic coverage or scope designation | Population field (Indicator Field 6) | For Pillar II activities, the geographic scope designation is "global" or "international." Field 6 accommodates this: the population scope can specify a global affected population without a country code. |
| SDG alignment | Theory of Change (goal level SDG linkage); Indicator Field 10 (framework alignment including SDG targets) | CROSS programs that declare SDG target alignment in the ToC goal level and in Field 10 produce the SDG documentation TOSSD requires. |
| Amount of support | No CROSS equivalent | Financial flow data. Outside CROSS scope; managed by the funding organization's financial systems. |
| Pillar II public goods qualification | Theory of Change architecture; causality stance field; obligation mode | The ToC goal level specifies the public goods claim. The causality stance field specifies the contribution pathway. Build-obligation programs produce output-level deliverables that can be assessed for public goods qualifying criteria. |
| SDG contribution explanation | Named causal links and assumptions in ToC architecture | CROSS's requirement to name causal links and document assumptions produces the contribution explanation that TOSSD's Pillar II public goods documentation requires. |

---

## The IATI Bridge

TOSSD and IATI were co-developed. The IATI Activity Standard produces TOSSD-compatible output through a structured field mapping maintained in the "Bridging Data Systems" initiative documentation. Providers that report to IATI satisfy TOSSD data format requirements for activity-level fields through this bridge, without separate TOSSD-specific data collection.

CROSS's IATI compatibility is separately documented in the CROSS+WALKRI IATI Compatibility Statement. Programs implementing CROSS under the IATI alignment pathway produce TOSSD-compatible output as a structural consequence: the CROSS gate record structure produces IATI-compatible data, which maps to TOSSD required fields through the IATI/TOSSD bridge.

For Web3 grants programs, this creates a single-source reporting architecture. A CROSS+WALKRI-conformant program operating as a Pillar II provider produces:

- DAOIP-5-compatible round and grant records, consumable by Web3 grants infrastructure including the OpenGrants Gateway;
- IATI-compatible activity data, consumable by institutional development sector transparency infrastructure;
- TOSSD-compatible activity data, consumable by the TOSSD reporting system through the IATI bridge;
- WALKRI-conformant field specifications that satisfy data quality requirements across all three ecosystems simultaneously.

No other grants specification framework produces data that is simultaneously consumable by these four reporting destinations from a single structured source.

---

## Sector Code Alignment: TOSSD Vocabulary and CRS Codes

TOSSD uses a sector vocabulary that aligns with the OECD DAC CRS five-digit sector codes. Web3 public goods programs should identify the CRS sector code that best represents their primary activity area. Common relevant categories include: information and communication technology (ICT, CRS code 220), general environmental protection (CRS code 410), democratic participation and civil society (CRS code 151), and research and development for development (CRS code 990).

Programs with outputs that serve multiple sectors should declare sector codes at the indicator cluster level in CROSS Field 10, since TOSSD accepts a primary sector designation per activity. The most granular declaration that accurately represents the primary public goods output is the appropriate choice. Programs uncertain about TOSSD sector categorization should consult the TOSSD Secretariat's guidance, available at tossd.online.

---

## Adoption Guidance

Web3 grants programs and implementing organizations seeking TOSSD reporting eligibility that adopt CROSS+WALKRI should:

1. Determine pillar classification. Programs with outputs that are globally accessible public goods are Pillar II programs. Programs with flows directed to specific recipient countries may qualify under Pillar I or both pillars. Assess this before configuring the obligation architecture.

2. Declare the TOSSD sector category and corresponding CRS sector code in Indicator Field 10 for each indicator cluster. This produces the machine-readable sector classification TOSSD requires at the activity level.

3. Specify SDG target alignment at the goal level of the Theory of Change architecture, and repeat the SDG reference in Field 10 for each indicator cluster that directly tracks SDG-relevant outcomes. This produces the SDG documentation TOSSD requires for contribution claims.

4. Use CROSS's causality stance field to declare contribution rather than attribution where the program's public goods outputs are upstream of complex SDG outcomes. This satisfies TOSSD's Pillar II public goods qualification documentation requirement without overclaiming direct causal attribution.

5. Implement IATI export from the CROSS gate record structure. Programs reporting under TOSSD that already produce IATI output satisfy TOSSD data format requirements through the IATI/TOSSD bridge; no separate TOSSD-specific reporting workflow is needed.

6. Apply WALKRI's five field requirements to all collection instruments. TOSSD does not specify collection instrument standards; WALKRI fills this gap and ensures that the data supporting TOSSD SDG contribution claims is produced by specified, auditable instruments rather than by undefined collection processes.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

TOSSD Framework: https://tossd.online/about

IATI Standard v2.03: iatistandard.org

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. Pillar II frame established for Web3 public goods. CROSS field mapping to TOSSD required fields. IATI bridge pathway documented. Sector code and SDG alignment guidance. Adoption guidance for Pillar II programs. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
