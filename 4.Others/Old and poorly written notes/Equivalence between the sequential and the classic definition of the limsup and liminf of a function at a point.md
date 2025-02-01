---
mathLink: auto
Date created: 2024-05-22 09:57
tags:
  - Type/Proof
cssclasses:
---

---  

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---

> [!quote] Proof: Equivalence between the sequential and the classic definition of the limsup and liminf of a function at a point
> We only cover the proof for superior limits, as the the proof for inferior ones is very similar.

During the whole proof we use $E\subseteq X\subseteq \mathbb R$ and some function $f:X\to \mathbb R$. So suppose that $\limsup_{ x_{0} \to x: x\in E }f(x)=L$ by the classic definition, then we have $$\forall N, \; L\leq \sup \left(f\left(\left[x_0-\frac{1}{N}, x_0+\frac{1}{N}\right]\cap E\right) \right)$$
