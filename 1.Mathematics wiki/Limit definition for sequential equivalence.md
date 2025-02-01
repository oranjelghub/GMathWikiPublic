---
mathLink: auto
Date created: 2024-06-16 22:56
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Cauchy sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Limit definition for sequential equivalence
> Two real valued sequences $(a_n)^\infty_{n=0}$ and $(b_n)^\infty_{n=0}$ are equivalent if and only if $$ \lim_{ n \to \infty } (a_{n}-b_{n})=0 $$

>[!quote] Proof: Limit definition for sequential equivalence
>Define $c_{n}:=a_{n}-b_{n}$, since the sequences are equivalent we have that $$ \forall \varepsilon>0\; \exists N: \forall n\geq N, \left| a_{n}-b_{n} \right| \leq \varepsilon $$ But notice that this implies that for all $n\geq N$ we have that $\left| c_{n} \right|\leq \varepsilon$, which means that $\lim_{ n \to \infty }c_{n}=0$ or in other words $\lim_{ n \to \infty }(a_{n}-b_{n})=0$.
>
>**Q.E.D.**

