# Repair Identifiability and Product-Measurement Complexity of Bond Failures in Graph States

**Author:** Ayush Nadiger  
**Status:** manuscript v10, August 2026 — not yet posted to arXiv  
**Latest retained source snapshot:** `main_v10(1).tex` (30 August 2026)

This paper asks a repair-level question for a known graph-state network: after an intended bond is suspected, can product-Pauli data distinguish a genuinely severed entangling bond from endpoint-memory dephasing that can look identical under the target stabilizer dictionary?

The central exact support statement is

```text
P distinguishes C_e from D_e  iff  P ∈ ±S(G−e) \ ±S(G).
```

The manuscript develops the resulting measurement-resource theory: near-blindness of target-stabilizer data, locality criteria, raw-versus-compressed product-measurement context complexity, bounded-weight separations, exact graph-family results, computer-assisted finite censuses, and finite-shot/noise scaling.

## Current theorem package

- Target-stabilizer diagnosis becomes ill-conditioned as endpoint coherence `g -> 0`, with optimal copy scaling `Theta(g^-2 log(1/delta))`; at full dephasing the target graph-basis diagonals coincide exactly.
- The missing repair information lives exactly in failed-graph stabilizers absent from the target stabilizer group.
- Endpoint-pair tomography is blind except at the leaf/external-twin boundary characterized in the manuscript.
- Three finite setting resources are separated: raw cut diagnosis, target-compressed cut diagnosis, and raw bond-repair diagnosis, with `c_raw^cut <= c_targ^cut <= c_raw^rep`.
- A raw repair schedule must simultaneously localize the candidate edge at the target level and expose a compatible failed-graph repair witness for every edge.
- For connected graphs with an edge, one-context raw repair is possible iff the graph is a star; complete graphs need two contexts, non-star trees need two, and wheels need at most three.
- For wheels `W_n`, `n >= 8`, a weight-three cap creates a qualitative raw-versus-target separation.
- Exact enumeration over all 12,112 connected graph isomorphism classes on 2–8 vertices found no raw-cut cost above 2 and no raw-repair cost above 3; these are computer-assisted finite results, not universal theorems.

## Source provenance

The exact reviewed manuscript source is retained as `main_v10(1).tex` in the project source archive. The connected File Library exposes it for review but not as a raw byte stream that can be safely mirrored through the GitHub connector. I therefore do **not** reconstruct a purported exact `main.tex` from truncated excerpts here.

The source will be mirrored verbatim when the frozen submission bundle is exported. Until then, this directory records the precise reviewed snapshot and points to the complete public verification package below.

## Verification

Dedicated public verification repository:

- https://github.com/ayushnadiger/repair-identifiability

Project page:

- https://ayushnadiger.github.io/projects/graph-state-repair-diagnosis.html

The verification repository contains the v10 adversarial audit, citation metadata, exact Python checks, and the C++17/OpenMP sources used for the large wheel obstruction calculations.

## Claim boundary

This is a known-topology, product-Pauli, independent-copy diagnosis model. The bond-local repair catalogue is deliberate. Side information such as heralding records, hardware telemetry, and timestamps is outside the state-only model, and finite graph census results are not promoted into unproved asymptotic claims.
