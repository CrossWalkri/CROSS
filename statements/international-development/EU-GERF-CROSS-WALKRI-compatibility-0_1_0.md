---
title: EU Global Europe Results Framework Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.0 (github.com/cross-walkri/CROSS), WALKRI v0.1.6 (github.com/cross-walkri/WALKRI)
references:
  - EU DG INTPA Global Europe Results Framework (GERF)
  - NDICI-Global Europe, EU External Assistance Regulation
  - EU Capacity4Dev Results and Indicators Library, https://capacity4dev.europa.eu/resources/results-indicators_en
  - OECD DAC Creditor Reporting System (CRS)
---

# EU Global Europe Results Framework Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

A CROSS+WALKRI-conformant program satisfies EU DG INTPA Global Europe Results Framework (GERF) documentation requirements as a structural consequence of conformance. The Global Europe Results Framework governs all EU external development funding under the NDICI-Global Europe instrument, requiring results chains, predefined core indicators per sector, and indicator definition before implementation. All programs must report to the OECD DAC Creditor Reporting System.

CROSS's Theory of Change architecture maps directly to the GERF results chain. CROSS's OECD DAC alignment, documented separately in the CROSS+WALKRI OECD DAC Creditor Reporting System Compatibility Statement, covers the statistical reporting dimension. CROSS Field 10 accommodates GERF sector codes and core indicator references. A program funded under NDICI-Global Europe that implements CROSS satisfies GERF indicator documentation requirements as a structural consequence of conformance, without additional documentation work.

---

## What GERF Requires

DG INTPA operates the Global Europe Results Framework for all EU external development programming. Core requirements at program design stage:

1. A results chain specified before implementation, structured as input, activity, output, outcome, and impact levels
2. Core indicators per sector selected from DG INTPA's published library of ready-to-use results chains
3. All indicators defined before implementation, with baselines and targets
4. Data sources specified and confirmed as accessible before indicator adoption
5. Reporting via the OPSYS information management platform throughout the program lifecycle
6. Alignment with OECD DAC CRS for all statistical reporting obligations
7. Sector code declarations aligned to the GERF sector classification system

The EU Capacity4dev platform publishes sector-specific results chains that programs may adopt or adapt. Programs that adopt a published results chain must implement its core indicator set.

---

## Theory of Change Architecture Mapped to the GERF Results Chain

CROSS's Theory of Change architecture specifies four levels: goal, outcome, output, and activity. The GERF results chain specifies five levels: impact, outcome, output, activity, and input.

The mapping between these levels is direct at three of the four levels CROSS governs.

| GERF Results Chain Level | CROSS Theory of Change Level | Notes |
| :-- | :-- | :-- |
| Impact | Goal | The GERF impact level corresponds to the CROSS goal level: the long-horizon change in systemic conditions that the program contributes to |
| Outcome | Outcome | Direct correspondence. CROSS's intermediate and long-term outcome registers map to the GERF outcome level |
| Output | Output | Direct correspondence |
| Activity | Activity | Direct correspondence |
| Input | No CROSS equivalent | Input specification is outside CROSS scope. GERF inputs are managed by the grantee's financial and procurement systems |

**Result:** Four of the five GERF results chain levels have direct CROSS equivalents. The input level is outside CROSS scope and is managed by financial and procurement systems. A CROSS-conformant program's Theory of Change declaration produces the GERF results chain documentation for the four levels CROSS governs.

---

## Core Indicator and Sector Code Alignment

GERF core indicators are predefined per sector in DG INTPA's library. Programs selecting a sector results chain must implement its core indicator set. These indicators have defined names, definitions, and data sources in the published library.

CROSS Field 10 (institutional framework alignment) accommodates external framework codes and sector classifications. Programs implementing a GERF sector results chain should declare the GERF sector code and core indicator references in Field 10 for each indicator that originates from the DG INTPA library. This makes the GERF indicator provenance explicit and auditable within the CROSS obligation architecture.

For programs with multi-sector portfolios, GERF allows sector classification at the activity level. CROSS Field 10 declarations at the indicator level preserve this granularity, since each indicator carries its own Field 10 declaration independently.

---

## OECD DAC CRS Alignment

All EU programs funded under NDICI-Global Europe must report to the OECD DAC Creditor Reporting System. CROSS's OECD DAC Creditor Reporting System compatibility is documented separately. The structural summary: CROSS's eleven-field indicator specification produces the programmatic fields of CRS compliance (project title, project description, recipient country code, sector code, channel code, expected start date, expected end date) through its standard obligation architecture.

Programs that implement CROSS under GERF alignment satisfy both the GERF indicator documentation requirements and the CRS programmatic field requirements through a single conformance pathway. The two frameworks do not require separate documentation streams for the fields CROSS governs.

---

## OPSYS Reporting and Gate Architecture

DG INTPA requires programs to report progress through the OPSYS information management platform at prescribed intervals throughout the program lifecycle. CROSS's progress verification gates produce the review-point documentation that OPSYS reporting requires. Gate evidence submissions correspond to OPSYS progress reports; gate configurations produce the reporting schedule.

Programs using CROSS with GERF alignment should configure progress verification gate schedules to match OPSYS reporting intervals. The gate evidence package produced at each progress verification gate can then be used directly as the basis for OPSYS submissions.

---

## WALKRI and Data Quality

DG INTPA expects indicator data to meet the quality standards it publishes for the GERF indicator library. WALKRI's five data quality standards (validity, reliability, precision, integrity, timeliness) are applied at field specification stage, ensuring that intake fields collecting GERF indicator data are measurement instruments before deployment. This is the same quality assurance logic that the GERF indicator library applies when defining core indicators: the library's indicator definitions specify collection methods and data quality expectations at design time.

---

## Adoption Guidance

Programs funded under NDICI-Global Europe that adopt CROSS+WALKRI should:

1. Select the applicable GERF sector results chain from the DG INTPA library. Declare the sector code and core indicator references in Field 10 for each indicator from the published chain.

2. Configure the Theory of Change declaration at goal, outcome, output, and activity levels to match the GERF results chain for the selected sector. This produces the results chain documentation GERF requires.

3. Configure the entry specification gate to be complete before implementation authorization. All indicator specifications must be locked at this gate, satisfying GERF's pre-implementation indicator definition requirement.

4. Configure progress verification gates to align with OPSYS reporting intervals.

5. Declare OECD DAC sector codes in Field 10 alongside GERF sector codes for programs with CRS reporting obligations. This produces the sector classification documentation both frameworks require from a single field declaration.

---

## Further Information

CROSS: github.com/cross-walkri/CROSS

WALKRI: github.com/cross-walkri/WALKRI

EU Capacity4Dev Results and Indicators Library: https://capacity4dev.europa.eu/resources/results-indicators_en

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-05-18 | Initial draft. GERF results chain mapped to CROSS Theory of Change architecture. Core indicator and sector code alignment documented. OECD DAC CRS bridge documented. OPSYS reporting interval alignment mapped to gate schedule. WALKRI data quality standards mapped to GERF indicator quality expectations. |
