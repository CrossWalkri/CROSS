---
title: United Way Worldwide Global Results Framework Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.7 (github.com/CrossWalkri/WALKRI)
references:
  - https://www.unitedway.org/
  - https://clearimpact.com/solutions/united-way/global-results-framework/
  - https://clearimpact.com/rba-case-study-united-way-worldwide/
  - https://clearimpact.com/uww-global-results-framework-data-reporting-guide/
  - https://clearimpact.com/uww-global-results-framework-orientation/
  - https://clearimpact.com/scorecard/united-way-software/
  - https://www.unitedway.org/the-latest/press/uw-programs-helped-nearly-4k-children-enter-primary-school-ready-to-learn
  - https://equity.unitedway.org/equity-impact/overview
lens_tags:
  calibration_tier: outcome_specified_self_reported
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: pooled_fund_or_intermediary
  framework_scope_type: grantee_outcome_measurement
  # United Way Worldwide Global Results Framework; pooled_fund_or_intermediary captures the federated United Way network typology
---

# United Way Worldwide Global Results Framework

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

The United Way Worldwide Global Results Framework (GRF), formally published in 2015 and administered through the Clear Impact Scorecard platform, is a network-level aggregation framework: a core set of reach and outcome indicators across five impact areas (childhood success, youth success, economic mobility, access to health, and community engagement) that local United Ways report annually to United Way Worldwide so that the network can document its collective impact. The obligation relationship the GRF covers is the relationship between local United Way affiliates and the network as a whole, not the relationship between local United Ways and the nonprofits they fund. This distinction is decisive: the GRF is an affiliate-to-network reporting standard, and CROSS+WALKRI compatibility for it is meaningful precisely because affiliate-to-network reporting is itself a grants-and-membership obligation architecture where indicator pre-specification, evidence quality, and pre-commitment all apply. CROSS provides the gate architecture and indicator specification machinery the GRF requires to operate as a measurement framework rather than a survey instrument; WALKRI ensures that the indicator definitions local United Ways receive from the network are operational definitions, not labeled containers.

---

## The United Way Global Results Framework's Approach

United Way operates as a federated network: United Way Worldwide is the umbrella organization, and the network consists of roughly 1,100 local United Ways in the United States and approximately 1,800 affiliates globally. Each local United Way is a separately incorporated nonprofit organization with its own board, fundraising operation, and grantmaking program serving its defined geographic community. Local United Ways raise funds through workplace campaigns and other sources and re-grant those funds to local nonprofits delivering services in the affiliate's community. The relationship between United Way Worldwide and the local affiliates is a network membership relationship: affiliates pay dues, use the United Way brand under licensing terms, and report participation data to the network.

The Global Results Framework, developed in 2015, addresses a specific reporting-obligation problem this federated structure produces: while each local United Way can describe its own community impact, the network as a whole has historically had no shared instrument for documenting what United Way collectively delivers across communities. Donors, corporate partners, and the public encountered United Way as a national brand without seeing aggregated evidence of what funding through that brand produces. The GRF was designed to fill this gap by establishing a limited core set of indicators that local affiliates report to the network annually, so that United Way Worldwide can publish aggregate figures showing the network's collective contribution to its five impact areas.

The framework defines five impact areas. Childhood success addresses school readiness, early literacy, and kindergarten preparation for children below school age. Youth success addresses academic achievement, school engagement, and high school graduation outcomes for school-age youth. Economic mobility addresses workforce readiness, employment, income stability, and financial capability for working-age adults. Access to health addresses health insurance enrollment, preventive care access, and behavioral health outcomes. Community engagement addresses volunteering, civic participation, and collective action across the population. Each impact area is anchored by a small set of core indicators with defined measurement protocols. The initial draft contained more than eighty measures and was reduced substantially before publication, on the recognition that a reportable network-wide indicator set must be small enough that every affiliate can actually report against it. The reduced set is the published GRF.

The framework is administered through the Clear Impact Scorecard platform, the same Results-Based Accountability (RBA) software environment used by RBA-aligned public and nonprofit measurement programs. The GRF Data Reporting Platform is the United Way Worldwide deployment of Clear Impact Scorecard. Local United Ways enter their annual outcome data into the platform against the GRF indicator definitions, and United Way Worldwide aggregates the data into network-level figures. The Clear Impact administration choice anchors the GRF in the RBA tradition: the quantity, quality, and effect metric structure that defines RBA is the structural model for how each GRF indicator is operationalized at the local affiliate level, even when the network-level aggregation focuses on quantity totals.

**What the GRF does not cover.** The GRF does not specify requirements imposed on the nonprofits that local United Ways fund. A nonprofit that receives a grant from a local United Way is not obligated by the GRF; its reporting obligation is to the local affiliate, subject to that affiliate's grant agreement and program design. The GRF covers only the data the local affiliate then reports up to United Way Worldwide. This is why the gap map documents the GRF as not a grantee-facing MEL standard. It is a network-level reporting standard. CROSS+WALKRI compatibility for the GRF is meaningful at the layer it actually covers: the affiliate-to-network reporting architecture. A local United Way's grantmaking to local nonprofits is a separate obligation architecture that may, independently, adopt CROSS+WALKRI for its grant programs, and the two adoptions are coherent: outcomes a CROSS-conformant local grant program generates can be reported up through a GRF-conformant network channel without conflict.

---

## How CROSS Satisfies the Global Results Framework

CROSS provides the gate architecture, indicator specification structure, and obligation mode classification that the GRF requires to operate as a measurement framework rather than a survey instrument.

The GRF's network-level indicator catalogue corresponds to CROSS's eleven-field indicator specification applied at the network level rather than at the individual round level. The five impact areas function as program-level Theory of Change pathways, each with a defined population (children below school age, school-age youth, working-age adults, the general population for health access, the population for civic engagement) and a defined condition the network is contributing to change. Each core indicator within an impact area is the operational expression of the pathway. CROSS Fields 1 through 11 (indicator name, definition, unit, baseline, target, timing, data source, collection method, comparison group, causality stance, evidence threshold) provide the full specification an indicator catalogue needs to function as a measurement instrument, and the GRF's existing indicator definitions (developed for Clear Impact Scorecard administration) supply most of these fields already. CROSS's contribution at this layer is to make the unspecified fields explicit and to provide a portable schema in which the indicator catalogue can be expressed independent of any single administration platform.

The affiliate-to-network reporting relationship maps to CROSS's continuation gate architecture configured at the program level rather than the round level. The annual GRF reporting cycle is structurally a continuation gate: it is the gate at which local United Ways demonstrate to the network the outcomes attributable to their participation in the network's collective work for the period just completed, and the network determines whether the affiliate's participation continues in good standing. CROSS's continuation gate specification (Part IV) requires that gate criteria be published before the period it covers begins, that evidence scope and strength be declared, and that the determination be documented against pre-committed criteria. The Clear Impact Scorecard administration provides the documentation infrastructure; CROSS provides the structural specification of what the gate must require.

The five impact areas map to CROSS's coherence disclosure and Portfolio Position primitive at the network level. United Way Worldwide's coherence disclosure declares which population conditions the network as a whole is contributing to and how the five impact areas collectively constitute the network's theory of change. Each local United Way's annual GRF submission is a portfolio contribution statement: how the affiliate's local grantmaking and direct service work contributed to each impact area's network-level totals. CROSS's Portfolio Position primitive distinguishes initiating, continuation, and convergence contributions, and the GRF aggregation logic is a convergence operation: many independent affiliates contributing to shared indicators that aggregate into a single network-level figure. CROSS makes this convergence structure explicit and provides the language for distinguishing what an affiliate originates from what an affiliate contributes to an aggregate.

The RBA lineage of the GRF (administered through Clear Impact Scorecard, structured around RBA's quantity, quality, and effect metric system) is already addressed in the published Annie E. Casey Foundation RBA compatibility statement: CROSS's Build and Change obligation modes map to RBA's quantity, quality, and effect metric structure. For the GRF specifically, the network-level aggregation emphasizes quantity totals (how many children entered school ready to learn, how many youth graduated, how many adults achieved employment milestones), but the underlying affiliate-level reporting captures quality and effect through the RBA program structure beneath each aggregated count. CROSS accommodates this by allowing different gate types to operate at different layers of the program structure: quantity at the network aggregation layer, quality and effect at the affiliate program layer.

The annual reporting cadence maps to CROSS's pre-commitment record requirement at the program level. Each GRF reporting cycle is anchored to indicator definitions published before the year begins. Affiliates know what they will be asked to report on at the start of the year, not at the end. This is the network-level analogue of the round-level pre-commitment requirement in CROSS Part IV: the structural form of the obligation is the same, and the verifiable record that criteria existed before reporting began is the same.

| GRF Requirement | CROSS Provision |
|---|---|
| Five-impact-area indicator catalogue | Eleven-field indicator specification at network program level |
| Affiliate-to-network annual reporting | Continuation gate configured at program level |
| Network-level aggregate impact claim | Coherence disclosure + Portfolio Position convergence classification |
| RBA quantity/quality/effect structure (Clear Impact administration) | Build and Change obligation modes (mapping detailed in AECF RBA compatibility statement) |
| Pre-published indicator definitions | Pre-commitment record at program level (Part IV) |
| Federated network with local autonomy | Format agnosticism (Part I): affiliate program design is local; reporting interface is network-specified |

---

## How WALKRI Complements This Alignment

WALKRI ensures that the indicator definitions United Way Worldwide publishes to its affiliate network are operational definitions rather than labeled containers. A network-wide indicator such as "number of children entering kindergarten ready to learn" is reportable only if every local United Way is operating from the same definition of "ready to learn," the same eligible age range, the same assessment instrument or proxy, and the same evidence threshold. Without operational definition at the network level, the aggregation produces a sum of differently-measured quantities that cannot be meaningfully reported as a single figure. WALKRI's five pre-publication field requirements (criterion intent, operational definition, response form, evidence form, conformance threshold) apply to every GRF indicator definition before the reporting cycle opens.

The network aggregation problem WALKRI specifically addresses is the inter-affiliate reliability question. When 1,100 US affiliates report against the same indicator, the reliability of the aggregate figure depends on whether all 1,100 affiliates applied the same operational definition. WALKRI's operational definition requirement is the structural condition under which the aggregate is interpretable. A figure such as "United Way programs helped nearly 400,000 children enter primary school ready to learn" carries meaning only to the extent that the affiliates contributing to that 400,000 were measuring the same condition. WALKRI does not impose this requirement on local affiliate program design (which remains the affiliate's authority); it imposes it on the network-level indicator definitions the affiliates report against.

WALKRI also addresses a structural risk specific to federated reporting networks: the temptation to keep indicator definitions broad enough that every affiliate can report against them, at the cost of operational specificity. The GRF reduced its initial catalogue from more than eighty indicators to a small core set precisely because broader catalogues exceeded affiliate reporting capacity. WALKRI's conformance threshold requirement asks the opposite question of the reduced set: now that the catalogue is small enough to be reportable, are the definitions tight enough that the reports mean what the network claims they mean? A network that publishes its operational definitions, evidence forms, and conformance thresholds for each GRF indicator has done the work to make its aggregate figures defensible to external scrutiny; a network that publishes only indicator names and impact-area assignments has not.

For the United Way Equity Framework, which sits alongside the GRF and articulates equity-focused programmatic strategy across the network, WALKRI's criterion intent requirement applies to any GRF indicator that is intended to surface equity outcomes. An indicator that aggregates children entering school ready to learn without disaggregation by population subgroups does not function as an equity indicator regardless of the rhetorical framing around it. WALKRI's response form requirement addresses this directly: the disaggregation categories must be specified at the indicator level before the reporting cycle opens, not requested after the aggregate figure has been computed.

---

## Notes on the Affiliate-Grantee Distinction

The obligation layer the GRF covers is worth restating because it is the source of the framework's placement in the coverage gap map and the reason CROSS+WALKRI compatibility is meaningful at the network-reporting layer specifically.

A local United Way is itself a grantmaker. It receives donations through its annual campaigns and other channels, and it disburses funds through grants to nonprofits delivering services in its community. The grant agreements between local United Ways and the nonprofits they fund are subject to each affiliate's own grant policy, reporting requirements, and evaluation methodology. The GRF does not standardize these grant agreements; United Way Worldwide does not require local affiliates to impose any specific evaluation framework on their grantees, and most local United Ways adopt grant evaluation practices reflecting their own community context, donor expectations, and capacity. Some local United Ways use the Clear Impact Scorecard tools for their grantee reporting, which produces alignment between affiliate-level and network-level reporting structures, but this is a local affiliate choice rather than a network requirement.

The GRF's reporting requirement runs in the other direction: from the local affiliate to United Way Worldwide. The local affiliate aggregates outcome data from its own programs, including outcomes reported by its grantees, and reports the aggregated outcomes against the GRF's core indicators to United Way Worldwide annually. The reporting obligation the GRF creates runs from the affiliate to the network: a local United Way that uses the United Way brand, pays network dues, and benefits from network-level fundraising and public relations is answerable for participating in the network's collective impact documentation. The grantees the affiliate funds locally are not parties to this obligation relationship.

This is the layer at which CROSS+WALKRI compatibility is structurally appropriate. The GRF is, in CROSS terminology, a program-level standard covering the reporting obligation between a federation member and the federation as a whole. CROSS's program-level continuation gate architecture, indicator specification framework, and coherence disclosure mechanism are designed exactly for this layer. A local United Way's grantmaking program to local nonprofits is a separate program that may independently adopt CROSS+WALKRI; the two adoptions can coexist coherently, and a local United Way running CROSS-conformant grantmaking would produce affiliate-level outcome data that flows naturally into GRF-conformant network reporting without translation loss.

The federated structure also has implications for Part XI of CROSS, which specifies funder obligations and redress mechanisms. In the GRF context, the obligations of the "funder" are United Way Worldwide's obligations to its affiliates: to publish indicator definitions before the reporting cycle, to operate the Clear Impact Scorecard infrastructure reliably, to aggregate data accurately, and to not impose retroactive requirements that affiliates could not have anticipated. CROSS's Part XI obligations on funders translate directly into network obligations on the federation center, providing the redress architecture that participating affiliates can invoke if the network changes the reporting requirements mid-cycle.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
