---
mathLink: auto
Date created: 2024-04-28 12:06
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Infinite series]], [[Absolute and conditional convergence of series]]

Specializations: _Not applicable_
Generalizations: [[Properly divergent permutation of a series (Riemann series theorem)]]

---

> [!quote] Theorem: Divergence of the series of positive or negative entries of a conditionally convergent series
> Let $\sum^\infty_{n=0}a_n$ be a conditionally converging series, but not a absolutely converging one. Define the sets $A^+:=\{ n\in \mathbb N: a_n\geq 0 \}$ and $A^-:=\{ n\in \mathbb N: a_n< 0 \}$. Then both of the series $\sum_{n\in A^+}a_n$ and $\sum_{n\in A^-}a_n$ are divergent.

Proof at the start of this pdf:

>[!quote] Proof: Divergence of the series of positive or negative entries of a conditionally convergent series
>We prove this by proving the proper divergence of $\sum^{}_{n\in A^+}a_{n}$ to $+\infty$. Notice that the series grows arbitrarily large, since if this wasn't the case, then there would be a upper bound on the partial sums which are also increasing and thus the series would be absolutely convergent. Where the same argument applies to $\sum^{}_{n\in A^-}a_{n}$, adding these two together and using properties of series over infinite sets we would have that the original series is also absolutely convergent, a contradiction. 
>
>**Q.E.D.**

