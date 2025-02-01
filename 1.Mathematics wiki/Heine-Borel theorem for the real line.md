---
mathLink: auto
Date created: 2024-05-07 19:23
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Axiom of choice]], [[Bounded sets in R]], [[Bolzano-Weierstrass theorem]]
References: _Not applicable_
Justifications: [[Subsequences]], [[Closed subsets]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

This theorem requires the axiom of choice.

> [!quote] Theorem: Heine-Borel theorem for the real line
> A set $X \subseteq \mathbb{R}$ is closed and bounded if and only if every $(x_n)^\infty_{n=0}$, where for all $n$ we have $x_{n}\in X$, has some convergent subsequence $(x_{f(n)})^\infty_{n=0}$ with $\lim_{ n \to \infty }x_{f(n)} \in X$. 

>[!quote] Proof: Heine-Borel theorem for the real line
>We first prove the statement from left to right. Since $X$ is bounded we have that every sequence in $X$ is also bounded above by $M$ and below by $-M$, which means we can apply the Bolzano-Weierstrass theorem and find some convergent subsequence which must also converge in $X$ since $X$ is closed. This closes the first case. Now we want to prove it from right to left. Since every convergent subsequence converges in $X$ we already have that $X$ is closed, it remains to show that it is also bounded. Suppose for the sake of contradiction that that isn't the case and that $X$ is unbounded. Then notice that $$ E_{M}:=X\backslash [-M,M] $$ is never empty. Thus we can pick some choice function $(c_n)^\infty_{n=0}$ and notice that $$ \forall M\in \mathbb{N}\; \forall K\geq M, M\leq \left| c_{K} \right|  $$ Notice that this sequence does not have any convergent subsequence. But this would mean that our original hypothesis is wrong. Thus $X$ must be bounded, which closes the last case
>
>**Q.E.D.**

