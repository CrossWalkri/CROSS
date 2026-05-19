---
title: OECD DAC Blended Finance Guidance 2025 Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/cross-walkri/CROSS), WALKRI v0.1.6 (github.com/cross-walkri/WALKRI)
references:
  - OECD DAC Blended Finance Guidance 2025, https://www.oecd.org/en/publications/oecd-dac-blended-finance-guidance-2025_e4a13d2c-en/
---

# OECD DAC Blended Finance Guidance 2025 Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

CROSS and WALKRI together address OECD DAC Blended Finance Guidance 2025 Principle 5 (Monitor for transparency and results) at the specification layer. Principle 5 requires a shared theory of change developed jointly with co-investors, KPIs agreed before activities begin, and harmonized reporting across all capital providers. CROSS implements each of these requirements structurally through its gate architecture, ToC specification, and concurrent funding disclosure provisions.

This statement is distinct from existing CROSS+WALKRI alignment documentation covering the OECD DAC Evaluation Criteria. The Blended Finance Guidance governs co-investment structures where official development finance is combined with private capital; the Evaluation Criteria govern the quality of evaluations conducted on any development program. The two frameworks address different functions, and the structural mappings are different.

This compatibility matters for development finance institutions structuring blended vehicles, for fund managers deploying ODA-catalyzed capital, and for co-investors in blended structures who need a shared reporting layer that satisfies Principle 5 requirements for all parties simultaneously.

---

## What the OECD DAC Blended Finance Guidance 2025 Is

The OECD DAC Blended Finance Guidance 2025 is the current normative reference for official development assistance actors entering blended finance structures. It updates the 2020 guidance in response to evidence from a decade of blended finance practice and addresses five principles: mobilize private finance for development, support sustainable development in developing countries, pursue transparent, responsible, and inclusive development finance, align interests of all investors, and monitor for transparency and results.

Principle 5 is the measurement and accountability principle. It operates at the deal and portfolio level: it is concerned with what is measured, when KPIs are set, how results data is shared across capital providers, and what theory of change structures the monitoring framework. Its requirements apply to blended vehicles, to individual transactions within those vehicles, and to the co-investment relationships that blended structures involve.

The principle is operationally demanding in the blended context because multiple investors with different accountability systems must produce harmonized results data from a shared intervention. A single intervention cannot run parallel measurement architectures for different investors without producing incomparable data. Principle 5's harmonization requirement is the structural recognition that shared measurement must be specified jointly and early.

---

## Principle 5: Structural Mappings

**Shared theory of change developed jointly with co-investors.** CROSS's ToC architecture requires explicit documentation of goals, outcomes, outputs, and activities with named causal links and stated assumptions before the entry gate closes. In a blended structure, the obligation record documenting this ToC is a shared artifact. Each co-investor's performance expectations are anchored to the same ToC, and deviations from the ToC trigger gate evidence requirements. The "jointly developed" requirement is satisfied structurally: the ToC is not a funder's internal document but a gate-locked specification that all parties' grant records reference.

**KPIs agreed from the start.** CROSS's entry specification gate is the gate at which the eleven-field indicator specification is finalized. Fields 1 through 11 (name, definition, unit, baseline, target, population scope, disaggregation, collection methodology, collection frequency, evidence form, and compliance threshold) are locked at entry. No KPI can be added, removed, or redefined after the entry gate closes without a formal gate record of the change and its rationale. This is a structural implementation of "agreed from the start": the gate architecture makes late KPI changes visible, traceable, and formally documented rather than allowing quiet drift.

**Harmonized reporting across capital providers.** CROSS obligation records are not investor-specific documents; they are obligation-level specifications that apply to the grant program regardless of which capital tranche is being reported against. A blended vehicle using CROSS for its grant facility produces one indicator specification that all capital providers' reporting references. WALKRI's five field requirements, applied before the measurement instruments are published, ensure that the collection instruments producing actuals are internally consistent and replicable; this is the instrument-level precondition for data that multiple investors can rely on simultaneously.

**Additionality and causality.** The causality stance field in CROSS requires the program to declare what attribution claim it is making and on what basis. In the blended finance context, this field is the structural location for the additionality argument: the program must state whether it is claiming that the intervention produces outcomes that would not have occurred absent the blended structure, and what counterfactual logic supports that claim. The causality stance field does not adjudicate the additionality claim; it requires that the claim be stated explicitly and consistently across reporting cycles, enabling co-investors to assess it.

**Concurrent funding disclosure.** CROSS's concurrent funding disclosure provision requires programs to declare all co-financing and capital relationships in the obligation record. In a blended structure, this provision produces the transparency layer that Principle 5 requires across capital providers: each provider's contribution is documented in the same record that documents the shared ToC and KPIs.

---

## Scope Limitations

Principle 5 also addresses portfolio-level monitoring aggregation across multiple blended transactions, co-investor-level reporting obligations to home-country disclosure regimes, and private capital mobilization attribution methodology. These are governance and reporting system questions that are outside the specification layer addressed by CROSS and WALKRI. This statement addresses only the transaction-level specification layer where CROSS and WALKRI operate.

---

## Structural Mapping Table

| Principle 5 Requirement | CROSS Provision | WALKRI Provision | Coverage |
| :-- | :-- | :-- | :-- |
| Shared theory of change | ToC architecture (goal/outcome/output/activity with named causal links); gate-locked before entry closes | No direct provision | Structural: ToC is a shared obligation artifact |
| KPIs agreed from the start | Entry specification gate; eleven-field indicator specification (Fields 1-11) locked at entry | Five pre-publication field requirements ensure instruments match field specifications | Structural: gate architecture enforces pre-specification |
| Harmonized reporting across capital providers | Obligation record is specification-layer artifact, not investor-specific | Validity, reliability, and integrity requirements ensure instrument consistency across programs | Structural: one indicator specification, multiple capital provider reference |
| Additionality / causality | Causality stance field: explicit attribution claim required | No direct provision | Structural: additionality claim must be stated explicitly |
| Concurrent funding disclosure | Concurrent funding disclosure provision in obligation architecture | No direct provision | Structural: co-financing documented in obligation record |

---

## Further Information

CROSS: github.com/cross-walkri/CROSS

WALKRI: github.com/cross-walkri/WALKRI

OECD DAC Blended Finance Guidance 2025: https://www.oecd.org/en/publications/oecd-dac-blended-finance-guidance-2025_e4a13d2c-en/

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. Principle 5 analyzed in full. Concurrent funding disclosure, ToC architecture, causality stance, and entry specification gate mappings documented. Scope limitations identified. |
