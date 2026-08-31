# Predictive Rank as a Circuit-Conditioned Memory Witness for Quantum Error-Correction Syndrome Records

**Author:** Ayush Nadiger  
**Status:** manuscript, August 2026 — not yet posted to arXiv  
**Latest retained source snapshot:** `predictive_rank_qec_arxiv_v8.tex` (17 August 2026)

Repeated QEC syndrome streams inherit memory from both the known extraction circuit and the unknown noise process. This paper asks what finite observed syndrome records can certify about that memory without first assigning physical meaning to an arbitrary latent-state realization.

## Structural result

For a finite past–future word block `H^(ell)` and a causal cut `Gamma` through the selected detector light cone, the manuscript first bounds observable rank by an intrinsic cut complexity of the composed process,

```text
rank H^(ell) <= rho_Gamma,
```

where `rho_Gamma` is the operator-Schmidt rank of the contracted composed process across the cut. After a circuit/noise factorization is declared,

```text
rho_Gamma <= kappa_Gamma * product_e chi_e.
```

For the one-dimensional spatiotemporal Pauli-process model class this becomes `rank H <= kappa_Gamma D`. The statistical target is the **minimum compatible** SPP bond dimension, not the bond dimension of an arbitrary realization.

For a single repeated stabilizer detector track the circuit contribution is computed exactly as `kappa_Gamma = 2`. A controlled two-state correlated-noise model saturates the resulting rank-four bound.

## Finite-sample layer

The manuscript separates three inferential layers rather than treating them as interchangeable:

1. certified, conservative finite-rank tests;
2. empirically calibrated rank-one diagnostics;
3. conditional model checks against a supplied noisy circuit.

For independent windows, empirical distance to the rank-`r` variety gives matched `Theta(epsilon^-2 log(1/delta))` sample complexity for spectrally separated alternatives. The paper also treats beta-mixing and restrictive reversible observed-Markov extensions and states explicitly where those dependence assumptions do not apply.

## Public Google analysis

The current manuscript analyzes two public Google distance-5, 21-round surface-code records with 50,000 shots in each memory basis. The largest circuit-relative discrepancy occurs at detector track `x2_y5` in both bases and remains present across the tested horizons and retrospective acquisition halves.

The interpretation is deliberately limited: this is a **finite-horizon mismatch with the supplied noisy-circuit model**. It is not identification of leakage, a particular microscopic defect, or a device-level environment-dimension lower bound from the Google data alone.

## Source provenance

The exact reviewed source is retained as `predictive_rank_qec_arxiv_v8.tex` in the project source archive. It uses a separate `references.bib` and an accompanying reproducibility/data-analysis bundle. The connected File Library exposes the manuscript for review but does not provide the raw source bundle as a GitHub-uploadable byte stream, so I do not publish a reconstructed or excerpt-stitched `main.tex` here.

When the frozen source bundle is exported, this directory should receive the manuscript, bibliography, figure assets, and analysis scripts together so that the archived TeX is actually compilable.

## Project record

- https://ayushnadiger.github.io/projects/predictive-rank-qec.html

The manuscript's real-device analysis uses Google's public qec3v5 data archive and Stim-based circuit processing. The upstream experimental archive is not redistributed here.

## Claim boundary

Finite-horizon rejection can falsify a low-complexity process class; finite-horizon non-rejection does not certify low infinite-process rank. Converting observable rank into noise-memory or environment-memory statements is explicitly conditional on the declared circuit/noise representation class.
