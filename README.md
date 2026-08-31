# Ayush Nadiger — quantum papers

This repository is a clean archive of my quantum-information, quantum-hardware, and fault-tolerant-architecture manuscripts.

Each directory contains the manuscript source and a short status note. Public arXiv papers are preserved as canonical records; unpublished manuscripts are review snapshots and may change before submission. Reproducibility code that already has a dedicated repository is linked rather than duplicated wholesale.

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

- [`07_repair_identifiability/`](07_repair_identifiability/) — graph-state defect localization, repair identifiability, and diagnostic measurements.
- [`08_predictive_rank_qec/`](08_predictive_rank_qec/) — **Finite-Horizon Predictive-Rank Tests for Quantum Error-Correction Syndrome Records**.
- [`09_covariance_geometry_qec/`](09_covariance_geometry_qec/) — **Covariance Geometry of Linearized Quantum Erasure Correction**.

The two earlier graph-state cut manuscripts are being treated as one background research line in this archive; they should not be mistaken for two independent current research directions.

## Scope

The current research program is hardware-aware fault-tolerant quantum architecture: identifying which physical or stochastic state is lost in a scalar hardware abstraction, deriving the service law seen by the QEC consumer, and translating it back into hardware requirements.

This repository intentionally excludes unrelated optimization/software papers.