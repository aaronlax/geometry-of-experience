# Bell Inequality Violations from Hopf Linking on N=3 Shape Space

**Author:** Aaron Lax
**Date:** 2026-04-08

**Purpose:** Public timestamp for the result that Bell inequality violations arise from the linking number of Hopf fibers on N=3 shape space, violating Outcome Independence while preserving Parameter Independence. This is a prior-art note, not a full derivation paper.

---

## Claim

The Hopf fibration on N=3 shape space accounts for Bell inequality violations without non-local communication. The mechanism is topological linking of fibers over distinct base points, which creates irreducible bipartite correlations that cannot be factorized into local marginals.

---

## Jarrett-Shimony Decomposition

Bell factorizability requires:

\[
P(A, B \mid a, b, \lambda) = P(A \mid a, \lambda) \cdot P(B \mid b, \lambda).
\]

This decomposes into two independent conditions (Jarrett 1984, Shimony 1986):

- **Parameter Independence (PI):** \(P(A \mid a, b, \lambda) = P(A \mid a, \lambda)\). Alice's marginal is independent of Bob's setting choice.
- **Outcome Independence (OI):** \(P(A \mid a, B, b, \lambda) = P(A \mid a, \lambda)\). Alice's outcome probability is independent of Bob's outcome, given the hidden variable.

Bell factorizability holds if and only if both PI and OI hold.

---

## RIG Classification

| Condition | Status | Reason |
|-----------|--------|--------|
| **Parameter Independence** | SATISFIED | Correlations are topological, not dynamical. No signal propagates between fibers. |
| **Outcome Independence** | VIOLATED | Hopf linking creates irreducible joint correlations that cannot be factorized. |
| **Measurement Independence** | ASSUMED | No coupling mechanism between \(\lambda\) and measurement settings has been derived. |

This places RIG in the same cell as standard QM in the Jarrett-Shimony table: PI-yes, OI-no.

For comparison:

| Framework | PI | OI |
|-----------|----|----|
| Standard QM | Yes | No |
| RIG (Hopf linking) | Yes | No |
| Bohmian mechanics | No | Yes |
| Superdeterminism | Yes | Yes (MI violated instead) |

---

## Why Outcome Independence Fails

The linking number of two Hopf fibers \(\gamma_A\) and \(\gamma_B\) over distinct base points on \(S^2\) is given by the Gauss integral:

\[
\mathrm{Lk}(\gamma_A, \gamma_B) = \frac{1}{4\pi} \oint_{\gamma_A} \oint_{\gamma_B} \frac{(\mathbf{r}_1 - \mathbf{r}_2)}{|\mathbf{r}_1 - \mathbf{r}_2|^3} \cdot (d\mathbf{r}_1 \times d\mathbf{r}_2).
\]

Key properties of this invariant:

1. **Irreducibly bipartite.** The linking number is a property of the pair \((\gamma_A, \gamma_B)\). It cannot be decomposed into a product of single-fiber invariants. There is no function \(f(\gamma_A) \cdot g(\gamma_B)\) that reproduces \(\mathrm{Lk}\).

2. **Topological.** The linking number is invariant under continuous deformations of the fibers that do not pass one through the other. It depends only on the homotopy class of the pair.

3. **Non-signaling.** The linking number is a static geometric property. No dynamical process is required to establish or maintain it. Deforming \(\gamma_A\) alone (without crossing \(\gamma_B\)) does not change \(\mathrm{Lk}\), so Alice cannot signal to Bob by local operations.

Property 1 is why OI fails: the joint probability \(P(A, B \mid a, b, \lambda)\) inherits the irreducible bipartite structure of the linking number and cannot factorize.

Property 3 is why PI holds: the linking number is insensitive to local deformations of either fiber alone, so the marginal \(P(A \mid a, \lambda)\) is independent of Bob's setting \(b\).

---

## Physical Interpretation

"Spooky action at a distance" is the shadow of Hopf fiber linking projected onto the base manifold \(S^2\).

The base manifold sees correlated outcomes at spacelike separation and, lacking access to the fiber structure, interprets these as requiring non-local communication. From the total space \(S^3\), the correlations are geometric: the fibers are linked, and this linking is a topological fact about \(S^3\), not a dynamical process.

No signal is sent. The fiber topology makes outcomes irreducibly joint.

---

## Relationship to Other Results

- **Pointer directions** (see `measurement_algebra_factorization_note_2026_04.md`): The Kraus support graph fixes where collapse projects. The Hopf linking explains why joint outcomes across subsystems are correlated.
- **Born rule**: Metric compatibility on shape space determines outcome weights. Linking determines outcome correlations.

These are independent structural results that together constitute the measurement theory.

---

## Status

**DERIVED** (85% confidence, 2026-03-20).

The Jarrett-Shimony classification is clean: PI from non-signaling topology, OI violation from irreducible linking. The Gauss linking integral formulation is standard differential topology.

### What is closed

- Hopf fiber linking number is irreducibly bipartite (standard result)
- PI satisfaction follows from topological invariance under local deformations
- OI violation follows from non-factorizability of the linking number
- Classification matches standard QM in the Jarrett-Shimony table

### What is open

- Quantitative derivation of the Tsirelson bound \(2\sqrt{2}\) from the linking integral
- Explicit computation of \(P(A, B \mid a, b, \lambda)\) from the Hopf fiber geometry
- Extension beyond N=3 (higher linking invariants for N>3 shape spaces)
- Measurement Independence: no derived mechanism for or against \(\lambda\)-setting coupling
