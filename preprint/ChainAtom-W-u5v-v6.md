# The chain atom $W=u^5v+v^6$: Milnor number, diagonal symmetries, and the Berglund–Hübsch transpose

**Author:** Benjamin Stanley Frohman  
**Affiliation:** independent  
**X:** [@Investor0x](https://x.com/Investor0x)  
**GitHub:** [@BenFrohman](https://github.com/BenFrohman)  
**Date:** 25 September 2026  
**Copyright:** © 2026 Benjamin Stanley Frohman  
**License:** Apache-2.0  
**Version:** 1.0

Companion computation lab: [BenFrohman/SingularityLab](https://github.com/BenFrohman/SingularityLab)  
This shelf: [BenFrohman/ChainAtom-u5v-v6](https://github.com/BenFrohman/ChainAtom-u5v-v6)

---

## Abstract

The invertible chain germ

$$W=u^5v+v^6$$

is isolated as the local atom of the Calabi–Yau sextic

$$F=(x_0^5x_3+x_3^6)+(x_1^5x_4+x_4^6)+(x_2^5x_5+x_5^6)$$

in $\mathbb{P}^5$. Two integers attached to $W$ are not the same. The maximal diagonal symmetry group has order $|\mathrm{Aut}(W)|=|\det A|=30$. The Milnor number, the dimension of the Jacobian algebra, is $\mu(W)=25$. The Berglund–Hübsch transpose

$$W^T=u^5+uv^6$$

has the same Aut-order and the same central charge $\hat{c}=4/3$, but $\mu(W^T)=26=\mu(W)+1$. Three Thom–Sebastiani copies recover $F$, with $\mu(F)=25^3=15625$ and $|\mathrm{Aut}(F)|=30^3=27000$. The monodromy characteristic polynomial of $W$ is $\Delta_W(t)=(t^6-1)^4(t-1)$. This note records those counts, the standard monomial bases, the Steenbrink spectra, and what the pair does *not* do: it is not a Fourier–Mukai fourfold partner, not a rational Hodge miss on $V(F)$, and not a 3-variable strange-duality theorem.

**Keywords:** invertible polynomial, Berglund–Hübsch–Krawitz, chain singularity, Milnor number, monodromy zeta, Thom–Sebastiani

---

## 1. How the atom appeared

The polynomial $F$ is a sum of three disjoint chain blocks of type $x^5y+y^6$. Writing one block in local coordinates gives

$$W=u^5v+v^6=v(u^5+v^5).$$

The exponent matrix and its transpose are

$$
A=\begin{pmatrix}5&1\\0&6\end{pmatrix},\qquad
A^T=\begin{pmatrix}5&0\\1&6\end{pmatrix},\qquad
|\det A|=30.
$$

The corresponding transpose germ is $W^T=u^5+uv^6$. That pair is the Berglund–Hübsch atom of $F$ and $F^T$. The isolation of $W$ as a 2-variable plane-curve singularity is the accident that produced this note: a fourfold calculation dropped a local germ.

---

## 2. Two different counts

### 2.1 Diagonal symmetries

Characters $(\lambda,\mu)\in(\mathbb{C}^*)^2$ with $W(\lambda u,\mu v)=W(u,v)$ obey $\mu^6=1$ and $\lambda^5\mu=1$. There are 30 solutions. This is $|\mathrm{Aut}(W)|=|\det A|$. The same count holds for $W^T$.

### 2.2 Milnor number of $W$

Partials: $5u^4v$ and $u^5+6v^5$. In characteristic 0, $v^6$ lies in $(\partial W)$. Leading ideal $(u^5,\,u^4v,\,v^6)$. Standard monomials:

$$
\{u^iv^j:\ i\le 3,\ j\le 5\}\ \cup\ \{u^4\}.
$$

There are $4\cdot 6+1=25$ of them. The quasihomogeneous formula with weights $(1,1)$ and degree 6 gives the same integer:

$$\mu(W)=\Bigl(\frac{6}{1}-1\Bigr)^2=25.$$

Lean check (no `sorry`, `native_decide`): `lean/MilnorCount.lean` in SingularityLab.

### 2.3 Milnor number of $W^T$

Weights $(3,2)$, degree 15. Partials $5u^4+v^6$ and $6uv^5$. Lex Gröbner basis contains $v^{11}$. Standard monomials:

$$
v^{0,\ldots,10}\qquad\text{and}\qquad u^{1,2,3}v^{0,\ldots,4}.
$$

Count $11+15=26$. Quasihomogeneous check: $(15/3-1)(15/2-1)=26$. So

$$\mu(W^T)=\mu(W)+1.$$

BHK transpose preserves $|\mathrm{Aut}|$ and $\hat{c}$, not $\mu$. The directed shifts are $F=+1$ ($W\to W^T$) and $F=-1$ ($W^T\to W$). A sign flip of the polynomial is a different $F=-1$ and does not change $\mu$.

### 2.4 Three blocks

Thom–Sebastiani and the product of groups give

$$\mu(F)=25^3=15625,\qquad |\mathrm{Aut}(F)|=30^3=27000,\qquad \hat{c}(F)=4.$$

---

## 3. Spectrum and monodromy

Steenbrink numbers of $W$, weights $(1,1)$, degree 6:

$$
\tfrac13,\ \tfrac12,\ \tfrac23,\ \tfrac56,\ 1,\ \tfrac76,\ \tfrac43,\ \tfrac32,\ \tfrac53
$$

with multiplicities $1,2,3,4,5,4,3,2,1$. Mean $1$, support $[1/3,5/3]$.

Characteristic polynomial on $H_1$ of the Milnor fiber:

$$
\Delta_W(t)=(t^6-1)^4(t-1)=(t-1)^5(t+1)^4(t^2+t+1)^4(t^2-t+1)^4.
$$

With $\tilde\zeta(t)=\det(I-tT\mid H_1)$,

$$
\tilde\zeta_W(t)=(1-t)^5(1+t)^4(1+t+t^2)^4(1-t+t^2)^4.
$$

The 26 spectral numbers of $W^T$ (weights $(3,2)$, degree 15) are listed in SingularityLab `docs/ZETA.md`. They occupy the same interval $[1/3,5/3]$ with mean $1$. The extra $+1$ sits in the middle.

The fiber $W=-1$ is a bouquet of 25 circles; $W^T=-1$ is a bouquet of 26.

Saito duality of *reduced* monodromy zeta for invertible polynomials, in the form computed by Ebeling–Gusein-Zade, is stated in the literature for settings that include a 3-variable theorem. The pair $(W,W^T)$ is 2-variable. The identity $\tilde\zeta_W\leftrightarrow\tilde\zeta_{W^T}$ is therefore named, not claimed as a computed equality of these two functions. The suspension $W+z^2$ is a different germ ($\mu=25$) and is recorded separately; naming it does not run strange duality.

---

## 4. What this is not

- Not a Fourier–Mukai partner fourfold $Y\not\simeq V(F)$. $F^T$ is a BHK string, not six FM fields.
- Not a class in $H^4(V(F),\mathbb{Q})\cap H^{2,2}(V(F))$, and not a proof that some such class misses $\mathrm{im}(\mathrm{cl})$.
- Not a proof or disproof of the rational Hodge conjecture.
- Not Ebeling–Takahashi Dolgachev–Gabrielov duality (three variables).
- Not a heterotic $c=9$ compactification ($V(F)$ is a fourfold).

The contribution is classification: two integers that had been conflated are split, the $+1$ shift is written, and the monodromy polynomial of this specific chain is computed.

---

## 5. Repositories

- Computations, Lean, zeta, fibers: https://github.com/BenFrohman/SingularityLab
- Atom shelf and this preprint: https://github.com/BenFrohman/ChainAtom-u5v-v6

---

## References

1. P. Berglund, T. Hübsch, *A generalized construction of mirror manifolds*, Nucl. Phys. B 393 (1993).
2. M. Krawitz, *FJRW rings and Landau–Ginzburg mirror symmetry*, PhD thesis, Michigan (2010).
3. W. Ebeling, S. M. Gusein-Zade, *Monodromy of dual invertible polynomials*, arXiv:1008.4021.
4. W. Ebeling, A. Takahashi, *Strange duality of weighted homogeneous polynomials*, Compositio Math. 147 (2011).
5. J. Milnor, P. Orlik, *Isolated singularities defined by weighted homogeneous polynomials*, Topology 9 (1970).
6. J. H. M. Steenbrink, *Mixed Hodge structure on the vanishing cohomology*, Nordic Summer School / NAVF (1976).
