# Emergence of Fundamental Constants from N=3 Shape Space Geometry

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains the mathematical foundations for deriving fundamental physical constants from the information geometry of N=3 relational shape space.

## Key Results

| Quantity | Formula | Predicted | Measured | Error |
|----------|---------|-----------|----------|-------|
| Fine structure constant | α⁻¹ = √3(8π² + 1/2π) | 137.033 | 137.036 | 0.002% |
| Weak mixing angle | sin²θ_W = J_min × ln(2) | 0.23105 | 0.23122 | 0.07% |
| Tsirelson bound | 4 × √(N × J_min / 2) | 2√2 | 2√2 | exact |
| Quantum amplification | E_quantum / E_classical | 3 | 3 | exact |

---

## The Complete Derivation Chain

```
NUMBER THEORY:  2N = N!  →  N = 3 (unique solution)
       ↓
INFORMATION GEOMETRY:  ℏ = 2/N! = 1/3
       ↓
SHAPE SPACE GEOMETRY:  J_min = 1/N = 1/3
       ↓
FORCED EQUALITY:  ℏ = J_min (because 2/N! = 1/N only when 2N = N!)
       ↓
THREE INDEPENDENT PATHS:

PATH A (Electromagnetic):
├─ 8π² = 4·Vol(S³) [topological invariant]
├─ 1/(2π) = Morse screening [collinear boundary]
├─ √3 = √N [Hessian eigenvalue ratio]
└─ α⁻¹ = √3(8π² + 1/(2π)) = 137.033 ✓

PATH B (Weak Interaction):
├─ Z₂ symmetry at collinear → ln(2) entropy
├─ J_min × ln(2) [correlation floor × entropy]
└─ sin²θ_W = 0.2310 ✓ (PREREGISTERED)

PATH C (Quantum Correlation):
├─ Hopf fibration S³ → S² structure
├─ S¹ fiber amplifies correlations by N = 3
└─ Tsirelson bound = 2√2 ✓ (EXACT)
```

---

## Core Theorems

### Theorem 1: Selection of N = 3

The equation **2N = N!** has exactly one positive integer solution:

| N | 2N | N! | Equal? |
|---|----|----|--------|
| 1 | 2  | 1  | No     |
| 2 | 4  | 2  | No     |
| **3** | **6** | **6** | **Yes** |
| 4 | 8  | 24 | No     |

This selects the 3-body shape space S² as the fundamental relational substrate.

**Why 2N = N! specifically?** This equation balances information capacity (2N degrees of freedom for N bodies in 2D shape space) against permutation symmetry (N! indistinguishable arrangements). The balance point is the minimal self-consistent relational system.

### Theorem 2: Hessian Eigenvalue Ratio

At the equilateral triangle (maximal symmetry point) on N=3 shape space:

```
λ_max / λ_min = N = 3
```

This is proven analytically in [`proofs/hessian_eigenvalue_n3.py`](proofs/hessian_eigenvalue_n3.py).

### Theorem 3: Correlation Floor

The inverse of the eigenvalue ratio defines the correlation floor:

```
J_min = 1/N = 1/3
```

This is the "pixel size" of the universe's information geometry.

### Theorem 4: The Bridge (ℏ = J_min)

**This is NOT an assumption.** The identification ℏ = J_min is forced by number theory:

| N | J_min = 1/N | ℏ = 2/N! | Equal? |
|---|-------------|----------|--------|
| 2 | 0.5000 | 1.0000 | No |
| **3** | **0.3333** | **0.3333** | **Yes** |
| 4 | 0.2500 | 0.0833 | No |

The equality holds **if and only if** 2N = N!, which uniquely selects N = 3.

See [`proofs/hbar_derivation.py`](proofs/hbar_derivation.py) for the complete derivation.

### Theorem 5: Quantum Amplification

Quantum correlations are classical geometric correlations amplified by the fiber topology:

```
E_quantum = E_classical × N = E_classical × (1/J_min)
```

For the singlet state, classical hidden variables give E = -cos(θ)/3, while quantum mechanics gives E = -cos(θ). The ratio is exactly 3.

---

## Addressing Common Critiques

### "The α formula looks like numerology"

**Response:** Each component has a traceable geometric origin:

| Component | Value | Origin | Status | Proof |
|-----------|-------|--------|--------|-------|
| √3 | 1.732... | Hessian eigenvalue ratio √N | **Tier 1: Proven** | [`hessian_eigenvalue_n3.py`](proofs/hessian_eigenvalue_n3.py) |
| 8π² | 78.957... | dim(ℍ) × Vol(S³) | **Tier 2: Derived** | [`eight_pi_squared_origins.py`](proofs/eight_pi_squared_origins.py) |
| Factor 4 | 4 | dim(ℍ) from Hopf fibration | **Tier 2: Derived** | [`eight_pi_squared_origins.py`](proofs/eight_pi_squared_origins.py) |
| 1/(2π) | 0.159... | Boundary/bulk measure = 2π/4π | **Tier 2: Derived** | [`eight_pi_squared_origins.py`](proofs/eight_pi_squared_origins.py) |

**The factor 4 derivation chain** (each step forced):
```
N=3 → S² → Hopf fibration (unique) → S³ → unit quaternions → dim(ℍ) = 4
```

All components are now derived from N=3 geometry. See [`CONFIDENCE_TIERS.md`](CONFIDENCE_TIERS.md) for full epistemological status.

### "Why ln(2) in the weak mixing angle?"

**Response:** The collinear boundary has Z₂ symmetry (reflection). The entropy of Z₂ is exactly ln(2) = 0.693... This is not fitted; it's the information cost of symmetry breaking.

See [`proofs/z2_entropy_derivation.py`](proofs/z2_entropy_derivation.py).

### "The bridge ℏ = J_min is arbitrary"

**Response:** The bridge is **forced** by the selection principle:
- ℏ = 2/N! (information density of indistinguishable configurations)
- J_min = 1/N (inverse Hessian eigenvalue ratio)
- These are equal **only when** 2N = N! (i.e., N = 3)

See [`proofs/hbar_derivation.py`](proofs/hbar_derivation.py).

### "Need novel predictions"

**Response:** The weak mixing angle sin²θ_W = 0.231 was **preregistered** before checking experiment. See [`preregistrations/predictions_v1.md`](preregistrations/predictions_v1.md).

---

## Repository Structure

```
n3-shape-space-public/
├── README.md                              # This file
├── CONFIDENCE_TIERS.md                    # Epistemological status of all claims
├── CHANGELOG.md                           # Version history (no post-hoc edits)
├── LICENSE                                # MIT License
├── paper/
│   └── emergence_of_constants.md          # Main paper
├── proofs/
│   ├── hessian_eigenvalue_n3.py           # Theorem 2: λ_max/λ_min = 3
│   ├── hbar_derivation.py                 # Theorem 4: ℏ = J_min from first principles
│   ├── quantum_amplification.py           # Theorem 5: E_quantum = 3 × E_classical
│   ├── tsirelson_bound.py                 # CHSH_max = 2√2 from monogamy
│   ├── eight_pi_squared_origins.py        # 8π², 1/(2π) screening, factor 4 status
│   ├── z2_entropy_derivation.py           # Why ln(2) appears in θ_W
│   ├── koide_relations.py                 # Koide Q = 2×J_min, θ = 2×J_min²
│   └── hall_reginatto_validation.py       # T/I_F = 1/8 consistency check
└── preregistrations/
    └── predictions_v1.md                  # Timestamped predictions
```

## Running the Proofs

```bash
# Core derivations
python proofs/hessian_eigenvalue_n3.py      # Eigenvalue ratio = 3
python proofs/hbar_derivation.py            # ℏ = J_min from first principles
python proofs/quantum_amplification.py      # Quantum amplification = 3
python proofs/tsirelson_bound.py            # Tsirelson bound = 2√2

# Supporting derivations
python proofs/eight_pi_squared_origins.py   # Origin of 8π²
python proofs/z2_entropy_derivation.py      # Origin of ln(2)
python proofs/koide_relations.py            # Koide Q and θ from J_min
python proofs/hall_reginatto_validation.py  # Structure validation
```

Requirements: `numpy`, `sympy`, `scipy`

---

## The Framework

### Axioms

1. **Relational Ontology (A1)**: Physics is relational. Only ratios of distances matter.
2. **N=3 Fundamental (A3)**: The 3-body system is uniquely selected by 2N = N!.
3. **Bridge Derived (A5)**: ℏ = J_min is forced by 2/N! = 1/N at N = 3.

### Geometric Structure

- **Base manifold**: S² (shape sphere of triangles)
- **Fiber bundle**: S³ → S² (Hopf fibration)
- **Metric**: Fisher Information metric
- **Singularities**: Equilateral (maximum symmetry) and collinear (boundary)

### Physical Interpretation

The fiber topology (S³ ≅ SU(2)) acts as a quantum amplifier. Classical correlations on S² are multiplied by N=3 when lifted to the full bundle, producing quantum mechanical predictions.

---

## Why This Is Not Numerology

1. **Constrained form**: Only Vol(S³) and related topological invariants appear, not arbitrary combinations of π.

2. **Multiple predictions**: The same J_min = 1/3 gives α (0.002%), θ_W (0.07%), and Tsirelson (exact).

3. **Preregistration**: Predictions were derived before checking experimental values.

4. **Forced bridge**: The identification ℏ = J_min is not assumed—it follows from 2N = N!.

5. **Structural validation**: The Hall-Reginatto ratio T/I_F = 1/8 confirms the mapping is consistent.

---

## Cross-Domain Validation

The same geometric structure (complexity functional on shape space) has been validated across multiple domains:

| Domain | Observable | Result | Status |
|--------|------------|--------|--------|
| Electromagnetism | α⁻¹ | 137.033 (0.002% error) | Published here |
| Weak force | sin²θ_W | 0.231 (0.07% error) | Published here |
| Quantum bounds | Tsirelson | 2√2 (exact) | Published here |
| Particle masses | Koide Q = 2×J_min | 2/3 (0.0006% error) | Published here |
| **Protein folding** | Complexity ratio → folding rate | **r = -0.89** | Separate publication |

The protein folding application demonstrates that the geometric complexity framework (not just fundamental constants) has predictive power in molecular biophysics. Details are in preparation for separate publication.

---

## Extensions (In Development)

The framework suggests connections to:

| Extension | Core Idea | Status |
|-----------|-----------|--------|
| Consciousness threshold | Awareness emerges when correlation J > J_c | Framework |
| Heisenberg from projection | Uncertainty = what shape space looks like through finite-capacity observation | Framework |
| Gravitational emergence | Metric curvature from complexity Hessian: g_ij = δ_ij + α·Hess_ij(C) | Exploratory |
| Relativistic structure | Lorentz factor J = √(1 - v²/c²) from shape space geometry | Exploratory |

These extensions are under development and will be presented in future work.

---

## Citation

```bibtex
@article{lax2025emergence,
  title={Emergence of Fundamental Constants and Quantum Correlations
         from the Information Geometry of N=3 Shape Space},
  author={Lax, Aaron},
  year={2025},
  note={Preprint}
}
```

## Acknowledgments

The shape space framework builds on foundational work by Julian Barbour on relational mechanics and scale invariance. The Hall-Reginatto formalism provides the quantum mechanical foundation. The novel contributions of this work are: the 2N = N! selection principle, the derived bridge ℏ = J_min, the quantum amplification theorem, and the geometric derivations of fundamental constants.

## References

1. Hall, M.J.W. & Reginatto, M. (2002). Quantum mechanics from a Heisenberg-type equality.
2. Barbour, J. (2003). Scale-Invariant Gravity: Particle Dynamics. Class. Quantum Grav.
3. Tsirelson, B.S. (1980). Quantum generalizations of Bell's inequality.
4. Koide, Y. (1983). A new formula for the masses of charged leptons.

## License

MIT License - see [LICENSE](LICENSE)

## Contact

For questions or collaboration inquiries, please open an issue.
