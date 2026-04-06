# Pairwise vs Collective Structure on `N=3` Shape Space

**Date:** 2026-04-06

**Purpose:** Public timestamp for a simple structural split on the three-body shape sphere. This note distinguishes observables built only from pair distances from observables that require full triangle data.

---

## Claim

On `N=3` shape space, there is a clean structural split:

1. **Pairwise observables** depend only on the mutual distances `r_{12}, r_{23}, r_{31}`.
2. **Collective observables** require the full triangle invariant, in particular the oriented area `A`.

The split matters because pairwise observables control puncture-level / collision structure, while collective observables are the first place genuinely oriented triangle information can enter.

---

## Definitions

A pairwise observable has the form

\[
O_{\mathrm{pair}} = f(r_{12},r_{23},r_{31}).
\]

A collective observable has the form

\[
O_{\mathrm{coll}} = g(r_{12},r_{23},r_{31},A)
\qquad\text{with}\qquad
\frac{\partial g}{\partial A}\neq 0.
\]

Here `A` is the oriented area of the triangle, equivalently the first non-pairwise shape invariant.

---

## Why This Split Matters

Pairwise data alone can see:

- binary collisions
- inverse-distance singularities
- collinear limits
- symmetry under relabeling of pairs

Pairwise data alone cannot distinguish the two triangle orientations, because it does not depend on the oriented area.

The first genuinely triangle-level information enters when the observable depends on `A`.

So:

- pairwise sector: radial / collision / boundary structure
- collective sector: oriented / interior / triangle-wide structure

---

## Immediate `N=3` Consequence

The raw neutral Coulomb sum is pairwise:

\[
\widehat U = \frac{1}{\lVert q\rVert_2}\sum_{i<j}\frac{q_iq_j}{r_{ij}}.
\]

It depends only on `r_{ij}`.

Therefore any geometric effect that genuinely depends on triangle orientation or interior triangular organization cannot come from this raw pairwise term alone.

This aligns with the neutral `N=3` Coulomb classification:

- the pairwise neutral Coulomb problem loses the noncollinear branch
- the remaining critical structure is collinear

---

## Programmatic Use

This split is not a full dynamical derivation. It is a classification tool.

It tells us where to look for different kinds of structure:

- if a phenomenon is already visible at the level of pair distances and collisions, it belongs to the pairwise sector
- if a phenomenon requires an intrinsically triangular or oriented effect, it must come from the collective sector

For `N=3`, this is the cleanest first distinction one can make before moving to more elaborate ansätze.
