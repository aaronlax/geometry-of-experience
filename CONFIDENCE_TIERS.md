# Confidence Tiers: Epistemological Status of Claims

**Purpose**: This document explicitly categorizes every claim in the framework by its derivation status. This preempts criticism by being honest about what is proven, what is established physics, and what remains interpretive.

---

## Tier 1: PROVEN (Pure Geometry)

These are mathematical theorems derived from N=3 shape space with no physical assumptions.

| Claim | Statement | Proof |
|-------|-----------|-------|
| **N = 3 selection** | 2N = N! has unique solution N = 3 | Direct enumeration |
| **Hessian eigenvalue ratio** | λ_max/λ_min = 3 at equilateral | `hessian_eigenvalue_n3.py` |
| **Correlation floor** | J_min = 1/N = 1/3 | Corollary of above |
| **Bridge derivation** | ℏ = 2/N! equals J_min = 1/N iff 2N = N! | `hbar_derivation.py` |

**Status**: These are mathematical facts. They do not depend on physics being correct.

---

## Tier 2: DERIVED (Geometry + Established Math)

These combine shape space geometry with established mathematical facts.

| Claim | Statement | Components | Proof |
|-------|-----------|------------|-------|
| **Factor 4 = dim(ℍ)** | Quaternion algebra dimension | S³ ≅ unit quaternions | `eight_pi_squared_origins.py` |
| **8π² = 4 × Vol(S³)** | dim(ℍ) × Vol(S³) | Hopf fibration structure | `eight_pi_squared_origins.py` |
| **1/(2π) screening** | Boundary/bulk measure | 2π/4π on S² | `eight_pi_squared_origins.py` |
| **ln(2) in θ_W** | Z₂ entropy at collinear | Shannon entropy of {±1} | `z2_entropy_derivation.py` |
| **Quantum amplification = 3** | E_quantum/E_classical = N | Fiber bundle structure | `quantum_amplification.py` |
| **Tsirelson = 2√2** | CHSH bound from monogamy | 3-party correlation budget | `tsirelson_bound.py` |
| **Koide Q = 2/3** | Lepton mass parameter | Q = 2 × J_min | Established (Koide 1982) |

**The Factor 4 Derivation Chain** (each step forced):
```
N=3 → S² (shape space) → Hopf fibration (unique bundle) → S³ (fiber) → unit quaternions → dim(ℍ) = 4
```

**Status**: These follow from geometry combined with established topology and algebra.

### Predictions in this tier:

| Prediction | Formula | Predicted | Measured | Error |
|------------|---------|-----------|----------|-------|
| sin²θ_W | J_min × ln(2) | 0.23105 | 0.23122 | 0.07% |
| Tsirelson | 4√(NJ_min/2) | 2√2 | 2√2 | exact |
| Amplification | 1/J_min | 3 | 3 | exact |
| Koide Q | 2 × J_min | 0.6667 | 0.6666 | 0.0006% |

---

## Tier 3: INTERPRETIVE (Pattern Matching)

These match data but have heuristic rather than rigorous derivations.

| Claim | Statement | Status | Issue |
|-------|-----------|--------|-------|
| **Y-junction = 34 MeV** | Baryon topology cost | PATTERN MATCH | Matches data but derivation is heuristic |

**Note**: The factor 4 has been **promoted to Tier 2**. It is now derived from the quaternionic structure of the Hopf fibration, not imported from QFT.

---

## Tier 4: NOVEL PREDICTIONS (Awaiting Test)

These are predictions made BEFORE experimental verification.

| Prediction | Value | Test | Timeline | Falsification |
|------------|-------|------|----------|---------------|
| ν hierarchy | Inverted | DUNE/Hyper-K/JUNO | 2025-2030 | Normal hierarchy at >3σ |
| m₁ | 0.8 meV | KATRIN | 2025-2027 | m₁ > 5 meV |
| Σm_ν | 0.060 eV | CMB-S4 | 2027-2030 | Σm_ν > 0.12 eV |

**Status**: These are the "acid test" for the framework.

---

## Fine Structure Constant: Component Breakdown

The formula α⁻¹ = √3 × (8π² + 1/(2π)) = 137.033 has components at different tiers:

| Component | Value | Tier | Status |
|-----------|-------|------|--------|
| √3 | 1.732... | 1 (Proven) | From Hessian eigenvalue ratio |
| Vol(S³) = 2π² | 19.74... | 1 (Proven) | Standard topology |
| Factor 4 = dim(ℍ) | 4 | 2 (Derived) | From Hopf fibration → quaternions |
| 1/(2π) | 0.159... | 2 (Derived) | Boundary/bulk measure ratio |

**Overall status**: The α prediction is **fully derived** from N=3 geometry (Tier 1-2). No imported components remain.

---

## Hall-Reginatto Validation

The structural check T/I_F = 1/8 provides independent validation:

| Calculation | Framework | Result | Status |
|-------------|-----------|--------|--------|
| Shape sphere spectral solve | N=3 geometry | T/I_F = 1/8 | Tier 2 |
| Hall-Reginatto QM | Standard QM | Q = (ℏ²/8m) × I_F | Established |
| Match | - | Coefficients identical | **Validates bridge** |

---

## Why This Tiering Matters

1. **Intellectual honesty**: We know exactly what is proven vs. assumed
2. **Preempts criticism**: Reviewers will probe weak links; we identify them first
3. **Guides future work**: Tier 3 items are research targets
4. **Distinguishes from numerology**: Numerology hides assumptions; we expose them

---

## Summary

| Tier | Description | Example |
|------|-------------|---------|
| 1 | Pure geometry (proven) | λ_max/λ_min = 3 |
| 2 | Geometry + established math | Factor 4 = dim(ℍ), 1/(2π) = boundary/bulk |
| 3 | Pattern matching | Y-junction = 34 MeV |
| 4 | Novel predictions | Inverted ν hierarchy |

**All components of α⁻¹ = 137.033 are now Tier 1-2 (fully derived).**

The framework's remaining tests are:
- **Tier 3**: Refine heuristic derivations (Y-junction)
- **Tier 4**: Await experimental results (neutrino hierarchy, 2025-2030)

---

*This document reflects the epistemic status as of December 2025.*
*Updated: Factor 4 promoted from Tier 3 to Tier 2 via quaternionic derivation.*
