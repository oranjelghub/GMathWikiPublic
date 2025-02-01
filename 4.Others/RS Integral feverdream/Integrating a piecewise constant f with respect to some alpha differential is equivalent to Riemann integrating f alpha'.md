---
mathLink: Integrating a piecewise constant $f:\mathbb R \to \mathbb R$ with respect to some $\alpha$ differential is equivalent to Riemann integrating $f \alpha'$
Date created: 2024-09-25 17:05
tags:
  - Type/Theorem
cssclasses:
---




---

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---

> [!quote] Theorem:
> Let $\alpha:[a,b]\to \mathbb{R}$ be a differentiable $\alpha$-length on $[a,b]$, with $\alpha'$ being Riemann integrable. Let $f:[a,b]\to \mathbb{R}$ be a piecewise constant function on $[a,b]$. Then $f\alpha'$ is Riemann integrable and $$ \int_{[a,b]} f\; d\alpha=\int_{[a,b]} f\alpha' $$

>[!quote] Proof:

Since $f$ is piecewise constant on $[a,b]$, and since $\alpha'$ is also Riemann integrable, we know that $f\alpha'$ is also Riemann integrable. Suppose that $f$ is piecewise constant with respect to some partition $P$. WLOG we may assume that $P$ does not contain the empty set. Then we have $$ \int_{[a,b]} f\; d\alpha=\text{p.c.} \int_{[P]} f\;d\alpha=\sum^{}_{J\in P}c_{J}\alpha[J] $$On the other hand