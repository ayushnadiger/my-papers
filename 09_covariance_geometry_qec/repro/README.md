# Covariance Geometry of Linearized Quantum Erasure Correction

Public reproducibility files for the manuscript **Covariance Geometry of Linearized Quantum Erasure Correction**.

## Quick start

Tested with Python 3.13.5, NumPy 2.3.5, and SymPy 1.14.0.

```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python verify_erasure_geometry.py
```

The canonical verifier is maintained at:

https://github.com/ayushnadiger/ayushnadiger.github.io/tree/main/code/covariance-geometry-qec

It independently checks:

- the full covariance-normal Gram identity `J J^T = 4 Cov(sigma_A) \otimes I`, both in canonical coordinates and after independent random unitary changes of the erased-subsystem and logical bases;
- the trace and determinant formulas for the covariance operator;
- the Haar mean-square leakage identity, reporting a Monte Carlo standard error and using a six-standard-error acceptance criterion;
- the Knill--Laflamme scalar-compression conditions before any stabilizer-code Jacobian is formed;
- exact symbolic stacked-Jacobian rigidity calculations for `[[4,2,2]]` and `[[5,1,3]]`;
- the numerical first-order deformation count for the Steane `[[7,1,3]]` code.

A successful run ends with:

```text
ALL CHECKS PASSED
```

`verification_output.txt` in this directory is the frozen public output from that verifier. The Python script itself remains canonical at the link above until the full manuscript source bundle is exported, avoiding two independently drifting copies of the verification program.

The analytic claims are proved in the manuscript; the script is an independent reproducibility and sanity-check suite, not a substitute for those proofs.
