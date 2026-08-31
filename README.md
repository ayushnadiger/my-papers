# Ayush Nadiger — quantum papers

This repository is a clean archive of my quantum-information, quantum-hardware, and fault-tolerant-architecture manuscripts.

The public arXiv paper is preserved as a canonical record. The six active architecture papers include their current reviewed `main.tex` and `supplement.tex` sources. Background manuscripts 07–09 record the exact latest reviewed source snapshot and public verification provenance; source is mirrored only when it can be transferred without reconstructing or silently changing the retained manuscript. Reproducibility code that already has a dedicated public repository is linked rather than duplicated wholesale.

## Public preprint

- [`00_trapped_ion_geometry/`](00_trapped_ion_geometry/) — **Geometry-controlled correlated electric-field noise in enclosed ion traps from billiard return spectra**, arXiv:2608.24770 (2026).

## Fault-tolerant architecture manuscripts

- [`01_high_rate_qldpc_interconnects/`](01_high_rate_qldpc_interconnects/) — **High-Rate qLDPC Gates over Heralded Interconnects: QEC-Aware Entanglement Service**.
- [`02_2d_hybrid_repeaters/`](02_2d_hybrid_repeaters/) — **Correction Exposure and Service Geometry in Sparse Hybrid Quantum Repeater Networks**.
- [`03_trapped_ion_photonic_service/`](03_trapped_ion_photonic_service/) — **Fault-Tolerant Service Contracts for Integrated Trapped-Ion Photonic Interconnects**.
- [`04_gkp_resource_factories/`](04_gkp_resource_factories/) — **Throughput Is Not Enough: Synchronization and Loss Constraints for GKP-State Factories in High-Rate Photonic Repeaters**.
- [`05_reset_aware_spin_photon/`](05_reset_aware_spin_photon/) — **Occupancy-Aware Reset Control for Sequential Quantum Repeaters with Exposure-Aged Spin–Photon Interfaces**.
- [`06_stochastic_qldpc_factories/`](06_stochastic_qldpc_factories/) — **Tanner Frontiers in Stochastic qLDPC Entanglement Factories**.

## Background manuscripts

- [`07_repair_identifiability/`](07_repair_identifiability/) — **Repair Identifiability and Product-Measurement Complexity of Bond Failures in Graph States**, v10 (August 2026). Includes the frozen v10 adversarial audit and citation metadata; full verification code is maintained in the dedicated public repository linked inside.
- [`08_predictive_rank_qec/`](08_predictive_rank_qec/) — **Predictive Rank as a Circuit-Conditioned Memory Witness for Quantum Error-Correction Syndrome Records**, v8 source snapshot (August 2026).
- [`09_covariance_geometry_qec/`](09_covariance_geometry_qec/) — **Covariance Geometry of Linearized Quantum Erasure Correction**, August 2026 source snapshot. Includes frozen public verification metadata/output and the canonical verifier link.

The earlier graph-state cut/localization drafts are treated as one background research line here; the current v10 repair-identifiability manuscript is the archive entry rather than inflating successive drafts into separate papers.

## Source-status convention

- **Canonical public record:** an arXiv identifier is the source of truth.
- **Mirrored manuscript:** the reviewed TeX source is present in this repository.
- **Reviewed snapshot record:** the exact retained source filename/version is recorded, but no reconstructed TeX is substituted when the connected archive cannot export raw source safely.

This convention is deliberate: a public archive should not make an older draft or stitched excerpt look like the manuscript that was actually reviewed.

## Scope

The current research program is hardware-aware fault-tolerant quantum architecture: identifying which physical or stochastic state is lost in a scalar hardware abstraction, deriving the service law seen by the QEC consumer, and translating it back into hardware requirements.

This repository intentionally excludes unrelated optimization/software papers.
