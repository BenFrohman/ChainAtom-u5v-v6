# The chain atom $W=u^5v+v^6$: Milnor number 25, diagonal symmetry 30, and the transpose shift $+1$

**Author:** Benjamin Stanley Frohman  
**Affiliation:** independent  
**ORCID / contact:** GitHub [@BenFrohman](https://github.com/BenFrohman), X [@Investor0x](https://x.com/Investor0x)  
**Date:** 25 September 2026  
**License:** Apache License 2.0  
**Copyright:** © 2026 Benjamin Stanley Frohman  
**Repos:** [BenFrohman/ChainAtom-u5v-v6](https://github.com/BenFrohman/ChainAtom-u5v-v6), [BenFrohman/SingularityLab](https://github.com/BenFrohman/SingularityLab)

---

## Abstract

Let $W=u^5v+v^6$. This is an isolated invertible plane-curve singularity of chain type. Two integers that sit next to each other in the exponent matrix were conflated in earlier notes: the order of the maximal diagonal symmetry group is $|\det A|=30$, while the Milnor number — the dimension of the Jacobian algebra — is $25$. The Berglund–Hübsch transpose $W^T=u^5+uv^6$ has the same symmetry order and the same central charge $\hat{c}=4/3$, but Milnor number $26$. The shift is $\mu(W^T)=\mu(W)+1$. Three disjoint copies of $W$ reconstruct the locked sextic

$$
F=x_0^5x_3+x_3^6+x_1^5x_4+x_4^6+x_2^5x_5+x_5^6,
$$

with $\mu(F)=25^3=15625$ and $|\mathrm{Aut}(F)|=30^3=27000$. Steenbrink spectra and monodromy characteristic polynomials are computed from the Jacobian monomials. This note records those computations. It does not claim a Hodge miss on the fourfold $V(F)$.

## 1. The germ

$$
W(u,v)=u^5v+v^6,\qquad
A=\begin{pmatrix}5&1\\0&6\end{pmatrix},\qquad
|\det A|=30.
$$

Diagonal symmetries: $\mu^6=1$ and $\lambda^5\mu=1$, thirty characters. Weights $(1,1)$, degree $6$, charges $q=(1/6,1/6)$, central charge $\hat{c}=\sum(1-2q_i)=4/3$. Isolated at the origin: $\partial W/\partial u=5u^4v$ and $\partial W/\partial v=u^5+6v^5$ vanish together only at $0$.

## 2. Jacobian algebra

In characteristic $0$, $v^6\in(\partial W)$. A Groebner basis over $\mathbb{Q}$ is

$$
(v^6,\;u^5+6v^5,\;u^4v).
$$

Standard monomials, twenty-five:

$$
\{v^j,\ uv^j,\ u^2v^j,\ u^3v^j:\ j=0,\ldots,5\}\ \cup\ \{u^4\}.
$$

Quasihomogeneous check: $\mu(W)=(6/1-1)^2=25$. So $\mu(W)\neq|\mathrm{Aut}(W)|$. The integer $30$ is a group order, not a Jacobian dimension.

## 3. Transpose

$$
W^T=u^5+uv^6,\qquad
A^T=\begin{pmatrix}5&0\\1&6\end{pmatrix}.
$$

Weights $(3,2)$, degree $15$, same $\hat{c}=4/3$, same $|\mathrm{Aut}|=30$. Groebner basis $(uv^5,\,v^6+5u^4,\,u^5)$. Standard monomials, twenty-six. Quasihomogeneous check: $(15/3-1)(15/2-1)=26$. Bookkeeping:

$$
F=+1:\ W\mapsto W^T,\ \mu\mapsto\mu+1,\qquad
F=-1:\ W^T\mapsto W,\ \mu\mapsto\mu-1.
$$

A sign flip $-W$ is a different operation and does not change $\mu$. The affine fiber $W=-1$ is a Milnor fiber, homotopy-equivalent to a bouquet of $25$ circles. Compactification $X^5Y+Y^6+Z^6=0$ is a smooth plane sextic (genus $10$) minus six points at infinity; Euler characteristic $1-25=-24$ matches.

## 4. Spectrum and monodromy

Steenbrink numbers of $W$, $\alpha=(i+j+2)/6$ on the $25$ monomials:

$$
\tfrac13,\tfrac12,\tfrac23,\tfrac56,1,\tfrac76,\tfrac43,\tfrac32,\tfrac53
$$

with multiplicities $1,2,3,4,5,4,3,2,1$. Sum $25$, mean $1$, palindrome about $1$. Characteristic polynomial on $H_1$ of the Milnor fiber:

$$
\Delta_W(t)=(t-1)^5(t+1)^4(t^2+t+1)^4(t^2-t+1)^4=(t^6-1)^4(t-1).
$$

Reduced convention used in the companion file: $\tilde\zeta_W(t)=(1-t)^5(1+t)^4(1+t+t^2)^4(1-t+t^2)^4$. Compact form $\zeta_W(t)=(1-t^6)^{-4}$ matches the six-line tangent cone $W=v(u^5+v^5)$ after the usual $(1-t)$ bookkeeping.

For $W^T$, the $26$ spectral numbers lie in the same interval $[1/3,5/3]$ with mean $1$. The extra $+1$ sits in the middle. Then

$$
\Delta_{W^T}(t)=\Phi_1(t)^2\Phi_3(t)^2\Phi_5(t)\Phi_{15}(t)^2=\frac{(t^{15}-1)^2(t-1)}{t^5-1}.
$$

Ebeling–Gusein-Zade Saito duality of reduced zetas is a theorem about *three-variable* invertible polynomials (arXiv:1008.4021). This pair is two-variable. The polynomials above are the raw input, not a completed dual identity.

## 5. Three copies

Thom–Sebastiani and product of groups:

$$
\mu(F)=25^3=15625,\qquad |\mathrm{Aut}(F)|=30^3=27000,\qquad \hat{c}(F)=4.
$$

$F$ is the equation of a Calabi–Yau fourfold $V(F)\subset\mathbb{P}^5$. That fourfold is the geometric host in a separate project. The atom $W$ is local singularity data. Named algebraic classes on $V(F)$ (hyperplane square, plane, residual quintic) lie in the image of the cycle class map and are not a miss.

## 6. Suspension

$W+z^2$ is a three-variable germ with $\mu=25\cdot 1=25$. That is the object to which three-variable strange duality could be applied. Naming it is not computing Dolgachev–Gabrielov numbers.

## 7. What this note is not

Not a disproof of the rational Hodge conjecture. Not a Fourier–Mukai fourfold partner $Y$. Not an identification $\mu=|\det A|$. Lean checks of the two cardinalities $25$ and $26$ are `native_decide` counts of standard monomials (`lean/MilnorCount.lean` on SingularityLab).

## 8. Names, conversion, and machine-readable tables

Thirty is derived correctly as $\det A$. It becomes the wrong name only when it is called the Milnor number.

| integer | actual name |
|---|---|
| $30$ | $\lvert\det A\rvert=\lvert\mathrm{Aut}(W)\rvert$ |
| $25$ | $\mu(W)=\dim J_W$ |

The extra leading term $u^4v$ kills $u^4v,\,u^4v^2,\,u^4v^3,\,u^4v^4,\,u^4v^5$ in the $5\times 6$ box, so $30-5=25$. Conversion on this chain ($q=6$):

$$
\mu=\lvert\det A\rvert\cdot\bigl(1-1/q\bigr)=30\cdot\tfrac56=25.
$$

| | $\lvert\det A\rvert$ | $\mu$ |
|---|---|---|
| Meaning | diagonal symmetry order / exponent volume | Jacobian dimension / vanishing cycles |
| This $W$ | $30$ | $25$ |
| This $W^T$ | $30$ | $26$ |
| Three-block $F$ | $30^3=27000$ | $25^3=15625$ |
| Preserved by BHK transpose? | yes | no |

CSV keys live on the lab: [docs/tables/](https://github.com/BenFrohman/SingularityLab/tree/main/docs/tables). Prose lock: [DET_VS_MU.md](https://github.com/BenFrohman/SingularityLab/blob/main/docs/DET_VS_MU.md).

## References

1. M. Kreuzer, H. Skarke, *On the classification of quasihomogeneous functions*, Commun. Math. Phys. 150 (1992).
2. P. Berglund, T. Hübsch, *A generalized construction of mirror manifolds*, Nucl. Phys. B 393 (1993).
3. W. Ebeling, S. M. Gusein-Zade, *Monodromy of dual invertible polynomials*, arXiv:1008.4021.
4. J. Milnor, P. Orlik, *Isolated singularities defined by weighted homogeneous polynomials*, Topology 9 (1970).
5. Companion computations: https://github.com/BenFrohman/SingularityLab

---

*How to deposit.* Upload this file (or a PDF built from it) to Zenodo, attach `CITATION.cff` and `zenodo.json`, and use the metadata below. A DOI is issued by Zenodo after the user deposits; this repository does not mint one.
