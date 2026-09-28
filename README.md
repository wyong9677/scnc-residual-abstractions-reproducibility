# Numerical Reproducibility Package

This repository contains the numerical code, structured data, derived numerical
evidence, and final generated outputs supporting the numerical studies in:

**Compositional Residual Abstractions for Stateful Services in Safety-Critical
Networked Control: Semantics, Viability, and Information Complexity**

Authors: Yong Wang, Qiurui Liu, Ying Zhou, and Xiao Ma.

## Scope

The package is intended to reproduce and audit the numerical evidence reported
for the UAV, nonlinear CSTR, and finite full-history task studies.

Only canonical publication-facing numerical artifacts are included. Failed,
partial, temporary, duplicated, machine-local, and internal formal-audit
artifacts are intentionally omitted.

## Third-party data

Third-party raw packet captures, including external NIST C-V2X source captures,
are not redistributed in this repository. They should be obtained from the
original source cited in the associated article. Derived statistics and the
study-specific processing code may be included where redistribution is
permitted.

## Reproducibility boundary

Exact finite-domain claims apply only to the declared finite plant-anchor,
action, service-transition, and horizon sets specified in the article and
supporting material. Finite-grid certification is not presented as a
continuous-state maximal viability-kernel computation.

## Contents

- `artifacts/`: publication-facing numerical code, data, parameters, and outputs.
- `MANIFEST_INCLUDED.csv`: included-file inventory.
- `SHA256SUMS.txt`: SHA-256 hashes of included numerical artifacts.

A permanent DOI will be added after archival of the corresponding release in
Zenodo.

## Provenance sanitization

Four machine-readable provenance files from the canonical numerical freeze are
included in sanitized form. Machine-local absolute filesystem paths were
replaced by portable package-relative or symbolic path markers. Numerical
values, scientific status fields, filenames, hashes, and evidence relationships
were otherwise left unchanged.

The internal cleanup receipt was intentionally omitted because it records local
housekeeping operations rather than scientific evidence.

The canonical numerical source for this public package is the R13 final
numerical freeze. Earlier stage identifiers appearing in provenance records
document lineage only and do not supersede the R13 freeze.
