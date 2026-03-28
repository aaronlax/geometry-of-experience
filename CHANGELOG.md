# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

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
