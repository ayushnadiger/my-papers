# Covariance Geometry of Linearized Quantum Erasure Correction

**Author:** Ayush Nadiger  
**Status:** manuscript, August 2026 — not yet posted to arXiv  
**Latest retained source snapshot:** `covariance_geometry_linearized_qec(2).tex` (16 August 2026)

A fixed-dimensional quantum code is a point of a Grassmannian. Exact erasure correction cuts out a Knill–Laflamme zero locus inside that Grassmannian. This manuscript identifies the first-order normal geometry of that locus.

## Central theorem

At an exact erasure-correcting code with erased marginal `sigma_A`, the vertical differential of the KL section satisfies

```text
d^v s_A (d^v s_A)^* = 4 Cov_{sigma_A} ⊗ I_{Herm_0(L)}.
```

Thus the complete nonzero singular spectrum of the linearized exact-QEC constraints is fixed by the covariance spectrum of the erased marginal; logical dimension changes multiplicities rather than the underlying stiffness scales.

## Consequences

- On the full-rank erased-marginal stratum, the exact-code locus is smooth with the expected codimension.
- A quadratic mean-square leakage functional is the squared norm of the KL section up to the Haar factor, making the full-rank exact locus Morse–Bott with covariance-controlled normal Hessian.
- For qubit erasure, the reduced normal condition number is exactly the reciprocal of the common qubit–rest concurrence, `kappa_red = 1/C_A`.
- For simultaneous erasure constraints, the stacked KL sections produce cross-Gram blocks governed by compressed observable correlations and a linearized deformation complex.
- Exact symbolic calculations show infinitesimal rigidity modulo local physical unitaries for the `[[4,2,2]]` and `[[5,1,3]]` codes under the stated erasure constraints.

## Source provenance

The latest reviewed source is `covariance_geometry_linearized_qec(2).tex`. One archive-level correction is required before public source mirroring: that file still contains an old `lostree9` verification-repository URL. The correct public verification path is the `ayushnadiger` repository path below. I am recording the source snapshot here rather than silently publishing a modified file under the same provenance label.

Once the frozen manuscript bundle is exported, the source should be mirrored here with that stale URL corrected and otherwise kept scientifically unchanged.

## Verification

The public verification suite is mirrored under [`repro/`](repro/) and also remains available at:

- https://github.com/ayushnadiger/ayushnadiger.github.io/tree/main/code/covariance-geometry-qec

Project page:

- https://ayushnadiger.github.io/projects/covariance-geometry-qec.html

The verifier independently checks the covariance-normal Gram identity under basis changes, covariance trace/determinant formulas, the leakage identity, exact KL conditions, and the stated finite-code Jacobian/rigidity calculations.

## Claim boundary

The paper does not claim that covariance in quantum-state geometry is itself new, nor that the chosen quadratic leakage functional is the unique operational approximate-QEC metric. The novelty claim is restricted to the exact linearized KL normal form and its stated geometric consequences.
