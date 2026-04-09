# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [3.0.0] - 2026-04-08

### Added — Measurement Theory
- `paper/measurement_algebra_factorization_note_2026_04.md` — Pointer directions from Kraus support graph via Heisenberg fixed-point center
- `proofs/measurement_algebra_factorization.py` — Computational verification of the support/rate factorization
- Updated `proofs/born_rule_derivation.py` with full Cramér-Rao saturation theorem (F_C(α,θ) angular dependence proof)

### Added — Collision-Limit Spectral Theory
- `paper/collision_limit_spectral_structure_note_2026_04.md` — McGehee cone spectral theory, KZ Fibonacci bundle, systematic Abelian null results, hidden-symmetry matching framework
- `paper/chern_simons_from_collision_regularity_note_2026_04.md` — Complete chain: Fuchsian regularity → KZ → k=3 → SU(2)₃ MTC → Fibonacci → universal QC

### Added — Broader Prior Art
- `paper/generations_from_collision_topology_note_2026_04.md` — Three generations from b₁=3 on collision-excised shape space and |π₁(L(3,1))|=3
- `paper/bell_evasion_hopf_linking_note_2026_04.md` — Bell violations from Hopf fiber linking (OI failure, PI preserved)
- `paper/emergent_gravity_fisher_note_2026_04.md` — G from J²_min, MOND a₀ from η/J_min, Λ from (1-J_min)

### Changed
- PRIOR_ART.md extended with 6 new novel contribution entries
- CONFIDENCE_TIERS.md updated for new claims
- README updated with new repo structure and research frontier

### Notes
- This is a major prior-art stamp driven by publication-pipeline urgency
- The collision-limit spectral framework is Aaron's independent contribution, distinct from the Barbour/Lourenço central-configuration collaboration
- The measurement algebra + Born rule together constitute a complete geometric measurement theory

---

## [2.1.1] - 2026-04-06

### Added
- `paper/neutral_three_body_coulomb_note_2026_04.md` - dated note on neutral pairwise Coulomb critical shapes on the `N=3` preshape sphere
- `paper/pairwise_vs_collective_n3_note_2026_04.md` - dated note on the structural split between pairwise and collective observables on `N=3` shape space

### Changed
- README updated to link the new `N=3` geometry notes

### Notes
- These notes are public baseline geometry documents, not a many-body hydrogen package
- They are intended to separate stable `N=3` shape-space structure from internal operator-side work

---

## [2.1.0] - 2026-03-28

### Added
- `paper/structural_bridge_note_2026_03.md` - dated note on the activation / retention / reconciliation line

### Changed
- README now states repo scope explicitly: public prior-art mirror, not full canonical vault
- RELEASE_NOTES_v2.md corrected to match files actually present in the repository
- PRIOR_ART.md extended with the measurement / decoherence / gravity-bridge prior-art baseline

### Notes
- The new structural-bridge note is a timestamped research update, not a full derivation package
- The open gap is still geometric parameter derivation, not architecture

---

## [2.0.0] - 2026-01-31

### Added
- **Theorem 6: Parafermion Universality** — η = 1/15 from Z₃ CFT (k=3)
- **Theorem 7: Born Rule Derivation** — P = |ψ|² from Fisher-Fubini compatibility
- **Theorem 8: Fibonacci Fusion** — τ × τ = 1 + τ from collision topology
- **Theorem 9: Consciousness Framework** — Self as topological defect
- `proofs/parafermion_eta.py` — Derives η = 1/15 from SU(2)_k theory
- `proofs/born_rule_derivation.py` — Proves Born rule from metric compatibility
- `RELEASE_NOTES_v2.md` — Full documentation of new claims
- Prior art comparison with Nielsen (TUFT)

### New Predictions
| Prediction | Formula | Value | Status |
|------------|---------|-------|--------|
| Geometric friction | η = 1/15 | 0.0667 | NEW |
| MaxEnt exponent | β = η(1+h_σ) | 0.071 | Matches observation |
| Fibonacci quantum dimension | d_τ = φ | 1.618 | Exact |

### Framework Extensions
- Z₃ parafermion universality class identification
- Information-geometric derivation of Born rule
- Consciousness as fiber holonomy

---

## [1.1.0] - 2025-12-05 (Unreleased additions)

### Added
- `proofs/koide_relations.py` - Derives Koide Q and θ from J_min
- Mass ratio predictions (m_p/m_e, neutron-proton difference) to preregistrations
- Koide θ = 2/9 as independent prediction (0.0025% error)
- Cross-domain validation table in README
- Extensions (In Development) section in README
- Justification for why 2N = N! specifically

### Changed
- Updated CONFIDENCE_TIERS.md with Koide predictions
- Enhanced predictions_v1.md with additional confirmed predictions

---

## [1.0.0] - 2025-12-05

### Added
- Initial public release
- Core theorems: N=3 selection, Hessian eigenvalue ratio, correlation floor, bridge derivation
- Proof scripts for all Tier 1 and Tier 2 claims
- Preregistered predictions including neutrino hierarchy
- CONFIDENCE_TIERS.md for epistemological transparency

### Predictions Included
| Prediction | Formula | Error |
|------------|---------|-------|
| α⁻¹ | √3(8π² + 1/2π) | 0.002% |
| sin²θ_W | J_min × ln(2) | 0.07% |
| Tsirelson | 4√(NJ_min/2) | exact |
| Quantum amplification | 1/J_min | exact |

---

## Versioning Policy

- **Major versions**: New theoretical predictions or significant framework extensions
- **Minor versions**: Additional proofs, improved derivations, documentation
- **Patch versions**: Bug fixes, typo corrections

All predictions are timestamped via git commits. No post-hoc editing of predictions.

---

*This changelog establishes scientific priority through transparent version history.*
