---
mathLink: auto
Date created: 2024-06-22 01:07
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Uniform continuity of real valued functions]], [[Cauchy sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Uniformly continuous real valued functions preserve Cauchyness of sequences
> Let $X\subseteq \mathbb{R}$ and $f:X\to \mathbb{R}$ a uniformly continuous function on $X$. If $(a_n)^\infty_{n=0}$ is some Cauchy sequence consisting of elements of $X$, then $(f(a_{n}))^\infty_{n=0}$ is also a Cauchy sequence.

>[!quote] Proof: Uniformly continuous real valued functions preserve Cauchyness of sequences
>Since $f$ is uniformly continuous on $X$ we have $$ \forall \varepsilon>0 \; \exists \delta>0: \forall x,y\in X, \; \left| x-y \right| \leq \delta \implies \left| f(x)-f(y) \right| \leq \varepsilon $$ Since $(a_n)^\infty_{n=0}$ is Cauchy we know that for some $N$ we have that for all $n,m\geq N$ that $\left| a_{n}-a_{m} \right|\leq \delta$, thus implying that $\left| f(a_{n})-f(a_{m}) \right|\leq \varepsilon$. But since the choice of epsilon is arbitrary we have that $(f(a_{n}))^\infty_{n=0}$ is also a Cauchy sequence.
>
>**Q.E.D.**


