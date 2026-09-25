# Applications, safety, and a two-track roadmap

**Author:** Benjamin Stanley Frohman (@BenFrohman)  
**Copyright:** (c) 2026 Benjamin Stanley Frohman  
**License:** Apache-2.0

This file is attached to the ChainAtom preprint. It separates three layers
that must not be mixed.

1. What the object *is*.
2. What can actually be done with that object.
3. Two analog tracks (AI; materials / polymer physics) that share a *name
   pattern*, not an identity.

---

## Stark reality

`ChainAtom` here is the isolated plane-curve germ

    W = u^5 v + v^6,     μ(W) = 25,     |Aut(W)| = 30,
    W^T = u^5 + u v^6,   μ(W^T) = 26.

It is a quasihomogeneous invertible polynomial. It is not carbyne, not a
1D molecular wire, not a polymer, not a battery anode, and not an LLM
checkpoint tagged `u5v` / `v6`.

What this note **can** do:

- correct a bookkeeping error (|Aut| was labeled μ)
- feed FJRW / LG state-space calculations for this chain block
- feed monodromy-zeta and spectrum calculations (already written)
- serve as a Thom–Sebastiani atom inside the sextic F
- teach BHK transpose on a single explicit pair

What this note **cannot** do:

- prove or disprove rational Hodge on fourfolds
- produce a Fourier–Mukai partner Y of V(F)
- design a semiconductor, a drug, or a toxin
- move electrons ballistically
- fold a protein
- replace laboratory synthesis or toxicology

If a later project uses the *string* `u5v-v6` as a model name, that
project is a different object and needs its own safety file.

---

## Track A — AI and neural networks (analog, not identity)

Long tokens such as `u5v` or `v6` do appear as checkpoint names and as
embedding codes. A model that *ingested* this germ could, in principle,
be asked to predict Jacobian dimensions, spectra, or FJRW numbers for
other invertible polynomials.

**Possible uses if such a model is trained on invertible singularities**

- fast lookup of μ, |Aut|, ĉ, and leading ideals for chain / loop / Fermat atoms
- generating candidate BHK pairs and checking the +1-type μ shift
- assisting formalization (Lean statements like `mu_W` / `mu_WT`)

**Safety**

- Hallucination: a model that emits μ = 30 for W is repeating the error
  this note exists to kill. Treat model output as a conjecture until a
  Gröbner basis or `native_decide` check exists.
- Dual-use: general molecular-generation models can propose toxic or
  weaponizable compounds. This germ is not a molecule, but any pipeline
  that *turns polynomials into chemical graphs* inherits that hazard.
  Do not connect this repo to an unconstrained generator. Human review
  before any wet-lab suggestion. No automated synthesis loop.
- Provenance: keep the mathematical object and any ML checkpoint in
  separate repositories so a version tag cannot be mistaken for a proof.

**Roadmap (AI)**

1. Dataset of invertible germs with verified (μ, Aut, ĉ, Δ(t)).
2. Supervised predictor with a Lean verifier in the loop.
3. Refusal layer: no SMILES / PDB output from this track.
4. Audit log of every predicted integer against a computer-algebra oracle.

---

## Track B — materials / polymer physics (analog, not identity)

Literal atomic chains (carbyne, 1D wires, conjugated polymers) are a
different science. Insights there concern 1D electron transport and
tensile strength. Usefulness, if that science succeeds, is in
semiconductors, anodes, and nanomaterials.

**Safety (this track, if ever pursued as materials work)**

- Nanotoxicity: high-aspect-ratio carbon chains and related particles
  can cross membranes and the blood-brain barrier. Inhalation and skin
  exposure are the default hazards. Cleanroom or glovebox. No dry
  powder work without containment. Medical surveillance if a lab is
  stood up.
- This preprint does **not** authorize a materials experiment. There is
  no synthesis protocol in this repository.
- Do not cite μ(W)=25 as a tensile modulus or a band gap.

**Roadmap (materials) — only if a separate lab is funded**

1. Literature review of actual carbyne / polyyne stability. Not this germ.
2. Independent ethics and tox screen before any synthesis proposal.
3. No shared filename with the singularity shelf.

---

## What to do next on the real object

1. Deposit the preprint on Zenodo (DOI is not minted by GitHub).
2. Keep computing 2-variable facts: spectrum of W^T already listed;
   Saito identity still not claimed.
3. If strange duality is wanted, work on the named 3-variable germ
   W+z^2 as a *different* paper.
4. Do not move these files into HODGE as a miss class.
