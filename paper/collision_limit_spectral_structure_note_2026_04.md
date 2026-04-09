# Spectral Structure on the N=3 Shape-Space Cone: Collision-Limit Transport and the KZ Connection

**Author:** Aaron Lax
**Date:** 2026-04-08

**Scope.** This note records the theoretical framework and key results from an independent investigation into whether hydrogenic spectral structure emerges from the geometry of the N=3 shape-space cone. It is distinct from the scalar variety / central-configuration program (a collaboration with Julian Barbour and Maria Lourenço) and from any collaboration results.

---

## 1. Introduction

The quantum mechanics of N=3 particles can be formulated on the McGehee cone over shape space. The central question: does hydrogenic spectral structure — $n^2$ degeneracy and $1/n^2$ energy levels — emerge from the geometry of this cone?

The route explored here is **collision-limit transport**: the geometry of the vector bundle carried by the permutation-doublet fiber over the collision-excised shape sphere, and the non-Abelian connection forced on it in the triple-collision limit. This is a fundamentally different approach from the scalar/Abelian programs that study central configurations or the potential on shape space directly.

---

## 2. The McGehee Cone

The configuration space of N=3 particles, after center-of-mass removal, carries a natural cone metric:

$$
ds^2 = d\rho^2 + \rho^2 \, ds^2_{S^2}
$$

where $\rho = \sqrt{I_{\mathrm{cm}}}$ is the scale variable (square root of the center-of-mass moment of inertia) and $S^2$ is the shape sphere.

The Hamiltonian on the cone:

$$
H = -\frac{\hbar^2}{2\mu}\left[\partial_\rho^2 + \frac{2}{\rho}\partial_\rho + \frac{1}{\rho^2}\Delta_{S^2}\right] + \frac{1}{\rho}U(\Omega)
$$

where $U(\Omega)$ is the Coulomb potential evaluated at unit moment of inertia ($\rho = 1$).

**Separation into angular + radial problems.** Expanding in angular eigenstates $\psi_n(\Omega)$ of the angular operator:

$$
\left[-\kappa \, \Delta_{S^2} + V_E(\Omega)\right] \psi_n = \lambda_n \, \psi_n
$$

the diagonal radial approximation gives hydrogen-like form only if the effective Coulomb charge $U_n$ is constant across channels.

**The central obstruction.** For N=3 Coulomb, $U_n$ varies by a factor of approximately $2\times$ across angular channels, and off-diagonal coupling is 30--85% of diagonal (not perturbative). The diagonal radial approximation fails qualitatively.

---

## 3. Closed Routes (Abelian Sectors)

The following scalar/Abelian routes have been tested systematically and produce null results for hydrogen:

1. **Raw Coulomb on $S^2$** — free-sphere Laplacian perturbation only. Effective charge varies across channels.
2. **$k=0$ monopole sector** — varying $U_n$, strong off-diagonal coupling (30--85% of diagonal).
3. **$k=1$ monopole sector** — half-integer $j_{\mathrm{eff}}$, but coupling worse than $k=0$.
4. **$S_2$ parity decomposition** — block-diagonal by parity, but primary obstruction persists in each block.
5. **Aligned $Z_{\mathrm{eff}}$ rescue** — closed.
6. **$S_3$ $E$-sector projection** — corrected group-theoretic basis; $E$-projection WORSENS alignment vs unprojected control, charge spread $2.4$--$2.9\times$.

**All Abelian routes closed negative.** The obstruction is structural: angular Coulomb anisotropy on $S^2$ is irreducible in scalar sectors.

---

## 4. The Non-Abelian KZ Connection

The collision-excised shape sphere $S^2 \setminus \{3 \text{ punctures}\}$ carries a rank-2 vector bundle from the $E$-doublet of the $S_3$ permutation group. Under a Fuchsian regularity assumption (proved separately), the Berry connection on this bundle in the triple-collision limit is forced to be a **Knizhnik-Zamolodchikov connection at level $k=3$**.

Key structure:

| Component | Value |
|---|---|
| Base space | $S^2$ with 3 binary-collision punctures |
| Fiber | 2D complex (Fibonacci fusion space at $k=3$) |
| KZ residues | $\Omega_0 = \mathrm{diag}(-2, -1)$, normalized by $1/(k + h^\vee) = 1/5$ |
| F-matrix (Fibonacci) | $F = \begin{pmatrix} \varphi^{-1} & \sqrt{\varphi^{-1}} \\ \sqrt{\varphi^{-1}} & -\varphi^{-1} \end{pmatrix}$ where $\varphi = \tfrac{1+\sqrt{5}}{2}$ |
| Monodromy eigenphases | $(-144°, -72°)$, matching Fibonacci anyon exchange statistics |

The connection is:

$$
\nabla = d + \sum_{a=1}^{3} \frac{\Omega_a}{z - z_a} dz
$$

where $z_a$ are the puncture positions in the uniformizing coordinate and $\Omega_a$ are the KZ residue matrices related by the F-matrix conjugation.

---

## 5. Local Puncture Analysis

Near a binary-collision puncture, the covariant Laplacian on the KZ bundle gives a local indicial equation:

$$
\nu = |m + R|
$$

where $m \in \mathbb{Z}$ is the angular Fourier mode and $R$ is the KZ residue eigenvalue.

For $m = 0$:

$$
\nu_1 = \frac{2}{5} = 0.400, \qquad \nu_2 = \frac{1}{5} = 0.200
$$

Both $\nu < 1$, placing the reduced radial operator in the **limit-circle regime**. $L^2$ alone does not select the branch — the self-adjoint extension choice is load-bearing.

This contrasts with the Berry connection (where $\nu = 1$, limit-point, Friedrichs extension unique). The KZ connection opens a degree of freedom that the Abelian problem does not have.

---

## 6. Verified Stage 2A: KZ Pullback

The KZ connection has been pulled back to the physical shape sphere with physical masses (proton:electron mass ratio $= 1836:1$). Verified results:

- Physical punctures located at known positions on $S^2$
- Mobius uniformization maps punctures to $\{0, 1, \infty\}$
- Loop holonomies reproduce target KZ eigenphases
- Two-puncture noncommutativity: $\|[U_{C_{12}}, U_{C_{01}}]\| \approx 0.95$ (genuinely non-Abelian)
- KZ connection narrows effective-charge spread by $\sim 18.5\%$ relative to scalar baseline

---

## 7. Open Problem: Stage 2B

The global angular eigenvalue problem on the punctured sphere with the non-Abelian KZ connection remains open. Specifically:

1. **Full covariant Laplacian** $D^\dagger D + \rho V_E$ on $S^2$ with KZ link variables
2. **Domain regularization** at collision punctures (Frobenius-admissible boundary conditions)
3. **Self-adjoint extension selection** in limit-circle channels
4. **Global spectral computation**

---

## 8. Hidden-Symmetry Matching Framework

If hydrogenic structure does not live in the finite-$\rho$ operator directly, it may live in the collision-limit carrier $V_{\mathrm{pre}}$ and matching data $M_a : V_{\mathrm{pre}} \to V_{\mathrm{phys},a}$ at each puncture. The dressed puncture operators $M_a D_a M_a^{-1}$ may fail to commute, protecting hydrogenic observables after projection to the physical branch.

This framework requires:

1. Precise definition of $V_{\mathrm{pre}}$ (pre-physical fiber data, not $S^2$ eigenstates)
2. Physics that fixes $M_a$ at each puncture
3. At least one $M_a$-dependent observable

Status: design/theorem stage. Cannot proceed computationally until the global angular operator (Stage 2B) is resolved.

---

## Status Summary

| Component | Status |
|---|---|
| Closed Abelian routes | **[verified]** All tested scalar/Abelian sectors produce null for hydrogen |
| KZ pullback (Stage 2A) | **[verified]** Geometric object matches target monodromies |
| Local puncture law | **[verified]** $\nu = \|m + R\|$ in unitary gauge |
| Charge spread narrowing | **[verified]** KZ reduces spread by $\sim 18.5\%$ |
| Global angular eigenvalue (Stage 2B) | **[open]** |
| Hidden-symmetry matching | **[design only]** |
