# Applications, safety, and a two-lane roadmap

Author: Benjamin Stanley Frohman (@BenFrohman)
Copyright (c) 2026 Benjamin Stanley Frohman. Apache-2.0.
Companion preprint: PREPRINT.md on this repository.

## Stark reality first

$W=u^5v+v^6$ is a **polynomial**. It is an isolated plane-curve singularity
of invertible chain type. The numbers $\mu=25$, $|\mathrm{Aut}|=30$,
$\mu(W^T)=26$, $\hat{c}=4/3$, and $\Delta_W(t)=(t^6-1)^4(t-1)$ are
**local analytic invariants**. That is what is in hand.

It is **not**:
- a physical atomic chain (carbyne, a 1D molecular wire, a polymer backbone);
- an AI checkpoint whose version tag happens to look like `u5v` / `v6`;
- a Hodge class on the fourfold $V(F)$;
- a recipe for a material, a drug, or a device.

What can actually be done with it, today:
1. Feed $(W,G)$ and $(W^T,G^T)$ into existing Berglund–Hübsch, FJRW, and
   homological-mirror pipelines as a worked two-variable example.
2. Use three Thom–Sebastiani copies as the local model of the locked
   sextic $F$.
3. Suspend to $W+z^2$ and only then ask Ebeling–Gusein-Zade / strange
   duality questions that require three variables.
4. Teach the $\mu\neq|\det A|$ distinction so the two integers stop being
   merged.

That is the ceiling of the present object. Everything below is a
**roadmap**, not a result.

---

## Lane 1 — AI and neural networks (analogical, not a trained model)

The token string `u5v-v6` looks like a checkpoint name. It is not one.
A responsible AI program *around* this atom would treat the germ as
**structured data**, not as a black-box generator.

### Possible programs
- Supervised invariants: train a graph/polynomial network to predict
  $(\mu,|\mathrm{Aut}|,\hat{c},\Delta(t))$ from exponent matrices of
  invertible singularities, with this pair as a labeled test case
  ($25$ vs $30$ is the trap).
- Search: enumerate Kreuzer–Skarke atoms and flag chain pairs with
  $\mu(W^T)=\mu(W)+1$.
- Language-to-geometry: map informal notes (“Fermat block”, “chain
  block”) onto exponent matrices so the $\mu$/Aut split is not lost
  again.
- HMS aid: use the computed spectrum as a check against Floer / matrix-
  factorization computations (Cho–Choa–Jeong and related HMS-for-curves
  work), not as a replacement for them.

### Usefulness
Speed of classification. Error-catching on published tables. A unit test
for any “singularity oracle.”

### Dangers and cautions (AI lane)
- Hallucination: a model that emits a zeta polynomial is not a proof.
  Kernel checks (`lean/MilnorCount.lean`) and Groebner bases stay in
  front of the network.
- Bias: training on Fermat examples will overfit $|\det A|=\mu$, which
  is false for this chain.
- Dual-use of *chemical* generative models is a real class of risk in
  the wider field. **This germ does not design molecules.** Do not wire
  an unconstrained molecular generator to this repository and call it
  “ChainAtom chemistry.” No synthesis routes, no agent designs, no
  target lists belong here.

---

## Lane 2 — Advanced materials / polymer physics (analogical, not a sample)

Laboratories that study literal atomic chains — carbyne, 1D wires,
conjugated polymers — use the words “chain” and “atom” for matter.
Our $W$ uses them for a Newton polygon. Do not mix the two.

### Honest adjacency
Landau–Ginzburg potentials *do* appear as effective models for some
condensed-matter and string compactifications. That does not make
$W=u^5v+v^6$ a recipe for ballistic transport or an anode. Extreme
tensile strength, room-temperature 1D conduction, and nanotoxicity are
properties of **physical samples**, measured in labs with containment,
not properties of a Jacobian algebra.

### Possible programs (theory only)
- Catalog which invertible atoms have been used as LG superpotentials
  in existing string / Gepner-style compactifications, and place this
  chain on that list with the correct $\hat{c}=4/3$ (two-variable) or
  $\hat{c}=4$ (three-copy fourfold $F$).
- Keep polymer and carbyne literature on a **separate shelf**. If a
  later collaboration wants a 1D-material model, start from measured
  Hamiltonians, not from $A=\begin{pmatrix}5&1\\0&6\end{pmatrix}$.

### Dangers and cautions (materials lane)
Nanotoxicity is a documented hazard of real nanoscale chains and
particles: inhalation, membrane crossing, systemic exposure. That
hazard attaches to **handling matter**, not to editing this markdown.
If a future project ever moves from the polynomial to a physical 1D
wire, it needs cleanroom / fume-hood protocol, waste control, and a
separate safety review. This repository does not authorize that step.

---

## Safety measures that apply now

1. Keep the object labeled: *invertible plane-curve germ*, not material,
   not model weights.
2. Keep $\mu$ and $|\mathrm{Aut}|$ in different columns.
3. Do not deposit a “Hodge disproof” that uses $W$ as $\gamma_{\mathrm{bad}}$.
4. Dual-use gate: refuse requests that ask this project to generate or
   optimize harmful chemical or biological agents. High-level warning
   only; no methods.
5. AI outputs that touch invariants must be checked by Groebner / Lean
   before they are written as theorems.
6. Zenodo deposit of PREPRINT.md is a paper deposit, not a materials
   data sheet and not a model card for a generator.

## What would count as a next real result

- Computed Saito dual of $\tilde\zeta_W$ after suspension $W+z^2$.
- An HMS comparison (Fukaya / matrix factorizations) that uses the
  $\Delta_W$ written in the preprint as a numerical check.
- A Kreuzer–Skarke table row in which this chain is not mis-labeled
  $\mu=30$.

Anything else is speculation. Speculation is allowed on a roadmap.
It is not allowed to overwrite the germ.
