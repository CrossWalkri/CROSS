# CROSS+WALKRI JSON Schema Family

This directory holds the JSON Schema family for CROSS+WALKRI round artifacts. It carves a single funding round into the views the different parties need, so that a round can be configured, operated and published without any party working from a document written for someone else.

Three schemas are cohort-facing. `round-config-0_2_0.json` is the funder view: the complete configuration a funder publishes for a round, operationalizing the Commit stage of the CLEAR lifecycle. `runbook-0_2_0.json` is the operator view: how those parameters are executed across the lifecycle, where the config says what is to be done. `applicant-facing-publication-0_2_0.json` is the applicant view: the same round projected down to what applicants need in order to understand and act, with funder-side configuration detail withheld. The `0_1_0` file for each of the three is the earlier skeleton it supersedes, kept so that instances declaring those versions still resolve.

`round-identity-0_1_0.json` is the shared sub-schema every cohort schema references. Its fields, `round_id`, `program_id`, `funder_id`, `cycle_number` and `conforms_to`, are the join key across the family: they are what allows a config, a runbook and an applicant publication to be recognized as describing the same round.

`cross-walkri-release-0_1_0-manifest.json` names the compatible set, which is round-identity 0.1.0, round-config 0.2.1, runbook 0.2.0 and applicant-facing-publication 0.2.1. Conforming instances declare `conforms_to: cross-walkri/release@0.1.0`. Filenames are pinned at the minor version while the internal canonical version carries the patch, so `round-config-0_2_0.json` declares 0.2.1.

`examples/` holds two round-config instances, Octant Epoch 13 and the Te Puni Kokiri Iwi Development Fund.

## Status

This family is an interim pre-stability snapshot, not v1.0, and it trails the standard it serves. The release snapshot is 0.1.0, with members at 0.2.1 and below; the CROSS standard in this repository is at 0.5.2. The schemas have not been reconciled against that version of the standard, and the gap is stated here rather than left for a reader to discover.

## Identifiers

Every `$id` and `$ref` points at the raw content host, for example `https://raw.githubusercontent.com/CrossWalkri/CROSS/main/schemas/round-identity-0_1_0.json`. A resolver needs the file itself, and the ordinary github.com URL for a repository file serves an HTML page that no validator can read.
