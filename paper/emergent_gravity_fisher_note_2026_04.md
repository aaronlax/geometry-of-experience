# Emergent Gravity from the Fisher Information Metric on Shape Space

**Author:** Aaron Lax
**Date:** 2026-04-08

**Purpose:** Public timestamp for the identification of gravitational dynamics with the Fisher information metric on N=3 shape space, including derivations of Newton's constant, the MOND acceleration scale, and the cosmological constant. This is a prior-art note, not a full derivation paper.

---

## Claim

The Fisher information metric \(g^F_{ij}\) on N=3 shape space generates gravitational dynamics. The Raychaudhuri expansion scalar, Newton's constant, the MOND acceleration scale, and the cosmological constant all follow from the geometric properties of \(g^F_{ij}\) and a single shape-space parameter \(J_{\min} = 1/3\).

---

## Core Identification

The expansion scalar \(\theta\) in the Raychaudhuri equation is identified with the rate of change of the log-determinant of the Fisher metric:

\[
\theta \;\propto\; \frac{d}{d\tau} \log \sqrt{\det g^F_{ij}}.
\]

The Raychaudhuri equation governs the convergence/divergence of geodesic congruences:

\[
\frac{d\theta}{d\tau} = -\frac{1}{3}\theta^2 - \sigma_{\mu\nu}\sigma^{\mu\nu} + \omega_{\mu\nu}\omega^{\mu\nu} - R_{\mu\nu} u^\mu u^\nu.
\]

The identification maps Fisher metric degeneracy (loss of statistical distinguishability between configurations) to geodesic focusing (gravitational attraction).

---

## Newton's Constant

The N=3 Hessian of the shape potential on shape space has a minimal eigenvalue ratio:

\[
J_{\min} = \frac{1}{3}.
\]

Newton's constant is determined by this geometric correlation floor:

\[
G = J_{\min}^2 \times \frac{\hbar c}{m_P^2} = \frac{1}{9}\, G_{\text{Planck}}.
\]

The factor \(1/9\) is not a fit parameter. It is the square of the minimal eigenvalue ratio of the N=3 shape space Hessian.

---

## MOND Acceleration Scale

The Fisher metric degenerates when configurations become statistically indistinguishable. This defines a natural acceleration scale below which the Newtonian approximation breaks down.

Define the shape-space degeneracy ratio:

\[
\frac{\eta}{J_{\min}} = \frac{1/15}{1/3} = \frac{1}{5},
\]

where \(\eta = 1/15\) is the N=3 shape-space volume element normalization. The MOND acceleration scale is:

\[
a_0 = \frac{c^2}{5} \sqrt{\frac{\Lambda}{3}}.
\]

Numerically, using \(\Lambda\) from the derivation below:

\[
a_0 \approx 1.09 \times 10^{-10} \;\text{m/s}^2.
\]

This matches the observed MOND scale (Milgrom 1983: \(a_0 \approx 1.2 \times 10^{-10}\) m/s\(^2\)).

In the deep-MOND regime (\(g_N \ll a_0\)):

\[
g_{\text{eff}} = \sqrt{g_N \, a_0}.
\]

---

## Cosmological Constant

The cosmological constant follows from the same \(J_{\min}\):

\[
\Lambda = 3 H_0^2 (1 - J_{\min}) = 3 H_0^2 \times \frac{2}{3} = 2 H_0^2.
\]

The factor \((1 - J_{\min}) = 2/3\) is the fraction of shape-space degrees of freedom not captured by the minimal eigenvalue sector. This simultaneously determines the vacuum energy fraction and the action split.

Self-consistency: no additional parameters are introduced. The same \(J_{\min} = 1/3\) determines \(G\), \(a_0\), and \(\Lambda\).

---

## Testable Predictions

| Prediction | Value | Comparison |
|-----------|-------|------------|
| MOND acceleration scale | \(a_0 = 1.09 \times 10^{-10}\) m/s\(^2\) | Observed: \(\approx 1.2 \times 10^{-10}\) m/s\(^2\) |
| Cosmological constant ratio | \(\Lambda / H_0^2 = 2\) | From \((1 - J_{\min}) = 2/3\) |
| Dark matter particles | Null (no direct detection) | Geometric origin replaces particle dark matter |

---

## Relationship to Other Results

- **Bell correlations** (see `bell_evasion_hopf_linking_note_2026_04.md`): The Hopf fiber structure on the same N=3 shape space accounts for quantum correlations. Gravity and quantum correlations arise from different geometric properties (Fisher metric vs. fiber linking) of the same underlying space.
- **Pointer directions** (see `measurement_algebra_factorization_note_2026_04.md`): Measurement structure is algebraic. Gravity is metric. These are independent layers of the geometry.
- **Constants program** (see `emergence_of_constants.md`): \(J_{\min}\), \(\eta\), and related constants are derived from N=3 shape space geometry with zero free parameters.

---

## Status

**PROPOSED** (heuristic identification chain, not rigorous proof).

The Fisher metric \(\to\) Raychaudhuri identification is structural and motivated, but the full derivation of Einstein's field equations from this identification remains an open gap. The numerical agreements (\(a_0\), \(\Lambda\)) are suggestive but the derivation chain has steps that are identifications rather than theorems.

### What is closed

- \(J_{\min} = 1/3\) from N=3 Hessian eigenvalue analysis (derived, verified)
- \(\eta = 1/15\) from shape-space volume normalization (derived, verified)
- \(a_0\) numerical value from \(J_{\min}\) and \(\eta\) (computed, matches observation)
- \(\Lambda / H_0^2 = 2\) from \((1 - J_{\min})\) (computed)
- Self-consistency: single parameter \(J_{\min}\) determines all three quantities

### What is open

- Full derivation of Einstein field equations from Fisher metric on shape space
- Rigorous proof that Raychaudhuri expansion scalar equals Fisher log-determinant rate
- Extension to N>3 (higher particle number shape spaces)
- Post-Newtonian corrections and strong-field regime
- Relationship between Fisher metric degeneracy and horizon thermodynamics
