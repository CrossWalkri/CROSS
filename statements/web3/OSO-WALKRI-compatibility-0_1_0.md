---
title: Open Source Observer Compatibility - CROSS+WALKRI
version: 0.1.2
date: 2026-06-08
license: CC0
standards: CROSS v0.4.0 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - OSO oss-directory YAML Schema v7 (github.com/opensource-observer/oss-directory)
  - OSO Documentation (docs.opensource.observer)
  - OSO Data Exchange (Google BigQuery, docs.oso.xyz/docs/integrate/)
lens_tags:
  calibration_tier: process_conformant
  authority_source: voluntary_published
  cultural_methodological_lineage: western_institutional
  funder_typology: dao_or_protocol
  framework_scope_type: third_party_rating
  # Open Source Observer impact-data platform serving DAO and protocol grantmaking; third_party_rating scope; alternative pooled_fund_or_intermediary funder typology
---

# Open Source Observer Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

Open Source Observer (OSO) and CROSS+WALKRI operate at adjacent layers of the grants accountability stack. OSO measures impact by aggregating on-chain activity, GitHub commit data, npm downloads, and other verifiable signals against registered project identities. CROSS+WALKRI governs the obligation architecture and field quality of grant programs. The two systems are designed to be used together: CROSS gates specify which OSO metrics count as evidence at each gate, WALKRI evidence form requirements specify the OSO artifact access paths that count as verification, and CROSS Field 6 (on-chain identity anchor) maps directly to OSO's blockchain address registration.

A project registered in both systems benefits from bidirectional reinforcement: the WALKRI recipient profile becomes OSO-importable, and the OSO project entry provides independent verification for the CROSS organizational identity declaration.

---

## What OSO Is

Open Source Observer (docs.opensource.observer) is an open-source impact measurement platform that tracks verifiable on-chain and off-chain signals for open source projects. OSO aggregates data from GitHub (commits, contributors, stars, forks), npm (package downloads), blockchain networks (transaction counts, contract deployments, on-chain activity), and other public sources, and makes the aggregated dataset available via Google BigQuery on the OSO Data Exchange.

Projects register in OSO by submitting a YAML file to the oss-directory repository. The oss-directory schema (v7) defines the required and optional fields for project registration. Once registered, a project's OSO metrics are computed continuously and are publicly queryable.

OSO is used by Optimism (as a data source for RetroPGF badgeholder evaluation), Gitcoin, Octant, and other grant programs as an independent verification source for impact claims. It is the primary public data infrastructure for verifiable open source project activity in the Web3 ecosystem.

---

## How CROSS Uses OSO Metrics

CROSS's gate architecture specifies what evidence must be produced at each payment gate. For Build obligation programs, the completion gate requires evidence that a specified artifact was delivered. For Change obligation programs, the milestone gate requires evidence that a measurable condition has shifted from baseline toward target.

OSO metrics are the natural evidence source for several common Build and Change obligation gate tests:

Build obligation completion gate evidence: "A publicly accessible, open-source codebase with commit activity in the 90 days prior to the gate date" maps directly to OSO GitHub commit data. An OSO-registered project provides this evidence structurally: the OSO query for a project's commit activity over a period is an independently verifiable, reproducible evidence artifact that does not rely on self-reporting.

Change obligation milestone gate evidence: "Increase in developer engagement measured as GitHub contributor count, from a documented baseline to a documented target" maps directly to OSO's contributor aggregation. The baseline is queryable from OSO at the time of grant application; the target is declared in the entry specification; the gate test queries OSO for the current value at the milestone date.

When a CROSS gate criterion references an OSO metric, the entry specification field should specify: the OSO metric name, the time window, the project slug used in OSO, and the access path (OSO Data Exchange query or OSO API endpoint). WALKRI's evidence form requirement governs how these specifications are written into the intake field.

---

## How WALKRI Maps to the OSO oss-directory Schema

The OSO oss-directory schema (v7) requires or supports the following fields for project registration:

| OSO oss-directory field | CROSS/WALKRI provision |
|:--|:--|
| name (unique project slug) | CROSS Field 1 organizational identity: legal or registered name provides the display_name; a slug is derived from it |
| display_name (globally unique) | CROSS Field 1: organizational name |
| github (list of GitHub org URLs) | WALKRI evidence form: GitHub repository URL is the artifact access path for code-related gate criteria |
| blockchain (list of addresses with network and tags) | CROSS Field 6: on-chain identity anchor (blockchain address, network, protocol, tag) |
| npm (list of npm packages) | WALKRI evidence form: npm package URL is the artifact access path for package delivery gate criteria |

CROSS Field 6 (on-chain identity anchor) is the primary structural alignment point. Field 6 records the grantee's verifiable on-chain identifier: the blockchain address, the network, and the protocol. These are exactly the fields that OSO's oss-directory blockchain section requires. A project that has completed CROSS organizational identity declaration (including Field 6) has already documented the information needed for OSO registration.

---

## Bidirectional Reference

A project registered in OSO and applying to a CROSS-conformant program benefits from bidirectional reference:

From OSO to CROSS: The CROSS Attestation Corpus query, which retrieves all prior CROSS declarations associated with a grantee's on-chain identity anchor, can cross-reference the grantee's OSO registration to confirm that the declared GitHub organization, npm packages, and blockchain addresses are consistent across both systems. Discrepancies are a flag for review; consistency is an independent verification of the organizational identity declaration.

From CROSS to OSO: A WALKRI-conformant recipient profile that includes the on-chain identity anchor, GitHub URL, and npm package identifiers is directly importable as an OSO oss-directory entry. Programs that run CROSS+WALKRI can generate OSO-compatible project registration YAML as a structural export of their conformant application data, reducing duplicate registration burden for grantees.

---

## OSO as a Funder-Side Verification Tool

OSO is most valuable to CROSS when used at the Attestation Corpus query stage. Before a funding decision is made, the funder queries OSO for the applicant's registered project metrics: commit activity, contributor count, on-chain transaction history, npm download trends. These are independent, reproducible signals that do not rely on the applicant's own reporting.

When a CROSS entry specification gate requires a baseline measurement, and the baseline draws from an OSO metric (commit count, contributor count, on-chain activity), the OSO query at application time is the baseline. The gate test at the completion or milestone date re-runs the same query and compares. This structure is free of self-reporting bias for any metric that OSO tracks.

---

*Published under CC0. For the current version of CROSS and WALKRI, see github.com/CrossWalkri.*

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-06-08 | Frame Language own-voice pass applied as part of the corpus-wide 2026-06-08 sweep: own-voice watchlist terms (govern-family, accountability, mandatory, compliance, enforce, legitimate) recast to conformance and obligation vocabulary where they appeared in this document's own voice; citation use of source-framework terms preserved. Primitive-rename references aligned to current canon (Continuity Capacity, the Collective disbursement state, Affected Population Verification Gate). Em-dash- and watchlist-clean re-verified. No compatibility finding or mapping changed; vocabulary only. |
| 0.1.1 | 2026-05-23 | Retroactive lens tagging: added calibration_tier, authority_source, cultural_methodological_lineage, funder_typology, framework_scope_type per Lenses Framework v0.1.0. |
