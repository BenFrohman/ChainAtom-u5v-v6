# Teaching the atom

Author: Benjamin Stanley Frohman (@BenFrohman).
Copyright (c) 2026 Benjamin Stanley Frohman. Apache-2.0.

The object:

    W(u,v) = u^5 v + v^6
    μ = 30, ĉ = 4/3
    W^T(u,v) = u^5 + u v^6

## To a ten-year-old

Imagine a tiny dent at the origin of a sheet of paper. The dent is made by
the equation W = 0. It is a local picture, like looking at one bump on a
road with a magnifying glass. The number 30 counts how complicated that
bump is. The flipped equation W^T is a different bump that mathematicians
use as a mirror of the first bump. Three copies of the first bump glued
side-by-side make the big sextic fourfold. Studying one bump is not the
same as studying the whole fourfold, just like studying one brick is not
studying the house.

## To a lay adult

A germ is the local analytic shape of an equation near a point — here the
origin. W is a plane-curve singularity: two variables, isolated critical
point, Milnor number 30 (dimension of the Jacobian algebra). Its Berglund–Hübsch
transpose W^T is the exponent-matrix flip, another two-variable germ with
the same central charge 4/3. The global variety X = V(F) is a smooth
Calabi–Yau fourfold built as the Thom–Sebastiani sum of three copies of W.
The atom is a *local ingredient* of F. Programs that apply to two-variable
chain singularities (Fan–Shen, 2-var HMS, monodromy zeta) apply to W.
They do not automatically become facts about Hodge classes on X.

A *different germ* means a different local equation. Adding a square,
W + z^2, changes the number of variables and the type of singularity
(curve → surface). Theorems written for three-variable invertibles
(Ebeling–Takahashi Dolgachev/Gabrielov) apply to that suspension, not
to W and not to V(F).

## To a professional

W is the invertible chain atom of type X^5 Y + Y^6. Isolated hypersurface
singularity in (C^2, 0). Jacobian algebra dimension μ = det A = 30.
Quasihomogeneous weights (1,1)/6, ĉ = Σ(1−2q_i) = 4/3.
BHK transpose is the chain of opposite type X^5 + X Y^6, weights (3,2),
degree 15, same ĉ. Thom–Sebastiani: F = W(x0,x3) ⊕ W(x1,x4) ⊕ W(x2,x5),
so μ(F) = 30^3 and ĉ(F) = 4, matching the CY4 charge of X = V(F) ⊂ P^5.

Applicable: Fan–Shen isomorphism of FJRW quantum ring of the chain with
the Milnor ring of the dual; Guéré chain FJRW integrals; Habermann–Smith
2-variable HMS D_sg(W) ≃ FS(W^T); Ebeling–Gusein-Zade zeta of an
invertible chain versus its transpose.

Not applicable as written: Ebeling–Takahashi strange duality (3-var),
heterotic Gepner c=9 (CY3), Fourier–Mukai partnership of fourfolds,
rational Hodge on H^4 ∩ H^{2,2}. The suspension W + z^2 is a different
germ in (C^3, 0). Passing to the projective hypersurface V(F) is a
different global object. None of these substitutions fills Term A or Term B.
