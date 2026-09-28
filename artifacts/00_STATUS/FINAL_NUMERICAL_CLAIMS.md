# Safety-Critical Networked Control — Final Numerical Freeze

This directory is the canonical numerical closure snapshot.
It contains the successful evidence runs copied before cleanup.

## Final certified numerical claims

- Full-history residual-to-task upper sensitivity passed in 6 scenarios; observed theorem-facing `C_T` values: `[0.1875]`.
- Global reverse constants observed: `[0.0]`; therefore no global reverse sensitivity is claimed.
- UAV same-application calibrated factors:
  - timer: a=0.9375000000000133, d=0.9999999999999997, C=57.60000000000016, R2=1.0.
  - position_grid: a=0.25000000000000006, d=1.9683178004367246, C=18.27625176835979, R2=0.9999628922122721.
  - velocity_grid: a=0.6250000000000001, d=1.9235018959479995, C=3.5330494147764475, R2=0.9997842532248722.
- UAV calibrated allocation Delta = `0.08440117217519658`.
- Analytic epsilon* = `[0.018403768449072183, 0.135841743875344, 0.05309952525656824]`.
- Modeled cost reduction versus equal weighted-budget allocation = `0.18068975339112148`.
- KKT residual = `0.0`.
- Declared finite Stage-7 task value is replayed with exact rational arithmetic:
  `eta_V = 0` on the declared 81-anchor, finite-action, two-sample task.
- Maximum legacy float32 export error = `8.344650268554688e-09`.
- Exact E=0.001 graph `independent_dtau_0p025`: chi=[25,25], exact=1, edges=300, legacy edge mismatches=0.
- Exact E=0.001 graph `shared_dtau_0p025`: chi=[59,59], exact=1, edges=3852, legacy edge mismatches=0.

## Claim boundary

- CSTR delay is a coordinate metric d_tau, not the behavioral residual metric d_sigma.
- Exact eta_V=0 is restricted to the declared finite Stage-7 task.
- UAV allocation constants are finite-grid application calibrations under the frozen model.
- No continuous-domain exact viability-kernel equality is asserted by this freeze.
