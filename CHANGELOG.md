# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased]

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
