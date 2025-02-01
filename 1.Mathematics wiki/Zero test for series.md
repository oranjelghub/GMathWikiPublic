
---

mathLink: auto

---
Date created: 2024-02-10 16:32
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Cauchyness lemma for convergence of series]]
References: _Not applicable_
Justifications: [[Infinite series]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Zero test for series
> Let $\sum^{\infty}_{n=m}a_{n}$ be a convergent series of real numbers. Then we must have $\lim_{ n \to \infty }a_{n}=0$.

>[!quote] Proof: Zero test for series
>Since the series converges we must have $$\forall \varepsilon>0\; \exists N\geq m: \forall p,q\geq N,\;      \left| \sum^{q}_{n=p} a_{n} \right|\leq \varepsilon $$ This is also true if we always pick $p=q$ thus giving us $$\forall \varepsilon>0\; \exists N\geq m: \forall p\geq N,\;      \left| a_{p} \right|\leq \varepsilon$$ Implying the sequence converges to 0.
>
>**Q.E.D.**


