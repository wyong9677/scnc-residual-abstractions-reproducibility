# Numerical Evidence Dataset

This repository contains the publication-facing numerical data, machine-readable
certificates, calibrated parameter tables, derived evidence, and provenance
records supporting the numerical studies in:

**Compositional Residual Abstractions for Stateful Services in Safety-Critical
Networked Control: Semantics, Viability, and Information Complexity**

Authors: Yong Wang, Qiurui Liu, Ying Zhou, and Xiao Ma.

## Scope

The dataset records the numerical evidence used for the UAV, nonlinear CSTR,
and finite full-history task studies reported in the associated article.

The repository is an evidence dataset rather than a complete archival copy of
the internal research workspace. Failed runs, temporary files, duplicated
archives, local execution logs, machine-specific paths, internal formal-audit
material, and unrelated development artifacts are intentionally omitted.

## Main contents

- UAV multi-factor calibration and grid-sweep evidence.
- CSTR coordinate-task and structured numerical evidence.
- Full-history residual/task data.
- Exact finite task-value profiles.
- Certified conflict-graph data and certificates.
- Application-level calibrated factors.
- Final numerical claims and provenance summaries.

## Third-party data

Third-party raw packet captures, including externally hosted NIST C-V2X source
captures, are not redistributed here. Such data should be obtained from the
original source cited in the associated article. Only study-specific derived
evidence is included where appropriate.

## Claim boundary

Exact finite-domain numerical claims apply only to the declared finite
plant-anchor, action, service-transition, and horizon sets specified in the
article and supporting material.

Finite-grid safety certification is not identified with a continuous-state
maximal viability kernel.

Coordinate metrics are not identified with behavioral residual metrics unless
an explicit comparison result is established.

## Provenance sanitization

Four provenance records from the canonical R13 numerical freeze are included in
sanitized form. Machine-local absolute filesystem paths were replaced by
portable symbolic or package-relative paths. Scientific numerical values,
status fields, evidence relationships, and study identifiers were otherwise
preserved.

The internal cleanup receipt and local housekeeping checksums are not part of
this public dataset.

## Integrity

`MANIFEST_INCLUDED.csv` lists publication-facing artifacts.

`SHA256SUMS.txt` contains SHA-256 checksums generated from this public dataset
after sanitization and is the authoritative checksum list for the archived
release.

## Archival record

A permanent Zenodo DOI will be added after the public v1.0.0 release is
archived.
