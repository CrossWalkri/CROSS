---
title: Attestation Landscape - CROSS+WALKRI
version: 0.1.2
date: 2026-05-18
license: CC0
standards: CROSS v0.3.7 (github.com/cross-walkri/CROSS), WALKRI v0.1.6 (github.com/cross-walkri/WALKRI)
---

# Attestation Landscape

## CROSS+WALKRI Reference Document v0.1.0

---

## Purpose

CROSS and WALKRI are format-agnostic standards. They specify what gate records, conformance records, identity anchors, and pre-commitment records must contain; they do not specify the format those records must take. This document maps the main attestation and verification mechanisms available to programs implementing CROSS+WALKRI, with their properties, tradeoffs, and appropriate use cases.

This document does not prescribe a mechanism. It provides the information a program needs to make a deliberate choice matched to its institutional context, technical capacity, and intended audience.

---

## What Attestations Do in This Context

CROSS+WALKRI produces four types of verifiable records:

**Gate records.** Funder-signed determinations at each gate: entry, progress, completion, continuation. A gate record confirms that a specific entity demonstrated specific obligations to a specific published standard at a specific point in time. Gate records are the cross-program track record infrastructure; when accumulated across rounds and programs, they constitute independently verifiable grantee history.

**Conformance records.** WALKRI audit outcomes for each field specification before a round opens. A conformance record confirms that each application field was specified to WALKRI standard before any applicant saw it. Conformance records are the field quality accountability layer.

**Identity anchors.** Publicly queryable records linking a grantee's display name, legal entity, and prior work to a stable identifier. Identity anchors are the cross-program identity infrastructure; they are what makes the organizational identity declaration independently verifiable rather than self-reported.

**Pre-commitment records.** Content-addressed commitments to the round specification published before the application window opens. Pre-commitment records are the evidentiary basis for applicant redress rights under the summative gate provisions.

Each of these four record types has different requirements for who signs it, when it is produced, and who needs to be able to verify it. The mechanism choice should match those requirements.

---

## The Four Main Mechanisms

### On-Chain Attestations (EAS and comparable)

The Ethereum Attestation Service (EAS) and comparable on-chain attestation systems produce chain-anchored, schemaUID-typed records that any party can query without trusting any intermediary. Records are permanently associated with a signing address (the attesting party), a recipient address (the subject of the attestation), a schema, and a data payload.

**Properties:**
- Publicly queryable by any party with a blockchain explorer or API
- Permanent and non-repudiable once anchored
- Funder-signed records require the funder to control a signing address
- Schema-typed: the data structure is registered and verifiable
- Available on Optimism, Base, Arbitrum, Ethereum mainnet, and comparable EVM-compatible chains
- Gas cost per attestation (typically small but non-zero)
- Natively readable by Web3 infrastructure (KarmaGAP, Gitcoin Passport, Hypercerts, and comparable platforms)

**Best for:**
- Cross-program track records that any subsequent program should be able to verify without contacting the original funder
- Grantee milestone records where cross-ecosystem visibility is the goal
- Identity anchors in Web3 contexts where wallet-address-based identity is the norm
- Pre-commitment records for Web3 programs where on-chain timestamp is the standard of proof

**Not ideal for:**
- Institutional funder contexts where on-chain records are not recognized as official documentation
- Programs with no technical capacity to manage signing addresses
- Sensitive contexts where the data payload should not be permanently public

---

### W3C Verifiable Credentials

W3C Verifiable Credentials (VCs) are JSON-LD signed documents issued by a credential issuer (the funder or auditor), held by a credential holder (the grantee), and verifiable by any credential verifier (a subsequent program, an institutional funder, an analyst). VCs are holder-sovereign: the grantee controls which credentials they present and to whom.

**Properties:**
- Cryptographically signed by the issuer (funder or auditor) using a DID-based key
- Holder-sovereign: the grantee holds the credential and presents it selectively
- No blockchain required; credentials can be stored anywhere and verified offline
- Natively readable by any standards-compliant VC verifier
- Compatible with W3C DID infrastructure (did:web, did:key, did:ethr, and others)
- No per-credential cost beyond the issuer's key infrastructure
- Selective disclosure is possible with certain VC formats (SD-JWT)

**Best for:**
- Portable grantee credentials that can be presented to any program or institutional funder
- Conformance records that WALKRI-certified programs want grantees to carry
- Contexts where the credential holder's sovereignty over their record matters
- Cross-sector use cases spanning both Web3 and institutional contexts

**Not ideal for:**
- Contexts where the verifier cannot operate VC verification infrastructure
- Programs that want records queryable without grantee cooperation (the grantee must present the VC; a verifier cannot query for it without grantee consent)

---

### Signed Institutional Documents

Signed institutional documents include signed PDFs, notarized records, official letters on institutional letterhead, and comparable traditional verification formats. These are familiar to institutional funders, legal bodies, and government agencies.

**Properties:**
- Requires no technical infrastructure beyond document signing
- Universally recognized in institutional contexts
- Verification typically requires contacting the issuing party or checking a registry
- Not natively queryable by digital systems without additional infrastructure
- Can be timestamped via RFC 3161 timestamp authorities for pre-commitment use
- Long-term storage is the responsibility of the issuing or holding party

**Best for:**
- Programs reporting to USAID, the Gates Foundation, World Bank, or comparable institutional funders who require official documentation
- Legal contexts where digital-only records do not satisfy documentation requirements
- Programs with no Web3 technical capacity
- Jurisdictions where notarized documents are the standard of proof for accountability claims

**Not ideal for:**
- Cross-program digital verification where a program needs to query records programmatically
- Web3 contexts where institutional documents are not natively readable by the infrastructure

---

### Timestamping Services

Timestamping services (RFC 3161 compliant authorities, on-chain anchoring, or comparable mechanisms) produce verifiable proof that a specific document existed at a specific point in time. They are the primary mechanism for round specification pre-commitment records.

**Properties:**
- Proves that content existed at a timestamp, not who signed it or what it means
- RFC 3161 timestamps are issued by trusted timestamp authorities (including many national and commercial certificate authorities) and are legally recognized in many jurisdictions
- On-chain anchoring (publishing a content hash to a public blockchain) achieves the same temporal proof with different trust assumptions
- No ongoing relationship with the timestamping authority required after issuance
- Verification is straightforward: hash the document, compare to the anchored hash, verify the timestamp

**Best for:**
- Round specification pre-commitment records: proving that the round specification existed before the application window opened
- Any situation where the primary evidentiary need is "this document existed at this time"
- Programs that want pre-commitment capability without publishing a full on-chain transaction

**Not ideal for:**
- Situations where the record also needs to name the issuer (use signed records instead)
- Situations where the record needs to be queryable by entity (use EAS or VCs instead)

---

## Selection Guidance

The right mechanism for each record type depends on three factors: who the primary verifier is, whether the grantee's cooperation is required for verification, and what the program's technical capacity is.

| Record type | Primary verifier | Grantee cooperation needed | Recommended mechanism |
| :-- | :-- | :-- | :-- |
| Gate records (Web3-facing programs) | Subsequent Web3 programs | No (public queryable) | On-chain EAS attestation |
| Gate records (institutional-facing programs) | Institutional funders | No (registry or direct contact) | Signed institutional document with timestamp |
| Gate records (bridging programs) | Both | Partial (VC is holder-sovereign) | W3C Verifiable Credential |
| WALKRI conformance records | Any program auditing field quality | No (public queryable or holder-presented) | On-chain EAS or W3C VC |
| Identity anchors (Web3) | Subsequent Web3 programs | No | On-chain EAS or ENS |
| Identity anchors (institutional) | Institutional funders, legal bodies | No (public registry) | Signed institutional document |
| Pre-commitment records (Web3) | Any party, no cooperation needed | No | On-chain transaction (hash anchor) |
| Pre-commitment records (institutional) | Any party, no cooperation needed | No | RFC 3161 timestamp authority |

---

## Use Case Mapping for CROSS+WALKRI Provisions

**Organizational identity declaration (CROSS Part IV):** The prior round history field benefits from funder-signed gate records as independently verifiable corroboration. In Web3 programs, on-chain EAS attestations from prior funders serve this function. In institutional programs, signed document registries serve this function. The WALKRI public record query evidence form applies to any mechanism that is publicly queryable without grantee cooperation.

**Sufficiency architecture declaration - co-funding coordination (CROSS Part IV):** A coordination record proving co-funding was committed before work began is best served by an on-chain contract (the commitment is provably timestamped) or a multi-party signed document with a trusted timestamp. The key property is the pre-work timestamp; the mechanism is secondary.

**Gate record legibility and cross-program track record (CROSS Part IV):** On-chain EAS is the highest-value mechanism for this use case because records are queryable without grantee cooperation. W3C VCs are second-best where the grantee is expected to present credentials proactively. Signed institutional documents require direct contact with the prior funder for independent verification.

**Round specification pre-commitment (CROSS Part IV):** Timestamping (RFC 3161 or on-chain) is the appropriate mechanism. The record needs only to prove that the document existed before the window opened; it does not need to name the issuer or be queryable by entity.

**WALKRI conformance records (WALKRI Part I, Section 3.7):** On-chain EAS or W3C VCs are the most useful mechanisms for conformance records that programs want downstream data consumers to be able to verify. Signed documents work for institutional contexts. The public record query evidence form in WALKRI Section 3.7 applies when the conformance record is in a publicly queryable format.

---

## Layered Attestation

Programs that bridge institutional and Web3 contexts may produce layered attestations: the same accountability event is recorded in multiple formats for different consumer audiences. A completion gate determination might produce both an EAS attestation (queryable by KarmaGAP and subsequent Web3 programs) and a signed institutional document (presentable to USAID or a foundation board). The two records are not redundant; they serve different verifier audiences with different infrastructure.

Layered attestation is not a conformance requirement. It is a practical option for programs operating across both ecosystems. The content requirements from CROSS and WALKRI apply equally to both records; the format is determined by the target audience for each.

---

## Further Information

CROSS: github.com/cross-walkri/CROSS

WALKRI: github.com/cross-walkri/WALKRI

Ethereum Attestation Service: attest.sh

W3C Verifiable Credentials: w3.org/TR/vc-data-model

RFC 3161 Timestamping: tools.ietf.org/html/rfc3161

License: CC0

---

## Changelog

| Version | Date | Summary |
|---|---|---|
| 0.1.2 | 2026-05-18 | Standards references updated to CROSS v0.3.7 and WALKRI v0.1.6. |
| 0.1.1 | 2026-05-17 | Standards references updated to CROSS v0.3.3 and WALKRI v0.1.1. |
| 0.1.0 | 2026-05-16 | Initial draft. Four record types (gate records, conformance records, identity anchors, pre-commitment records). Four mechanism options (on-chain EAS, W3C VCs, signed institutional documents, timestamping services) with properties, best-use, and not-ideal characterizations. Selection guidance table. Use case mapping to CROSS+WALKRI provisions. Layered attestation section. |
