# Prior Art Stamp: v3.0.0

**Date:** 2026-04-08
**Project:** geometry-of-experience
**Type:** decision
**Branch:** main

## Context

Three papers approaching submission: (1) Born rule / quant-ph with Marcel Reginatto endorsing for arXiv, (2) central-configuration / variety collaboration with Julian Barbour and Maria Lourenco, (3) broader constants / gravity paper. Too many results floating in private repos (RIG vault, barbour-variety-lab) with no public timestamp. Prior art urgency.

## What Was Done

Audited RIG vault (228 derivations, 14 theorems), barbour-variety-lab (3-track program), and Ontigon legal/IP boundaries. Selected results safe for public disclosure (pure mathematical physics, no patent-adjacent implementation details). Created 7 new research notes and 1 new proof script establishing prior art across:

### Measurement Theory (supports Marcel paper)
- Pointer directions from measurement algebra factorization (Ptr = MCP(Z(Fix_H)))
- Born rule saturation theorem strengthened (full F_C(alpha,theta) angular dependence proof)

### Collision-Limit Spectral Theory (Aaron's independent contribution)
- McGehee cone spectral theory with systematic Abelian closures
- KZ Fibonacci bundle (k=3) on collision-excised shape sphere
- Hidden-symmetry matching framework (Track C design)
- Complete Fuchsian -> KZ -> Fibonacci -> universal QC chain

### Broader Framework
- Three fermion generations from b_1=3 on collision-excised shape space
- Bell violations from Hopf fiber linking (OI failure, PI preserved)
- Emergent gravity: G from J_min^2, MOND a_0 from eta/J_min, Lambda from (1-J_min)

Updated all metadata: PRIOR_ART.md (+6 novel claims), CONFIDENCE_TIERS.md, CHANGELOG.md (v3.0.0), README.md (new scope and structure).

## IP Boundary Respected

Excluded: VIMANA coupling, Fibonacci anyon braiding implementation (patent 63/978242 ready to file), Walsh character encoding, GPU kernel parameters, DAEMON architecture, all Ontigon product connections.

## Files Changed

New (7):
- paper/measurement_algebra_factorization_note_2026_04.md
- paper/collision_limit_spectral_structure_note_2026_04.md
- paper/chern_simons_from_collision_regularity_note_2026_04.md
- paper/generations_from_collision_topology_note_2026_04.md
- paper/bell_evasion_hopf_linking_note_2026_04.md
- paper/emergent_gravity_fisher_note_2026_04.md
- proofs/measurement_algebra_factorization.py

Updated (5):
- proofs/born_rule_derivation.py (full saturation theorem)
- PRIOR_ART.md, CONFIDENCE_TIERS.md, CHANGELOG.md, README.md

## Decision Record

The collision-limit spectral theory note explicitly separates Aaron's independent hydrogen program (Track B/C) from the Barbour/Lourenco collaboration (Track A variety line). This separation was requested in the April 8 email to Julian. Track B/C content has never been shared with collaborators and is purely Aaron's contribution.
