
---

mathLink: Convergence of $\zeta(q)$

---
Date created: 2024-02-26 11:26
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Cauchy condensation test for series]], [[Geometric series]]
References: _Not applicable_
Justifications: [[Infinite series]]

Specializations: _Not applicable_
Generalizations: [[Riemann-zeta function]]

---  

Considering the restricted Riemann-zeta function $$ \zeta: \mathbb{Q}^+ \to \mathbb{R}:q \mapsto \sum^{\infty}_{n=1} \frac{1}{n^q} $$
> [!quote] Theorem: Convergence of $\zeta(q)$
> Let $q>0$ be a rational number. Then $\zeta(q)$ is convergent if $q>1$ an divergent when $q\leq 1$.

>[!quote] Proof: Convergence of $\zeta(q)$
>The sequence $\left( \frac{1}{n^q} \right)^\infty_{n=1}$ is non-negative and decreasing. We can thus apply the Cauchy condensation theorem and study the convergence of $$ \sum^{\infty}_{k=0} 2^k\frac{1}{({2^k})^q} =\sum^{\infty}_{k=0} (2^{1-q})^k$$ Which according to theory around geometric series will convergence if and only if $\left| 2^{1-q} \right|<1$ or in other words if $q>1$ the series would be convergent, otherwise it would be divergent.
>
>**Q.E.D.**

Note that we also implicitly proved the divergence of the [[Harmonic series]].