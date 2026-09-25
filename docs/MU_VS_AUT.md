# μ is not |Aut|

Author: Benjamin Stanley Frohman (@BenFrohman).
Copyright (c) 2026 Benjamin Stanley Frohman. Apache-2.0.

Earlier notes used det A = 30 as the Milnor number of
W = u^5 v + v^6. That number is the order of the maximal diagonal
symmetry group, not dim of the Jacobian algebra.

## Two different 30-adjacent numbers

    A = [[5, 1], [0, 6]]
    |det A| = 30 = |Aut(W)|     # diagonal symmetries
    μ(W)   = 25 = dim C{u,v}/(∂W)

Quasihomogeneous check: weights (1,1), degree 6,

    μ = (6/1 - 1)(6/1 - 1) = 25.

Jacobian ideal (char 0):

    ∂W/∂u = 5 u^4 v,   ∂W/∂v = u^5 + 6 v^5.
    v^6 ∈ (∂W) because u·(∂W/∂u) and v·(∂W/∂v) differ by 6 v^6.

Leading ideal (u^5, u^4 v, v^6). Standard monomials, 25 of them:

    v^j          (j = 0..5)
    u v^j        (j = 0..5)
    u^2 v^j      (j = 0..5)
    u^3 v^j      (j = 0..5)
    u^4

Thom–Sebastiani on three disjoint copies:

    μ(F) = 25^3 = 15625
    |Aut(F)| = 30^3 = 27000

ĉ is unchanged: one block 4/3, three blocks 4.

## What this does not change

Still a 2-variable germ. Still not a class in Hdg^2(V(F)).
Still not Field 2 or Field 3. Coordinate-plane search on V(F):
only Π = V(x3,x4,x5) among the 20 coordinate P^2s. Span remains
Q h^2 + Q[Π].
