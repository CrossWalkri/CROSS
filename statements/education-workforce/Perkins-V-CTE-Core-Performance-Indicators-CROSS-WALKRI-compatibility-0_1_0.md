---
title: Perkins V CTE Core Performance Indicators Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.5 (github.com/cross-walkri/CROSS), WALKRI v0.1.7 (github.com/cross-walkri/WALKRI)
references:
  - Strengthening Career and Technical Education for the 21st Century Act (Perkins V), 20 USC Chapter 44
  - cte.ed.gov/accountability/core-indicators
  - 20 USC Chapter 44 (Carl D. Perkins Career and Technical Education Act)
  - State Determined Performance Level (SDPL) Guidance (ED/OCTAE)
---

# Perkins V Career and Technical Education Core Performance Indicators

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Strengthening Career and Technical Education for the 21st Century Act (Perkins V), codified at 20 USC Chapter 44, establishes the federal framework for career and technical education (CTE) funding in the United States. The act fixes its core performance indicators by statute: no state may substitute, omit, or redefine the indicator categories, making Perkins V the most binding expression of CROSS's entry specification gate in US federal education grant-making. CROSS+WALKRI satisfies Perkins V's accountability requirements structurally, and WALKRI's pre-publication requirements address the data quality risk introduced when CTE program intake instruments are designed to generate Perkins V disaggregation data without standardized specification of what documentation qualifies a student for each status category.

---

## The Perkins V Core Performance Indicator Framework

Perkins V establishes two sets of core performance indicators: one for secondary CTE programs (grades 9-12) and one for postsecondary CTE programs. Secondary indicators include the graduation rate, academic proficiency in reading and language arts, academic proficiency in mathematics, postsecondary placement (measured as further education or employment), and three program quality indicators covering postsecondary credential attainment during secondary enrollment, dual or concurrent enrollment participation, and work-based learning participation. Postsecondary indicators include credential attainment, enrollment in further education or advanced training, employment status, and earnings.

States set state-determined performance levels through a public comment process before any program year begins. Local eligible recipients negotiate performance levels with state agencies separately, creating a two-tier accountability structure: state-level performance levels and local-level performance levels are both pre-specified before any CTE enrollment occurs. Programs that fail to reach 90% of their negotiated performance levels in any indicator trigger a required local improvement plan. Sustained failure triggers sanctions.

The statute requires disaggregated reporting by gender, race and ethnicity, and eight special population categories: students with disabilities, English learners, economically disadvantaged students, single parents, out-of-workforce individuals, homeless individuals, youth in foster care or aging out of foster care, and youth with a parent who is an active duty military member. These disaggregation requirements are fixed by statute: states and local recipients cannot omit any special population category from their reporting, regardless of the demographic composition of their enrollees.

---

## How CROSS Satisfies the Perkins V Performance Indicator Framework

CROSS addresses Perkins V's core performance indicator requirements at the structural level, from the statutory indicator categories through the dual-tier accountability structure and the disaggregation requirements.

| Perkins V Accountability Element | CROSS Provision |
|:--|:--|
| Legislatively fixed indicator categories (no state substitution permitted) | Entry specification gate at statutory level: indicator domains are fixed before any state plan is submitted |
| State-determined performance levels, public comment process, pre-program-year | Field 5 (target): performance levels established through a formal process before the program year, not retrospectively |
| Local performance levels negotiated with state | Portfolio aggregation: local recipient performance levels pre-specified and aggregated to state-level performance |
| Secondary indicators (graduation, academic proficiency, postsecondary placement) | Fields 1-5 (name, definition, unit, baseline, target) for each statutory indicator |
| Program quality indicators (credential attainment, dual enrollment, work-based learning) | Fields 1-5 + Field 6 (timing: during secondary enrollment for quality indicators) |
| Postsecondary indicators (credential attainment, employment, earnings) | Fields 1-5 + Field 6 (timing: after exit for employment and earnings indicators) |
| 90% threshold improvement plan trigger | Field 11 (evidence threshold): statutory performance threshold constitutes the accountability cycle's evidence threshold |
| Disaggregation by gender, race/ethnicity, and eight special population categories | Disaggregation ratchet: all statutory demographic categories established at enrollment and maintained across all reporting periods |
| Two-tier accountability (state and local recipient) | Portfolio aggregation: local recipient outcomes aggregate to state-level outcomes, with both tiers pre-specified |
| Public comment on state-determined performance levels | Entry specification gate: public comment process occurs before performance levels are finalized, before any program year begins |

Perkins V's legislatively fixed indicator categories constitute the most binding form of the entry specification gate in US federal grant-making. Where other frameworks (WIOA, SNAP-Ed, Perkins' own precursors) allow some funder or grantee discretion in indicator selection, Perkins V eliminates that discretion for core indicators entirely: the indicator categories are established by Congress, and no state education agency or local CTE program can substitute its own preferred measurement domains. This means that a CTE program's CROSS conformance for the Perkins V indicator set begins with a set of Fields 1 through 4 (name, definition, unit, baseline) that are largely satisfied by the statute and its implementing guidance before any program plan is written.

The dual-tier accountability structure corresponds to CROSS's portfolio aggregation capability. State-level Perkins V performance levels are the aggregation of local eligible recipient outcomes, and both levels are pre-specified before the program year begins through a process that is itself regulated. A state that applies CROSS to its Perkins V system has a pre-specified indicator specification at both the state level and the local level, with the local specifications feeding into the state-level aggregation in a manner that is traceable from the entry specification gate through the completion gate.

The statutory disaggregation requirements correspond to CROSS's disaggregation ratchet at the strongest possible regulatory level. Perkins V's eight special population categories are fixed by statute; they cannot be omitted by any state or local program regardless of enrollment demographics or local preference. CROSS's disaggregation ratchet encodes this same protection as a structural principle: once a demographic dimension is captured at the entry specification gate, it cannot be removed in subsequent rounds. Perkins V makes this non-removal obligation a matter of federal law.

---

## How WALKRI Complements This Alignment

WALKRI's five pre-publication requirements address the data quality risk that Perkins V's special population disaggregation requirements create at the intake instrument level. The statute specifies eight special population categories and requires disaggregated reporting for each. What the statute does not specify is what documentation a CTE program intake worker must examine before coding a student as economically disadvantaged, what classification process applies to a student who qualifies for multiple special population categories, or what evidence standard applies when a student's special population status changes mid-enrollment.

These determination gaps are resolved by WALKRI's operational definition and evidence form requirements, applied to CTE program intake instruments before any student is enrolled. A WALKRI-conformant CTE intake form for the economically disadvantaged category specifies exactly which income and program participation documentation qualifies, which verification method is required when a student self-reports without documentation, and how the intake worker codes a student whose documentation arrives after initial enrollment. Applied across all eight special population categories before any enrollment period opens, WALKRI's requirements produce intake instruments that generate Perkins V disaggregation data from a consistent evidentiary base.

The program quality indicators raise a distinct WALKRI challenge. Work-based learning participation is a statutory indicator, but what qualifies as work-based learning ranges from job shadowing to paid internship to apprenticeship, and different CTE programs define the qualifying threshold differently. WALKRI's criterion intent requirement, applied before the program year opens, requires the program to specify which work-based learning modalities it is counting and what minimum participation constitutes a qualifying event. This pre-specification prevents post-hoc expansion of the definition to improve apparent performance, which is exactly the integrity protection that the evidence threshold and compliance threshold requirements in WALKRI are designed to provide.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/cross-walkri.*
