# CROSS as a machine-readable conformance contract

A short read for engineers deciding whether this is the shape they want for validating grant outcome indicators.

## Two machine-readable layers, and which one this is

CROSS has two machine-readable layers, and they answer different questions. The `schemas/` directory is the serialization and interop layer: the JSON Schema family (round-config, runbook, applicant-facing-publication) that lets a funder configure a round, an operator run it, and an applicant see it, so implementers can build tooling and move round data into and out of CROSS. This directory is the conformance layer: it validates whether one CROSS conformance object, the outcome indicator, is well-formed against the standard. Serialization moves the data; conformance checks it. Neither replaces the other, and this one is generated from a single source while the serialization family is currently hand-authored.

## The problem this addresses

A grant round collects outcome claims from applicants, and the decision to fund or to release the next payment rests on them. When the analysis later turns out wrong, it usually traces to an indicator that was a label, not a measurement instrument: a name with no operational definition, a claim with no baseline to measure change against, a number sourced from a spreadsheet only the applicant can see. CROSS makes the specification of each self-specified indicator a checkable artifact before the round opens, so what varies in the reported data is real difference, not applicants reading the same field differently. This directory is that discipline expressed as a machine-readable contract.

## What CROSS is, in one line

CROSS is the grants domain application of CRAFT: the standard for a grant round's obligation architecture, gates, and indicators. Its conformance-bearing measurement unit is the outcome indicator (Part V), the object this layer models, which is CROSS's realization of CRAFT Condition 4 and its composition point with WALKRI.

## The rules that make an indicator more than a name

Three conditional obligations do the work a bare field list cannot. A contract-centric indicator, one whose obligation is a contract's behavior, must name its execution and verification instruments (the invariant, the method, the artifact, a failure surface); an indicator resting only on applicant-controlled test suites fails. A change or retroactive indicator must carry a baseline, because a change with no documented FROM state cannot be shown. And an applicant-controlled data source must name independent corroboration, because a number only the beneficiary can see is not auditable. The schema enforces all three, and closes its top level so no aggregate score can be smuggled in to stand for the profile.

## One source, every format

The prose standard and the machine-readable schema come from one source, neither a byproduct of the other. One LinkML model generates the JSON Schema, the Zod, the JSON-LD context, SHACL, OWL, and GraphQL, plus a conformance verdict and a SARIF findings run. Edit the standard, regenerate, and every format moves together. Nothing is hand-maintained, so no format can silently fall behind the standard, which is the failure the `schemas/` family, hand-authored and by its own note trailing the standard, currently shows.

## What the schema does and does not decide

CROSS's obligations split, and because CROSS is a large standard about rounds, most of them are audit judgments over a round rather than a shape in one indicator. Some are **shape**: the indicator carries its required fields, the measurement form is classified on three axes, a contract-centric indicator names its verification instruments, a change indicator carries a baseline, an applicant-controlled source names corroboration. Most are **judgment**: whether the rationale engages seriously with alternatives, whether the operational definition actually meets WALKRI's bar, whether the round runs its gate architecture and conflict-of-interest framework, whether Part XIII declares the full CRAFT and CSIS inheritance. The register (`src/cross-register.yaml`) marks each obligation as shape, judgment, or mixed. The schema enforces the shape of the indicator; the round-level and judgment obligations are the auditor's, and this directory is honest about that line.

## Where this fits the family

CROSS is the first domain application in a family that shares this one-source-generate approach: STRUCK at the exit boundary, ORE at the input boundary, WALKRI at the field, and CRAFT as the meta-standard between the doors. CROSS inherits CRAFT's chain-framing conditions and composes with WALKRI at the field level, which is exactly where the indicator's operational definition meets WALKRI's Part III. Proving the pipeline on STRUCK, ORE, WALKRI, CRAFT, and now CROSS means the conformance-layer shape and tooling are settled across the family.
