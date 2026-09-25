# What the atom is — three registers

Author: Benjamin Stanley Frohman (@BenFrohman).
Copyright (c) 2026 Benjamin Stanley Frohman. Apache-2.0.

The object:

    W = u^5 v + v^6
    W^T = u^5 + u v^6
    μ(W) = 30
    ĉ(W) = 4/3

Three copies of W, in six variables, assemble the locked sextic

    F = x0^5 x3 + x3^6 + x1^5 x4 + x4^6 + x2^5 x5 + x5^6.

## To a ten-year-old

Imagine a hill made of dough. Most of the hill is smooth. At one point
the dough pinches. That pinch is a *singularity*.

W is a recipe for a pinch that lives in a flat kitchen counter with only
two coordinates, called u and v. If you write the recipe on the counter,
the pinch happens only at the origin (u=0, v=0). Everywhere else nearby,
the dough is smooth.

The number 30 is a count of how complicated the pinch is. Think of it as
how many independent wiggles the nearby smooth slices of the dough have.
Bigger number, richer pinch. 30 is a specific count for this recipe, not
a guess.

W^T is the same kind of recipe with the exponents flipped. It is a
*mirror recipe*, not a different kitchen. The kitchen is still two
coordinates.

If you take three separate pinches like W and set them side by side in a
big six-coordinate room, you get the big shape F. That big shape is a
four-dimensional crystal sitting in five-dimensional projective space.
The small pinch W is a *building block* of that crystal. It is not the
crystal itself.

A miss in the Hodge problem would be a special shadow on the crystal
that no actual surface drawn on the crystal can make. W is a pinch in
two coordinates. It is not that shadow.

## To an adult who is not a mathematician

A *germ* is a tiny neighborhood of a point, plus the equation that cuts
out a shape there, with two germs counted as the same if they look the
same after a local change of coordinates. You are not looking at the
whole universe. You are looking at a spot under a microscope.

W = u^5 v + v^6 is an isolated plane-curve singularity. Isolated means:
zoom in close enough, and the only bad point is the origin. Plane-curve
means: the ambient space is two complex coordinates. The zero set is a
curve with a bad point.

The Milnor number μ = 30 is the dimension of the Jacobian algebra
C{u,v} / (∂W/∂u, ∂W/∂v). It is also the number of vanishing cycles in
the Milnor fiber: slice the equation at a tiny nonzero value, and the
smooth nearby fiber deformation-retracts onto a bouquet of 30 circles.
That is a topological count of the pinch.

The central charge ĉ = 4/3 is a weighted-homogeneous invariant. For one
block both variables have weight 1/6, and ĉ = Σ(1 − 2q_i) = 4/3. Three
blocks give ĉ(F) = 4, which is the Calabi–Yau fourfold charge. The
block and the fourfold share an arithmetic, not an identity of spaces.

W^T is the Berglund–Hübsch transpose of the same 2×2 exponent matrix.
It is the Landau–Ginzburg mirror of the *atom*, used by Fan–Shen, Guéré,
and 2-variable homological mirror symmetry. It is not a fourfold Y
derived-equivalent to V(F), and it is not a Hodge class on V(F).

"A different germ" means: you changed the local equation so the
microscope picture is no longer equivalent. Adding a third variable,
W + z^2, is a *suspension*. That is a surface singularity in three
coordinates. Strange duality theorems that need three variables talk
about that other germ, or about other 3-variable invertible polynomials.
They do not compute a number for W itself, and they do not produce a
(2,2)-class on the fourfold V(F).

What we uncovered is a clean split of objects that had been getting
mixed in conversation:

1. The atom W — 2-variable pinch, μ=30, own shelf.
2. Three atoms assembled as F — a smooth projective fourfold in P^5.
3. Surfaces Π and S on that fourfold — algebraic, so they hit the cycle
   class map.
4. The BHK string F^T — a mirror *recipe* in weighted space, not Y.
5. Vacuous Hodge — extra classes vanish on a *very general* high-degree
   fourfold, which V(F) is not.
6. Term A / Term B — the Clay sentence and its negation. Both empty.

The uncovering is classification, not a prize proof.

## To a professional

W is the Kreuzer–Skarke chain atom of type X^p Y + Y^q with (p,q)=(5,6).
Exponent matrix A = [[5,1],[0,6]], det A = 30 = μ(W). Isolated at 0 in
(C^2, 0). Quasihomogeneous: one convenient weighting is (1,1) of degree
6; the transpose weighting on W^T is (3,2) of degree 15. Charges
q_u = q_v = 1/6, ĉ = 4/3.

The germ (W,0) is the analytic equivalence class of this isolated
hypersurface singularity. Two germs are the same when there is a local
holomorphic coordinate change carrying one equation to the other
(right or contact equivalence, according to the problem). A *different
germ* is a different class. In particular:

- Suspension W(u,v) + z^k is a germ in (C^3, 0). Not (W,0).
- The three-block sum F in (C^6, 0) is a different germ again, and after
  projectivization and smoothness it is not a germ at all: V(F) subset P^5
  is a compact Calabi–Yau fourfold.
- Ebeling–Takahashi strange duality pairs Dolgachev and Gabrielov numbers
  of invertible polynomials in *three* variables. It does not assign those
  numbers to W.
- Ebeling–Gusein-Zade reduced monodromy zeta duality *does* apply to
  invertible chains, including this atom and its transpose.

Theorems that attach to (W,0) itself: Fan–Shen isomorphism of the FJRW
quantum ring of the dual Fermat-chain with the Milnor ring of W (up to
the usual conventions on which side is Fermat-chain); Guéré's chain FJRW
Hodge integrals; 2-variable HMS comparing D_sg(W) with Fukaya–Seidel of
W^T; EGZ zeta. None of these writes a class γ ∈ H^4(V(F),Q) ∩ H^{2,2}
outside im(cl).

Thom–Sebastiani says the Milnor fiber of a sum of functions in separate
variables is a join. That is why μ(F) = 30^3 and ĉ(F) = 4. It is a
product formula for vanishing cohomology of the *affine* singularity of
F at the origin in C^6, not a formula for Hdg^2 of the projective
fourfold V(F).

Status lock: atom ≠ fourfold ≠ miss ≠ WrittenPartner Y ≠ Term A ≠ Term B.
