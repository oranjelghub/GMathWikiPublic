---
mathLink: auto
Date created: 2024-07-20 21:40
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Supremum and infimum]], [[Series over finite sets (Properties)]]
References: _Not applicable_
Justifications: [[Riemann sums]], [[Piecewise constant integral]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Bounds on the upper and lower Riemann sum
> Let $f:I\to \mathbb{R}$ be a bounded functions on a bounded interval $I$, and let $g:I\to \mathbb{R}$ be a piecewise constant function that majorizes $f$ and let $h$ be a piecewise constant function that minorizes $f$. If $P$ is a partition of $I$ such that both $g$ and $h$ are piecewise constant with respect to $P$ then $$ \text{p.c.} \int_{I} g\geq U(f,P) \land \text{p.c.} \int_{I} h\leq L(f,P)$$

>[!quote] Proof: Bounds on the upper and lower Riemann sum
>We will only demonstrate that $\text{p.c.} \int_{I}\geq U(f,P)$ since the proof is symmetrical for the other part of the theorem. Since $g$ majorizes $f$ $$ \forall J\in P,  c_{J}\geq f(x) $$And by the definition of the supremum $$ c_{J}\geq \sup_{x\in J}f(x) $$ And since $\mu(J)$ is positive we have $$ c_{J}\mu(J)\geq (\sup_{x\in J}f(x)) \mu(J) $$ Taking the sum over all non-empty $J\in P$ gives us $$ \text{p.c.} \int_{I} g\geq U(f,P) $$
>
>**Q.E.D.**



