
---

mathLink: auto

---
Date created: 2024-02-10 17:00
Tags: #Type/Theorem  #Topic/Real_Analysis 

Proved by: [[Cauchyness lemma for convergence of series]], [[Finite series (Properties)]]
References: _Not applicable_
Justifications: [[Infinite series]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Absolute convergence test for series
>If the infinite series of real numbers $\sum^{\infty}_{n=m}a_{n}$ is absolutely convergent then it is also conditionally convergent.

>[!quote] Proof: Absolute convergence test for series
>Since the series is absolutely convergent we have that $$ \forall \varepsilon>0\; \exists N\geq m:\forall p,q\geq N,\; \left| \sum^{q}_{n=p}|a_{n}| \right| \leq \varepsilon $$ By applying a absolute value on both of the sides of the classic triangle inequality we get $$ \left| \sum^{q}_{n=p}a_{n}  \right| \leq\left| \sum^{q}_{n=p}|a_{n}| \right| \leq \varepsilon$$ Since $\varepsilon$ is arbitrary we have that the series $\sum^{\infty}_{n=m}a_{n}$ also converges.
>
>**Q.E.D.**



