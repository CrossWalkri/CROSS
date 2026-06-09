---
title: Research Performance Progress Report (RPPR) Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - https://www.nsf.gov/bfa/dias/policy/research-performance-progress-reports
  - https://grants.nih.gov/grants-process/post-award-monitoring-and-reporting/reporting-requirements/research-performance-progress-report-rppr
  - https://grants.nih.gov/sites/default/files/rppr_instruction_guide.pdf
  - https://www.era.nih.gov/about-era/services-for-applicants-recipients/reporting-requirements/overview-rppr.htm
  - https://www.govinfo.gov/content/pkg/FR-2010-01-13/html/2010-469.htm
  - https://www.ars.usda.gov/ARSUserFiles/FMAD/Agreements/rppr-final-format.pdf
  - https://www.ecfr.gov/current/title-2/subtitle-A/chapter-II/part-200
lens_tags:
  calibration_tier: outcome_specified_self_reported
  authority_source: regulatory
  cultural_methodological_lineage: western_institutional
  funder_typology: government_non_aid
  framework_scope_type: grantee_outcome_measurement
  # Federal Research Performance Progress Report under Federal Demonstration Partnership; regulatory framework adopted by federal research agencies
---

# Research Performance Progress Report (RPPR)

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The Research Performance Progress Report (RPPR) is the US federal government-wide standard format for interim and final performance reporting on federally funded research and research-related activities. It was developed by the Research Business Models (RBM) Subcommittee of the Committee on Science of the National Science and Technology Council, published in final form by OMB and OSTP in January 2010, and adopted across the major federal research funders, including NIH, NSF, NASA, USDA NIFA, AHRQ, ARPA-E, CDC, and the Department of Veterans Affairs Office of Research and Development. A CROSS+WALKRI conformant program operating under any RPPR-using funder satisfies the structural reporting requirements of the seven RPPR content components as a consequence of conformance. CROSS's gate architecture produces the timestamped, audit-ready Attestation Corpus that the RPPR's reporting cadence assumes; WALKRI's pre-publication field specification produces the operational definitions, evidence forms, and external standard references that the RPPR sections require grantees to supply year after year.

---

## The Standard

The RPPR is a uniform format, not a single submission portal. It standardizes what federal research grantees must report; each funding agency operates its own submission system against the same content specification. NIH submissions flow through eRA Commons. NSF submissions flow through Research.gov. NASA submissions flow through NSPIRES. USDA NIFA submissions flow through REEport. AHRQ uses the NIH grants infrastructure (eRA Commons). The Federal Demonstration Partnership piloted the RPPR before its general rollout and continues to maintain alignment across agency implementations.

The RPPR operates downstream of OMB's Uniform Guidance (2 CFR Part 200), which covers financial-obligation reporting and audit obligations for all federal awards regardless of funding agency. The RPPR is the research-grant-specific performance reporting layer on top of 2 CFR 200's broader financial framework. A federal research grantee operates under both simultaneously: 2 CFR 200 determines whether the organization's finances are managed lawfully and can withstand independent audit; the RPPR determines whether the research has progressed against its declared scope and produced the outputs, participants, and impact that justify continuation. A separate CROSS+WALKRI compatibility statement covers 2 CFR 200; this statement covers the research-performance reporting layer.

**The seven content components.** Beyond the cover page, the RPPR consists of seven standard sections.

**Section B (Accomplishments).** What were the major goals of the project, what was accomplished under those goals, what opportunities for training and professional development did the project provide, how were the results disseminated to communities of interest, and what do you plan to do during the next reporting period.

**Section C (Products).** Publications, conference papers, books, websites, technologies or techniques, inventions, patent applications, licenses, and other products generated under the award.

**Section D (Participants and Other Collaborating Organizations).** Personnel who worked on the project, the role each played, the calendar months committed, partner organizations, and other collaborators.

**Section E (Impact).** Impact on the development of the principal discipline, on other disciplines, on the development of human resources, on physical resources that form research infrastructure, on institutional resources that form research infrastructure, on information resources, on technology transfer, and on society beyond science and technology.

**Section F (Changes/Problems).** Changes in approach and reasons, actual or anticipated problems or delays and actions to resolve them, changes that have a significant impact on expenditures, significant changes in use or care of human subjects, vertebrate animals, or biohazards, and changes that have a significant impact on biohazards or select agents.

**Section G (Special Reporting Requirements).** Responsible conduct of research training, organizational duplication of effort, plans to address unobligated balance, project outcomes for the public (in final RPPRs).

**Section H (Budgetary Information).** Detailed expenditure information by category, present only in annual RPPRs; not present in Interim RPPRs or Final RPPRs.

**Cadence.** Annual RPPRs are due each year of a multi-year award, typically 45 to 60 days before the next budget period begins; the specific window varies by agency and grant mechanism. Interim RPPRs are submitted at the end of a competitive segment when a renewal application has been filed but a funding decision is not yet final; the Interim RPPR converts to the Final RPPR if the renewal is not funded and to the final-year annual RPPR if the renewal is funded. Final RPPRs are submitted when an award terminates and no renewal is pending; they include cumulative Project Outcomes content for public release through agency reporting systems such as NIH RePORTER.

---

## How CROSS Satisfies the RPPR

The RPPR is, structurally, a recurring evidence submission against a fixed content template. Each annual submission asks the grantee to demonstrate what was accomplished, what was produced, who participated, what impact occurred, what changed from plan, and what reporting obligations were addressed. This is a gate architecture in everything but name: the funder reviews the submission against the published template, makes a determination, and conditions continued funding on that determination.

CROSS's gate architecture maps directly onto the RPPR's reporting cadence.

| RPPR Requirement | CROSS Provision |
|:--|:--|
| Annual interim performance reporting against project goals | Progress verification gate: configured at the annual cadence, with the indicator specification from the entry gate carried forward as the obligation being measured |
| Final cumulative reporting at award termination | Completion verification gate: documented funder determination against published completion criteria, with output and outcome evidence at the strength level the funder configured |
| Renewal/continuation reporting (Interim RPPR convertible to Final or annual) | Continuation specification gate: program-level gate that determines progression between stages or rounds; supports the Interim RPPR's dual role as renewal evidence and closeout evidence |
| Section B: accomplishments against major goals | Indicator specification at entry gate (eleven-field specification under Part V) carried forward into annual gate evidence; outcome evidence under Part IV |
| Section C: products (publications, software, datasets, inventions) | Output evidence under Part IV; the Attestation Corpus retains publicly linkable artifacts for each reporting period |
| Section D: participants and collaborating organizations | Organizational identity declaration and affiliated entity disclosure under Part IV, refreshed at each progress gate; the disbursement authority field captures personnel with award control |
| Section E: impact | Public benefit mechanism declaration carried forward; for change-obligation rounds, outcome evidence against the declared FROM-TO state; for build-obligation rounds, usage evidence from parties outside the applicant's control |
| Section F: changes/problems | Unintended outcomes disclosure at each progress gate; adverse signal engagement applies to discovered changes that were not specified at entry |
| Section G: special reporting requirements (responsible conduct of research, unobligated balance, project outcomes for public release) | Coherence disclosure obligations configured in the round configuration; final completion gate submission includes public-release outcome statement |
| Section H: budgetary information (annual only) | Out of CROSS scope; covered by 2 CFR 200 compatibility (Part XII), which covers financial-obligation reporting for the same award |

The mapping is structural rather than procedural. A CROSS-conformant grantee preparing an RPPR submission draws each section's content from gate records that already exist in the Attestation Corpus: the entry gate produced the goals (Section B opening), the progress verification gates produced the accomplishments and unintended outcomes record (Sections B, E, and F), the organizational identity declaration produced the participants list (Section D), and the public benefit mechanism declaration produced the impact framing (Section E). The RPPR submission is the export, not a new construction.

**The annual cadence.** RPPR's annual reporting requirement aligns directly with the progress verification gate. A CROSS-conformant program operating under a federal research funder configures progress gates at the annual cadence that the RPPR requires. Each progress gate produces the evidence record that the corresponding annual RPPR submission documents. Where the funder's annual reporting window precedes the next budget period by 45 to 60 days, the progress gate is positioned in that window.

**Final RPPR and the completion gate.** The Final RPPR's cumulative scope, including the public-release Project Outcomes section, aligns with the completion verification gate's summative character (Part IV: gate function distinction between developmental progress gates and summative completion gates). The completion gate's documented determination, retained in the Attestation Corpus, is the audit-ready record that supports the Final RPPR's claims and remains queryable after the award terminates.

**Interim RPPR and the continuation gate.** The Interim RPPR's dual role, serving either as renewal-cycle evidence or as Final RPPR depending on the renewal outcome, aligns with the continuation specification gate's role of determining progression between stages or rounds. A CROSS-conformant program that operates multi-year research awards configures the continuation gate at the segment boundary; the gate's published criteria are the basis on which the Interim RPPR's evidence is assessed.

---

## How WALKRI Complements This Alignment

WALKRI operates at the field specification layer, before any applicant submits data. Its relevance to RPPR concentrates in the operational definitions that each section requires.

**Section B accomplishments require operational definitions.** What counts as a major goal accomplishment? What counts as a training opportunity? What counts as dissemination to a community of interest? An RPPR field that asks "what was accomplished" without operational definition produces narrative text that cannot be aggregated across grants or compared across years within the same award. WALKRI's operational definition requirement, applied at the entry gate when the program defines its accomplishment categories, forces the program operator to specify what counts as one instance of each category before the grantee writes the first annual RPPR. The resulting accomplishments section is structurally consistent across reporting years and across grantees in the same program.

**Section C products require evidence forms.** Publications need persistent identifiers (DOIs, PubMed IDs). Software needs repository URLs and license declarations. Datasets need repository deposits and access paths. WALKRI's evidence form requirement specifies, for each product type the program tracks, what artifact counts as evidence and what access path retrieves it. A WALKRI-conformant program collecting product information at the entry gate has defined these evidence forms before any grantee files an RPPR; the grantee fills in the evidence locations rather than negotiating with reviewers about what counts.

**Section D participants require external standard references.** Personnel records map onto ORCID identifiers; collaborating organizations map onto ROR (Research Organization Registry) identifiers; the discipline classifications used in some Section E impact reporting map onto agency-specific taxonomies. WALKRI's conformance threshold field is the correct place to bind these external standards to gate criteria. A program that declares ORCID as the personnel identifier and ROR as the organizational identifier at the entry gate produces RPPR Section D content that interoperates with federal personnel and organization databases.

**Section E impact requires causality stance specification.** RPPR Section E asks the grantee to characterize impact across multiple dimensions: discipline, human resources, infrastructure, technology transfer, and society beyond science and technology. Without an explicit causality stance, impact claims default to attribution language that the underlying evidence cannot support. CROSS's causality stance field (Part V) and the eleven-field indicator specification, applied through WALKRI's pre-publication audit, produce Section E content that distinguishes contribution claims (the funded work participated in a broader effort that produced the change) from attribution claims (the funded work caused the change), with the evidence appropriate to each.

**Section F changes/problems require unintended outcomes disclosure infrastructure.** The Adverse-Signal Engagement Principle that CROSS incorporates by reference (Part I) determines how Section F is treated structurally: changes and problems are disclosed, not concealed, and disclosed adverse outcomes are documented as features of the record rather than as evidence to be suppressed. WALKRI's evidence form requirement, applied to the Section F unintended outcomes disclosure, produces a structured change record rather than a free-text narrative.

---

## Framework-Specific Considerations

**NIH.** NIH RPPR submission flows through eRA Commons. NIH's data management policy (covered by the Research Funder DMP Standards compatibility statement) interacts with the RPPR through Section C products and Section G special reporting requirements: data management commitments declared at application are reported on annually through these sections. A CROSS+WALKRI conformant NIH-funded program carries the DMS Plan content into the RPPR sections without separate authorship.

**NSF.** NSF RPPR submission flows through Research.gov. NSF directorate-specific reporting requirements may add fields beyond the base RPPR; these are recorded in WALKRI's conformance threshold field as program-specific external standards.

**NASA.** NASA GCAM (Grant and Cooperative Agreement Manual) anchors to the government-wide RPPR for performance reporting. NASA submissions flow through NSPIRES. A CROSS+WALKRI conformant program operating under a NASA award satisfies the NASA-specific performance reporting requirements through the same gate architecture that satisfies the RPPR.

**USDA NIFA.** USDA NIFA operates REEport as its submission system; the underlying content standard is the RPPR. NIFA-specific extensions, including the formula funds reporting and capacity-grant requirements, are program-specific overlays on the RPPR base format. A CROSS+WALKRI conformant NIFA program records the NIFA-specific requirements in WALKRI's conformance threshold field; the base RPPR content is produced as a structural consequence of conformance.

**AHRQ.** AHRQ uses the NIH eRA Commons infrastructure (eRA Commons, the RPPR module, Federal Financial Report). The same CROSS+WALKRI conformance that satisfies NIH RPPR obligations satisfies AHRQ obligations.

**ARPA-E.** ARPA-E's ePIC reporting system operates on RPPR-derived content. A CROSS+WALKRI conformant ARPA-E grantee produces the RPPR-aligned content as a structural byproduct, then maps it to ePIC's submission interface.

**Other PHS agencies (CDC, FDA, HRSA, IHS, SAMHSA).** All Public Health Service agencies that issue research grants use the RPPR for performance reporting; submission infrastructure varies. The CROSS+WALKRI mapping above applies regardless of submission portal.

**Department of Veterans Affairs Office of Research and Development.** VA-ORD uses the RPPR through its own submission portal. The content alignment is the same.

---

## Scope

This statement covers CROSS and WALKRI's contribution to the seven RPPR content components: accomplishments (Section B), products (Section C), participants and collaborating organizations (Section D), impact (Section E), changes/problems (Section F), special reporting requirements (Section G), and budgetary information (Section H). Section H is partially out of scope: financial expenditure detail is covered by the 2 CFR 200 compatibility statement, which addresses the underlying financial-obligation reporting framework. Agency-specific extensions to the base RPPR (NIH program-specific instructions, NSF directorate-specific addenda, NASA GCAM extensions, NIFA capacity-grant overlays) remain agency-specific obligations on the grantee; CROSS+WALKRI conformance does not displace those obligations, but it produces the structural record from which the agency-specific extensions can be derived.

This statement also covers the cadence alignment: annual RPPRs map to progress verification gates, Final RPPRs map to completion verification gates, and Interim RPPRs map to continuation specification gates.

---

## Gap-Map Rows Anchored by This Statement

Because the RPPR is the government-wide research performance reporting standard, several agency-specific gap-map rows reference it as their underlying or anchoring standard. The following rows should be updated to point at this RPPR compatibility statement as the structural anchor; each retains its agency-specific content beyond the RPPR base.

- **NASA GCAM (Grant and Cooperative Agreement Manual).** GCAM anchors to the government-wide RPPR for performance reporting. Update to reference this statement as the anchor; retain NASA-specific GCAM content (NSPIRES submission, NASA-specific cost principles, NASA technology transfer provisions).
- **AHRQ.** AHRQ uses the NIH grants infrastructure (eRA Commons, RPPR, FFR). Update to reference this statement and the 2 CFR 200 statement as the structural anchors; retain AHRQ-specific programmatic content (health services research scope, AHRQ-specific data standards).
- **USDA NIFA REEport.** The broader REEport/RPPR system is a government-wide standard. Update to reference this statement as the underlying content standard; retain NIFA-specific overlays (formula funds reporting, capacity-grant reporting, agricultural research priorities).
- **ARPA-E ePIC.** ePIC is RPPR-derivative. Update to reference this statement as the underlying content standard; retain ARPA-E-specific programmatic content (energy research focus, ARPA-E milestone structure, technology-to-market provisions).

These are updates, not removals. Each agency-specific row retains its own programmatic, mechanism-specific, and submission-portal content; the RPPR statement provides the structural reporting backbone that those agency frameworks share.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
