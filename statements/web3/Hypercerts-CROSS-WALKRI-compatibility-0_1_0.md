---
title: Hypercerts Compatibility - CROSS+WALKRI
version: 0.1.0
date: 2026-05-16
license: CC0
standards: CROSS v0.3.7 (github.com/CrossWalkri/CROSS), WALKRI v0.1.6 (github.com/CrossWalkri/WALKRI)
references:
  - Hypercerts ERC-1155 Standard (hypercerts.org)
  - Hypercerts Metadata Schema (github.com/hypercerts-org/hypercerts)
  - ERC-1155 Multi-Token Standard
---

# Hypercerts Compatibility

## CROSS+WALKRI Compatibility Statement v0.1.0

---

## Summary

CROSS and Hypercerts address adjacent and complementary problems in impact accountability: CROSS specifies the obligation architecture that governs what funded interventions must demonstrate and at which gate; Hypercerts provides the on-chain token mechanism for representing and attributing past impact contributions. Together they close the loop between prospective obligation and retrospective verification.

CROSS's retroactive obligation mode is the most natural integration point, but the compatibility extends to all three modes. A CROSS completion gate attestation can reference a Hypercert as its primary evidence artifact; a Hypercert's impact scope metadata can be populated from CROSS's indicator specification to produce a more structured and auditable impact claim than the Hypercert standard alone specifies.

---

## What Hypercerts Are

Hypercerts (hypercerts.org) is an ERC-1155 multi-token standard for impact certificates. It was developed by Protocol Labs and the Funding the Commons community as infrastructure for impact markets and retroactive public goods funding. A Hypercert is an on-chain token representing a claim that a specific contribution was made toward a specific impact during a specific time period.

The Hypercerts metadata schema specifies four primary fields:

**Work scope**: what work was performed. A set of tags describing the activity or project.

**Impact scope**: what change in the world the work contributed to. A set of tags describing the impact domain.

**Work timeframe**: when the work was performed. Start and end dates.

**Contributors**: who performed the work. A list of wallet addresses or ENS names.

Hypercerts can be minted by the contributors themselves (self-certification) or by a third party. Fractions of a Hypercert can be distributed to acknowledge partial contributions from multiple parties. Hypercerts can be traded or retired; retroactive funding mechanisms often retire Hypercerts as part of the funding transaction, preventing double-counting.

---

## The Compatibility Gap Hypercerts Does Not Address

Hypercerts are expressive but underspecified at the impact claim level. The work scope and impact scope fields accept freeform tags. Two projects contributing to "clean water access" in "East Africa" produce Hypercerts with the same tags but potentially with entirely different baselines, measurement methodologies, populations, and causal arguments. The tags are labels; they are not instruments.

This is precisely the gap CROSS and WALKRI address. CROSS's indicator specification (11 fields) and WALKRI's criterion specification requirements (5 elements) transform the Hypercert's freeform impact scope into a structured, auditable, comparable impact claim. A Hypercert whose work scope and impact scope are populated from CROSS+WALKRI-conformant data is not merely a claim of contribution; it is an obligation-architecture-backed claim with a documented baseline, a specified methodology, and gate evidence attached.

---

## CROSS Mapping to Hypercerts

### Metadata Mapping

| Hypercerts Field | CROSS Equivalent | Notes |
| :-- | :-- | :-- |
| Work scope (tags) | Obligation mode + entry specification deliverable (build) or FROM state (change) | CROSS's entry specification is the structured form of the Hypercert's work scope. For build-obligation grants, the work scope is the deliverable specification. For change-obligation grants, the work scope is the intervention described in the entry specification. |
| Impact scope (tags) | TO state (target condition) + indicator name + domain tags | CROSS's TO state is the structured form of the Hypercert's impact scope. The indicator name provides the specific claim; the domain tags provide the thematic context. |
| Work timeframe (start/end) | Gate dates (entry gate to completion gate) | The Hypercert's work timeframe is bounded by the CROSS entry gate date and the completion verification gate date. |
| Contributors | Legal entity from organizational identity declaration | The Hypercert's contributors field maps to the applying entity's legal name and, where applicable, contributor wallet addresses. |
| (not in Hypercerts) | FROM state (baseline) | Hypercerts do not specify a baseline for the impact claim. CROSS's FROM state provides the structured baseline that makes the impact scope meaningful. |
| (not in Hypercerts) | 11-field indicator specification | Hypercerts have no indicator specification. CROSS's indicator fields provide the measurement methodology that the Hypercert's impact scope tags imply but do not specify. |
| (not in Hypercerts) | Gate evidence (completion attestation) | Hypercerts have no evidence attachment requirement. CROSS's completion gate evidence is the structured documentation of what the Hypercert claims. |
| (not in Hypercerts) | Causality stance | Hypercerts make no distinction between attribution and contribution claims. CROSS's causality stance primitive (attribution vs. contribution) makes this explicit. |

---

## Integration Patterns

### Pattern 1: CROSS Completion Gate Anchored to a Hypercert

The most direct integration. When a grantee completes a CROSS change-obligation or build-obligation grant, the completion verification gate produces a signed attestation. This attestation can reference a Hypercert minted by the grantee as the primary evidence artifact.

The integration works as follows:

1. The grantee mints a Hypercert at or near the completion gate, populating the work scope and impact scope from their CROSS entry specification (FROM state, TO state, deliverable specification).
2. The Hypercert token ID is included in the completion gate evidence submission as a verifiable on-chain reference.
3. The CROSS completion gate attestation references the Hypercert token ID and the chain on which it was minted. The format of this gate attestation (W3C Verifiable Credential, EAS attestation, DAOIP-3 VC for DAOIP ecosystem programs, signed document, or comparable mechanism) is determined by the program's infrastructure.
4. The funder's completion gate determination is recorded as a separate signed attestation referencing both the grantee's submission and the Hypercert.

This produces a chain of attestation: Hypercert (grantee's impact claim) + completion gate evidence + funder determination. Each link in the chain is independently verifiable, either on-chain or via the structured gate record mechanism the program uses.

### Pattern 2: Hypercerts as Retroactive Obligation Evidence

CROSS's retroactive obligation mode funds past contributions. The natural evidence artifact for a retroactive claim is a Hypercert minted to represent that past contribution.

For retroactive-obligation CROSS rounds, funders can configure the entry gate to require a Hypercert reference as the primary evidence artifact. The Hypercert's work timeframe, work scope, and impact scope are assessed against the program's published retroactive criteria. The 11-field CROSS indicator specification provides the structured metadata required to assess the Hypercert's impact claim against a documented baseline and methodology.

This pattern enables programs like Optimism RetroPGF, Gitcoin Retroactive, and comparable retroactive mechanisms to operate under CROSS's retroactive obligation mode while using Hypercerts as their native evidence format.

### Pattern 3: Hypercert Impact Scope Enriched with CROSS Metadata

For programs that mint Hypercerts as their primary accountability artifact, CROSS+WALKRI provide the indicator specification layer that makes the Hypercert's impact scope claim auditable.

The Hypercert's work scope and impact scope tag fields can reference CROSS indicator IDs and WALKRI field specification versions, enabling data consumers to retrieve the full specification metadata from the CROSS+WALKRI-conformant program's published round configuration. This transforms freeform impact scope tags into structured references to documented measurement methodologies.

---

## Structured Gate Records and Hypercerts: Complementary Accountability Layers

Hypercerts and CROSS gate attestation records are complementary mechanisms serving different functions:

**Hypercerts** represent impact claims as transferable, fractional on-chain tokens. They are designed for impact markets, retroactive funding, and contribution attribution. They do not carry structured specification metadata by design; their value is in their transferability and on-chain verifiability.

**CROSS gate attestation records** are signed, structured accountability records carrying the obligation metadata (indicator specification, gate evidence, funder determination) that Hypercerts cannot. These records may be expressed in any verifiable format appropriate to the program's infrastructure: W3C Verifiable Credentials, EAS attestations, DAOIP-3 VCs for programs operating within the DAOIP ecosystem, signed institutional documents, or comparable mechanisms.

A CROSS+WALKRI-conformant program produces both: structured gate records for the accountability layer and Hypercerts as the on-chain representation of the same contribution where Hypercerts are used. Neither layer replaces the other; they address different consumer needs. Retroactive funding programs and impact markets consume Hypercerts. Institutional evaluators and data analysts consume CROSS indicator specifications and gate records.

---

## What This Enables

The CROSS+WALKRI + Hypercerts integration enables a contribution accountability infrastructure that neither system can provide alone:

A Hypercert backed by a CROSS completion gate record is not merely a self-certified impact claim. It is an obligation-architecture-backed claim: the grantee specified a FROM state and TO state at the entry gate, worked toward the stated change, submitted evidence at the completion gate, and received a signed funder determination confirming the evidence met the published criteria. The Hypercert represents that entire process in a transferable on-chain token.

This makes Hypercerts-based impact markets and retroactive funding mechanisms substantially more reliable for buyers and evaluators, because the Hypercert now carries a structured, auditable accountability history rather than a freeform impact scope claim.

---

## Adoption Guidance

Programs currently using Hypercerts as their primary impact evidence mechanism and adopting CROSS+WALKRI should:

1. Configure CROSS's retroactive obligation mode or completion gate to accept a Hypercert token reference as a required evidence artifact. Publish the Hypercert chain and contract address in the gate configuration as a named evidence form.

2. Populate Hypercert work scope and impact scope fields from CROSS entry specification data: the obligation mode, the FROM state condition, the TO state target, and the indicator name. This makes the Hypercert's freeform tags into structured references.

3. Include the CROSS indicator specification fields as Hypercert metadata extensions, either in the Hypercert's `description` field or as a linked document-reference carrying the CROSS indicator ID and the published round configuration URL.

4. Express the CROSS completion gate determination as a signed gate record referencing the Hypercert token ID. This creates the chain of attestation: Hypercert (impact claim) + gate record (funder determination). The format of the gate record is determined by the program's infrastructure.

Programs that do not currently use Hypercerts but want to integrate them should adopt Pattern 1 (completion gate anchored to Hypercert) as the lowest-friction starting point.

---

## Further Information

CROSS: github.com/CrossWalkri/CROSS

WALKRI: github.com/CrossWalkri/WALKRI

Hypercerts: hypercerts.org

Hypercerts GitHub: github.com/hypercerts-org/hypercerts

License: CC0
