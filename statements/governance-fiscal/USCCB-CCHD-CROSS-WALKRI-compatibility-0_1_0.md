---
title: USCCB Catholic Campaign for Human Development (CCHD) Evaluation Criteria Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-18
license: CC0
standards: CROSS v0.4.4 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - https://www.usccb.org/committees/catholic-campaign-human-development/community-development-criteria-guidelines-and
  - https://www.usccb.org/committees/catholic-campaign-human-development/economic-development-criteria-and-guidelines
  - https://www.usccb.org/committees/catholic-campaign-human-development/grant-evaluation
---

# USCCB Catholic Campaign for Human Development (CCHD) Evaluation Criteria Compatibility - CROSS+WALKRI

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

This statement documents structural alignment between the United States Conference of Catholic Bishops' Catholic Campaign for Human Development grant evaluation criteria and the CROSS+WALKRI specification standards. CCHD administers two grant tracks, Community Development and Economic Development, each with formally published Criteria, Guidelines and Policies. The most analytically distinctive feature of the CCHD framework relative to all other frameworks in CROSS+WALKRI's coverage is the explicit faith-mission alignment criterion: both tracks require that funded organizations be consistent with Catholic moral and social teaching, and this is a formally published, enforceable evaluation criterion with no secular parallel. CROSS and WALKRI satisfy all CCHD structural evaluation requirements, and WALKRI specifically addresses the operationalization of the faith-mission criterion as a measurement instrument.

---

## The CCHD Evaluation Framework

The Catholic Campaign for Human Development is the US Catholic Bishops' domestic anti-poverty program, established in 1969. It distributes approximately $10 million annually to community organizations working to address the root causes of poverty in the United States. CCHD administers two distinct grant tracks with separate criteria documents.

The Community Development track funds organizations that build the power of low-income communities through organizing, advocacy, and community governance. The published Criteria, Guidelines and Policies for Community Development distinguishes between required criteria (mandatory eligibility conditions) and guidelines (strength factors that improve an application's competitiveness but are not absolute requirements). Required criteria include organizational capacity (demonstrated ability to manage grant funds), democratic governance (low-income individuals in decision-making roles), group self-sufficiency (evidence that the organization is building toward independence from external funding), and benefit to low-income populations (the primary beneficiaries must be people experiencing poverty).

The Economic Development track funds organizations that create economic opportunity through worker ownership, cooperative development, job creation, and wage improvement. Required criteria include evidence of community economic benefit, worker ownership or democratic governance structures, wage standards above poverty thresholds, and organizational financial capacity. Both tracks require a formal multi-stage evaluation process: diocesan director review via the Reviewer Portal, local bishop endorsement, and national subcommittee of bishops sign-off. A downloadable CCHD Economic Development Evaluation Form is publicly available, providing explicit transparency into evaluation criteria and scoring.

The faith-mission alignment criterion is formally published and enforceable in both tracks. Organizations must demonstrate that their governance, policies, and activities are consistent with Catholic moral and social teaching. This criterion is not a general values alignment statement; it is a formally listed evaluation criterion with stated consequences for non-compliance: organizations whose activities are inconsistent with Catholic moral and social teaching are ineligible for CCHD funding regardless of their merits on other criteria. The enforcement mechanism is the diocesan director and bishop review process, which includes assessment of faith-mission alignment before applications proceed to the national subcommittee.

No other framework in CROSS+WALKRI's current coverage includes a comparable faith-mission compliance criterion as a formally published, enforceable evaluation gate. The faith-mission criterion presents a distinctive operationalization challenge: unlike quantitative output or outcome criteria, faith-mission compliance requires that qualifying and non-qualifying examples be specified before the criterion can function as a measurement instrument rather than a post-hoc judgment.

---

## How CROSS Satisfies the CCHD Framework

CROSS satisfies CCHD's structural evaluation requirements through its entry specification gate, organizational identity fields, population scope declaration, and Change obligation indicators.

CCHD Community Development required criteria map to CROSS as follows. The organizational capacity criterion corresponds to CROSS's organizational identity fields, which require that the applicant organization's governance structure, disbursement authority, and financial management be declared before the round opens. These fields capture whether the organization has the structural capacity to manage grant funds, which is what the organizational capacity criterion requires. The democratic governance criterion, requiring low-income individuals in decision-making roles, corresponds to CROSS's governance structure field and the population scope declaration: the population the program is designed to benefit must be identified, and if democratic governance is a required criterion, the intake instrument must specify what evidence of low-income decision-making participation qualifies.

The group self-sufficiency criterion, requiring evidence of movement toward independence from external funding, corresponds to CROSS's concurrent funding declarations and Theory of Change sustainability field. CROSS requires that other funding sources be disclosed; for CCHD purposes, the self-sufficiency criterion requires that the Theory of Change include a pathway from current grant dependence toward organizational sustainability. CROSS's sustainability field captures this as a pre-specified commitment rather than a reporting aspiration.

The benefit to low-income populations criterion corresponds to CROSS's population scope declaration. CROSS requires that the population whose conditions the program is designed to affect be explicitly declared. For CCHD Community Development, the qualifying population is people experiencing poverty, and the population scope declaration must specify what income threshold defines the target population and what proportion of beneficiaries must fall within that threshold.

CCHD Economic Development criteria map to CROSS's Change obligation mode indicators at the employment and economic condition level. The job creation, wage level, and worker ownership criteria correspond to CROSS Fields 7-11: target condition (employment quality for low-income workers), baseline (current employment conditions), target threshold (number of jobs created, wage floor achieved, percentage of worker ownership), measurement timing, and comparison group if applicable. These fields operationalize the Economic Development criteria as pre-specified measurement commitments before any application is submitted.

The faith-mission alignment criterion corresponds to CROSS's compliance threshold field, which is WALKRI's fifth requirement. The compliance threshold field requires that qualifying and non-qualifying examples be specified for any compliance criterion before any applicant encounters the intake form. For the CCHD faith-mission criterion, this means the round specification must declare what activities, governance decisions, or organizational positions constitute non-compliance with Catholic moral and social teaching, so that the criterion functions as an evaluable gate rather than a post-hoc judgment.

| CCHD Criterion | CROSS Mechanism |
|---|---|
| Organizational capacity | Organizational identity fields: governance structure, disbursement authority, financial management |
| Democratic governance (low-income decision-making) | Governance structure field; population scope declaration |
| Group self-sufficiency | Concurrent funding declarations; Theory of Change sustainability field |
| Benefit to low-income populations | Population scope declaration; income threshold qualifying definition |
| Economic Development: jobs, wages, ownership | Change obligation Fields 7-11: employment condition indicators, baselines, targets |
| Faith-mission alignment with Catholic teaching | WALKRI compliance threshold field: qualifying/non-qualifying examples specified pre-publication |

---

## How WALKRI Complements This Alignment

WALKRI's pre-publication audit requirements are particularly important for the CCHD faith-mission alignment criterion. This criterion is structurally different from quantitative output and outcome criteria: it cannot be evaluated by counting outputs or measuring condition changes. It requires a judgment about organizational consistency with a normative framework. Without WALKRI's requirement that qualifying and non-qualifying examples be specified before any applicant encounters the criterion, the faith-mission criterion functions as a post-hoc judgment with no operationally defined standard, which makes it both unenforceably vague and vulnerable to inconsistent application across diocesan reviewers.

WALKRI's fifth requirement, the compliance threshold specification, requires that every compliance criterion specify before publication what evidence qualifies as compliance and what evidence disqualifies an applicant. For the CCHD faith-mission criterion, this means the diocesan director must, before opening the intake process, specify what categories of organizational activity or policy constitute non-compliance, what documentation the applicant must provide to demonstrate compliance, and what review procedure will be used to assess the documentation. When this specification is complete before any applicant encounters the form, the criterion becomes an auditable measurement instrument. When it is absent, it remains a values statement without operational definition.

WALKRI applies the same logic to all other CCHD criteria. The democratic governance criterion cannot function as a measurement instrument unless the intake form specifies what proportion of decision-making roles must be held by low-income individuals, what documentation constitutes evidence of that proportion, and what counts as a decision-making role. The self-sufficiency criterion cannot function as a measurement instrument unless the form specifies what trend in external funding dependence counts as progress toward self-sufficiency. In each case, WALKRI's pre-publication audit converts the criterion from an evaluative standard into a measurement instrument, making the evaluation process more consistent, more defensible, and more useful to applicants who are trying to understand what they need to demonstrate.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*
