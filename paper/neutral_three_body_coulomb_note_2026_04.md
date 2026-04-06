# Neutral Three-Body Coulomb Critical Shapes on the Preshape Sphere

**Date:** 2026-04-06

**Purpose:** Public timestamp for a clean `N=3` baseline in the Coulomb setting. This note records the pairwise neutral-Coulomb classification on the preshape sphere. It is not a full many-body or hydrogen derivation.

---

## Claim

For the normalized raw Coulomb potential on the three-body preshape sphere,

\[
\widehat U(x)=\frac{1}{\lVert q\rVert_2}\sum_{1\le i<j\le 3}\frac{q_iq_j}{r_{ij}},
\qquad
\sum_i m_i x_i=0,
\qquad
\sum_i m_i|x_i|^2=1,
\qquad
\sum_i q_i=0,
\]

if all three charges are nonzero, then there are no noncollinear critical shapes.

What remains are collinear critical shapes.

---

## Why the Newton/Lagrange Branch Disappears

Write

\[
c_{12}=q_1q_2,\qquad c_{23}=q_2q_3,\qquad c_{31}=q_3q_1.
\]

At a noncollinear triangle, the constrained critical-point equations in mutual distances give

\[
\frac{c_{ij}}{r_{ij}^3}=-2\lambda m_im_j
\qquad
\text{for all three pairs }(i,j).
\]

Since `m_i m_j > 0` and `r_ij > 0`, the right-hand side has the same sign for all three pairs.
Therefore `c_{12}, c_{23}, c_{31}` must all have the same sign at any noncollinear interior critical point.

But for a genuinely neutral triple with all charges nonzero, one charge has the opposite sign from the other two. So one pair product is positive and two are negative. The three `c_{ij}` cannot have a common sign.

Therefore the noncollinear branch is excluded.

---

## Equal-Mass Prototype

Take

\[
m_1=m_2=m_3=\frac13,
\qquad
q=(2,-1,-1).
\]

A surviving noncollision critical shape is the symmetric collinear one with the positive charge in the middle:

\[
x_1=(0,0,0),
\qquad
x_2=\left(-\sqrt{\frac32},0,0\right),
\qquad
x_3=\left(\sqrt{\frac32},0,0\right).
\]

Then

\[
r_{+,-}=\sqrt{\frac32},
\qquad
r_{-,-}=\sqrt{6},
\qquad
\widehat U=-\frac76.
\]

The structural sign behavior is:

- the like-sign `(-,-)` collision is repulsive, so `\widehat U \to +\infty`
- the opposite-sign `(+,-)` collisions are attractive, so `\widehat U \to -\infty`

So the neutral Coulomb landscape differs qualitatively from the Newtonian one.

---

## Interpretation

For the normalized Newton potential on `N=3` shape space, the standard critical shapes are the Euler collinear branch and the Lagrange equilateral branch.

For the neutral pairwise Coulomb problem, the equilateral/noncollinear branch disappears entirely. The surviving critical set is collinear.

This makes the neutral pairwise electric sector much poorer geometrically than the Newtonian one at the first nontrivial `N=3` level.

---

## Status

This note records a stable baseline result:

- pairwise neutral Coulomb on the preshape sphere does **not** support a noncollinear critical branch
- the first surviving noncollision prototype is collinear

That baseline is useful because it cleanly separates what the raw pairwise sector can do from what any additional collective geometric term would have to do.
