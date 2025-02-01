---
mathLink: auto
Date created: 2024-11-10 21:14
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Properties of absolute value]]
References: _Not applicable_
Justifications: [[Cauchy sequences]], [[Real numbers]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Cauchy sequences of real numbers are bounded
> Let $(a_n)^\infty_{n=0}$ be a Cauchy sequence of real numbers. Then $(a_n)^\infty_{n=}$ is bounded.

>[!quote] Proof: Cauchy sequences of real numbers are bounded
>Fix some $\varepsilon>0$, since $(a_n)^\infty_{n=0}$ is Cauchy we know that for some $N\in\mathbb{N}$ $$ \forall n,m\geq N: \left| a_{n}-a_{m} \right| \leq \varepsilon$$The first $N$ elements are bounded by $\max_{n\leq N}a_{n}$ whilst the remaining elements are bounded since by the triangle inequality $$ \forall m\geq N :\left| a_{m} \right| -\left| a_{N} \right| \leq \left| a_{m}-a_{N} \right| \leq \varepsilon $$Thus the entire sequences is bounded by $$ \max(\max_{n\leq N}a_{n}, \varepsilon+\left| a_{N} \right| ) $$
>
>**Q.E.D.**
