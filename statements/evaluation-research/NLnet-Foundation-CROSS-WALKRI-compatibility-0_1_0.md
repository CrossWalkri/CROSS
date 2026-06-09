---
title: NLnet Foundation Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - NLnet Foundation (https://nlnet.nl/)
  - NLnet Apply for a grant (https://nlnet.nl/propose/)
  - NLnet Open Application for Project Financing (https://nlnet.nl/foundation/request/application.html)
  - NGI Assure Guide for Applicants (https://nlnet.nl/assure/guideforapplicants/)
  - User-Operated Internet Fund Guide for Applicants (https://nlnet.nl/useroperated/guideforapplicants/)
  - NGI Zero Commons Fund (https://nlnet.nl/commonsfund/)
  - NGI Fediversity (https://nlnet.nl/fediversity/)
  - European Commission Next Generation Internet initiative (https://www.ngi.eu/)
lens_tags:
  calibration_tier: process_conformant
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: private_foundation
  framework_scope_type: allocator_process
  # NLnet Foundation small-grants program for open-source internet research
---

# NLnet Foundation Compatibility - CROSS+WALKRI

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

NLnet Foundation operates a family of grant programs (NGI Zero Commons, NGI Assure, NGI Fediversity, User-Operated Internet, NGI TALER, and adjacent funds) that fund free/libre/open source technology contributing to the open internet. The funds share a common applicant framework anchored on four eligibility-and-conduct requirements: an open license obligation, a peaceful and humane use clause, free availability of project results, and a dissemination commitment by the project team. A two-reviewer eligibility check governs proposal assessment, with a weighted-score threshold required to advance. NLnet's published criteria are stronger than typical for FOSS funders because they apply consistently across funds and are stated as binding conditions, not aspirations. They are, however, primarily eligibility-and-conduct criteria rather than outcome measurement requirements. CROSS+WALKRI accommodates this framework structure directly: Build obligation mode is the operative mode for deliverable-anchored FOSS grants, the public benefit mechanism declaration captures the license-and-access obligations, and dissemination commitments map to disclosure obligations declarable in the program's round configuration. NLnet's funds flow from the European Commission's Next Generation Internet initiative under Horizon 2020 and Horizon Europe grant agreements, which connects this statement to the existing CROSS+WALKRI coverage of EU research funding instruments.

---

## The NLnet Foundation Framework

NLnet Foundation, established in 1997 and based in the Netherlands, supports development of the open internet through a suite of grant programs operated as the implementing partner for the European Commission's Next Generation Internet (NGI) initiative. The bulk of NLnet's grantmaking is funded through Horizon 2020 and Horizon Europe grant agreements administered by the European Commission, with NLnet acting as the consortium lead distributing sub-grants to projects, individuals, and small organizations across Europe and beyond. Active funds at the time of writing include NGI Zero Commons (the broadest in scope, covering internet commons technologies), NGI Assure (trust, identity, and integrity technologies with a European dimension requirement), NGI Fediversity (federated social and cloud infrastructure), User-Operated Internet (user-controlled infrastructure and protocols), and NGI TALER (a payment system pilot). Grant amounts typically range from €5,000 to €50,000 with a lifetime per-recipient cap (€200,000 in NGI Assure) and bimonthly rolling deadlines.

The framework that governs applicant eligibility is consistent across funds, with per-fund variations described in each fund's published guide for applicants. The common elements are the following.

**Open license requirement.** All software and hardware produced under the grant must be published under a recognized free and open source license, in its entirety. All scientific outcomes must be published as open access. This is not an encouragement; it is a binding condition for successful project conclusion. NLnet's guidance specifically references OSI and FSF license recognition rather than admitting "source available" or non-commercial-restricted licenses by default.

**Peaceful and humane use clause.** The technology created within a funded project must be intended for peaceful and humane purposes. This is one of the four published eligibility criteria stated on NLnet's open application page and applies across funds. The clause is operationalized as an eligibility gate at proposal screening, not as an outcome to be measured during or after the grant.

**Free availability of project results.** Project results must be available to all at no cost, either as part of a proposed open standard or through an open license for software or hardware deliverables. This pairs with the open license requirement: the license satisfies the legal mechanism of free availability, and the project's deployment, repository, or specification access satisfies the practical mechanism.

**Dissemination commitment.** The project team must undertake adequate efforts to disseminate project results. NLnet's evaluation criteria reward demonstrable plans to reach relevant communities (developers, users, standards bodies, civil society) rather than treating publication of code as sufficient on its own. Dissemination is treated as part of the public good the grant funds, not as a downstream consequence.

**Two-reviewer eligibility check.** Each proposal is assessed by two independent expert reviewers on three weighted criteria: technical excellence and feasibility (30%), relevance and impact and strategic potential (40%), and cost-effectiveness and value for money (30%). The total weighted score must exceed 5 out of 7 to advance to the second stage, in which reviewers engage in clarifying dialogue with applicants and conduct independent fact-checking before final rating.

**Disqualifying conditions.** NLnet's published criteria explicitly exclude organizations in liquidation, enterprises in difficulty, and entities excluded from EU funding under national or EU law. These conditions reflect the European Commission's prime contractor obligations on NLnet and apply across funds derived from NGI funding.

**Reporting during the grant.** Reporting requirements are configured per fund and per project through a milestone-and-deliverable structure agreed at the award stage rather than through a single published measurement methodology. Successful project conclusion requires that deliverables be publicly available under recognized open or free licenses, with the dissemination commitment fulfilled.

The framework is, in CROSS+WALKRI terms, eligibility-and-conduct anchored. NLnet specifies who can be funded, what they must produce, how they must license it, and how reviewers assess proposals. NLnet does not specify a population-level outcome to be measured, a counterfactual baseline against which impact must be assessed, or a quantitative indicator framework that grantees must report against. The framework's verification obligation rests on the deliverable existing, being licensed correctly, being publicly accessible, and being disseminated, not on a measured change in a population.

---

## How CROSS Accommodates the NLnet Framework

CROSS's three obligation modes give NLnet's eligibility-and-conduct framework a structural home without forcing it into an outcome-measurement frame it does not claim. The mapping is direct.

**Build obligation mode is the operative mode for NLnet-funded projects.** NLnet funds projects that produce a specified deliverable: a software library, a hardware design, a protocol specification, a working federated service, a security audit, a documentation set. The entry specification gate in Build obligation mode asks whether the applicant can name a falsifiable deliverable with independently verifiable completion criteria. NLnet's two-reviewer eligibility check on technical excellence and feasibility is functionally this assessment, conducted by domain experts before funds are committed. The completion verification gate in Build mode requires that the deliverable exist, meet stated completion criteria, and be publicly accessible. NLnet's project conclusion conditions (deliverables publicly available under open licenses, dissemination commitment fulfilled) are the same content. A CROSS-conformant program that funds FOSS development in Build mode does not need to add a measurement framework that NLnet does not have; it implements the same architecture under explicit names.

**The public benefit mechanism declaration captures NLnet's license-and-access obligations directly.** CROSS's public benefit mechanism primitive recognizes four mechanism types (output production, access provision, condition change, ecosystem shift), each with its own evidence scope and access condition requirements. NLnet's typical grant operates through output production: the funded work produces an artifact, and the access condition is the open license under which it is released. CROSS Part IV requires that the access condition for an output production mechanism include the SPDX license identifier and the location of the license file in the repository or artifact, and that the license apply at the time of reporting, not only at the time of application. This is the same requirement NLnet enforces at successful project conclusion, expressed in CROSS's access condition vocabulary.

**Peaceful and humane use is an eligibility gate, not an obligation primitive.** CROSS does not currently encode peaceful-use clauses as a named primitive. The clause is best treated as an eligibility criterion in the program's round configuration: a published gate criterion that disqualifies proposals whose intended use is military, surveillance-state, or otherwise incompatible with the stated principle. CROSS Part IV permits funder-configured gate criteria of this kind through the external standard reference mechanism. A CROSS-conformant program that wishes to implement NLnet's peaceful-and-humane-use clause publishes it as a named eligibility criterion in the round configuration, with the conformance threshold specified clearly enough that an applicant can self-assess and reviewers can make a consistent determination.

**The dissemination commitment maps to a disclosure obligation declarable in the round configuration.** CROSS's coherence disclosure architecture allows a funder to require that grantees report on specific commitments at the completion gate. NLnet's dissemination commitment is suited to this mechanism: at the completion gate, the grantee documents the dissemination activities undertaken (publications, conference talks, community engagement, standards body participation, downstream adopter outreach) against the dissemination plan submitted at entry. The reporting is qualitative and narrative; the obligation is structural.

**The two-reviewer eligibility check is a reviewer infrastructure pattern, not an obligation primitive.** CROSS does not specify how reviewers are organized; Part I's format agnosticism principle explicitly permits any review infrastructure that satisfies the content requirements. NLnet's dual independent expert review, with a weighted-score threshold and a second-stage clarifying dialogue, is a conformant review infrastructure under CROSS. The structure is worth documenting as a reference pattern other funders can adopt, but it is not a CROSS primitive that needs to be invoked to describe NLnet's framework.

**The European Commission funding chain connects to existing CROSS+WALKRI EU coverage.** NLnet's grantmaking is downstream of Horizon Europe (and previously Horizon 2020) grant agreements. CROSS+WALKRI already covers Horizon Europe and the European Structural and Investment Funds at the framework level. A funder that has adopted CROSS+WALKRI for Horizon Europe compliance and operates a sub-granting program that mirrors NLnet's structure (a published applicant guide, dual independent review, open license and dissemination obligations) is structurally aligned across both layers: the prime contractor obligations under Horizon Europe and the sub-grantee obligations modeled on NLnet's framework can be expressed in a single CROSS-conformant round configuration.

| NLnet Framework Element | CROSS Mechanism |
|:--|:--|
| Open license requirement (software, hardware, scientific outcomes) | Public benefit mechanism declaration: output production with SPDX license identifier and license file location as access condition |
| Peaceful and humane use clause | Funder-configured eligibility criterion in round configuration with published conformance threshold |
| Free availability of project results | Access condition declaration paired with output production mechanism; license satisfies legal mechanism, repository or specification access satisfies practical mechanism |
| Dissemination commitment | Coherence disclosure obligation in round configuration; reported at completion gate against dissemination plan submitted at entry |
| Two-reviewer eligibility check with weighted scoring | Conformant review infrastructure under Part I format agnosticism; not a CROSS primitive |
| Disqualifying conditions (liquidation, enterprises in difficulty, EU funding exclusion) | Funder-configured eligibility criteria in round configuration |
| Project deliverables publicly available at conclusion | Build obligation completion verification gate: deliverable exists, meets completion criteria, is publicly accessible |
| European Commission NGI funding chain | Connects to existing CROSS+WALKRI Horizon Europe and ESIF coverage; sub-granting program structure expressible in a single CROSS-conformant round configuration |

---

## How WALKRI Complements This Alignment

WALKRI's contribution to NLnet's framework is in the specification of the intake fields through which the eligibility criteria are collected. NLnet's published guides describe the criteria clearly at the prose level, but the application form itself is the operational instrument that determines whether each criterion has been satisfied. A field asking "what license will your project use?" is not a license specification instrument unless it specifies what counts as a recognized free and open source license, what evidence the applicant must provide that the license will apply to the entire codebase (not only selected components), and what counts as satisfactory documentation of the license file's location. WALKRI's five pre-publication field requirements address each of these.

The license declaration field is a particularly clear case. Under WALKRI, the field collecting the applicant's license commitment must specify: criterion intent (the field measures whether the applicant has committed to a license that satisfies NLnet's open license requirement); operational definition (an enumerated list of accepted SPDX identifiers, with the boundary between accepted and non-accepted licenses stated); response form (single-select from the enumerated list, with a free-text field for licenses not on the list); evidence form (a link to the license file in the project repository or, for projects without a repository at the time of application, a statement of where the license file will be placed); and conformance threshold (the license must apply to the entire deliverable, not merely to selected components, and must be present at the time of completion gate submission). A WALKRI-conformant license field can be filled out by an applicant without ambiguity and can be assessed by a reviewer without interpretive latitude. NLnet's prose-level criteria become operational instruments at the form layer.

The peaceful and humane use field is harder to specify at the operational level. WALKRI's data quality standards require that the field be capable of detecting the magnitude of differences relevant to the criterion intent. A binary self-attestation ("I confirm that the project is for peaceful and humane purposes") has limited precision: it catches applicants who would refuse the attestation but does not distinguish between borderline cases. A WALKRI-conformant peaceful-use field might require the applicant to describe the intended use cases in sufficient operational detail that a reviewer can identify whether the project's primary use is consistent with the principle, with the field's conformance threshold specified as a named list of out-of-scope use categories (offensive military application, mass surveillance infrastructure, autonomous targeting systems) rather than a positive definition that would be impossible to bound. This is the form-layer instrument that operationalizes NLnet's prose-level clause.

The dissemination commitment field is the third case where WALKRI's specification rigor adds operational substance. A field asking "how will you disseminate the results of this project?" without specifying what counts as a dissemination activity, what evidence of dissemination is acceptable at the completion gate, and what minimum scope of dissemination the funder expects, is not a commitment instrument; it is a placeholder. WALKRI requires that the field's evidence form (the artifact that satisfies the criterion) and conformance threshold (the minimum standard the evidence must meet) be specified before the field is presented to applicants. This forces the funder to decide in advance what dissemination means in operational terms, which is the substance NLnet's prose-level clause leaves to per-grant negotiation.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
