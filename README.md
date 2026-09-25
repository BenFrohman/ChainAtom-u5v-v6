# Chain atom u^5 v + v^6

Author: Benjamin Stanley Frohman (@BenFrohman).
Copyright (c) 2026 Benjamin Stanley Frohman. Apache-2.0.

Atomic block of the locked sextic

    F = (x0^5 x3 + x3^6) + (x1^5 x4 + x4^6) + (x2^5 x5 + x5^6).

## The singularity

    W = u^5 v + v^6.

Two variables. Isolated plane-curve singularity at the origin.
A = [[5,1],[0,6]], det A = 30 = Milnor number.
Weights q_u = q_v = 1/6. Central charge of one block ĉ = 4/3.
Three disjoint blocks: μ(F) = 30^3 = 27000, ĉ(F) = 4.

Transpose block (one summand of F^T):

    W^T = u^5 + u v^6

weights (3,2), degree 15, same ĉ = 4/3.

## What applies

- Fan–Shen: FJRW quantum ring of X^p + X Y^q ≃ Milnor ring of the dual.
- Guéré: chain FJRW Hodge integrals.
- 2-variable HMS: D_sg(W) vs Fukaya–Seidel(W^T).
- Ebeling–Gusein-Zade monodromy zeta of an invertible chain vs transpose.

## What does not apply

Ebeling–Takahashi Dolgachev ↔ Gabrielov is three variables.
Suspension W + z^2 is a different germ.
Heterotic c=9 is CY3, not this atom.

## What this is not

Not a fourfold. Not a class in Hdg^2(V(F)). Not Term A. Not Term B.
Sisters: BenFrohman/DerivedCategories, BenFrohman/HODGE,
BenFrohman/NoetherLefschetz.
