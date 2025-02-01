---
mathLink: auto
Date created: 2024-07-11 21:32
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Comparison principle of sequences]], [[Sequential definition of limit of a function at a point]]
References: _Not applicable_
Justifications: [[Monotone real valued functions]], [[Differentiation of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Monotone real valued functions have non-zero derivative
> Let $X\subseteq \mathbb{R}$, let $x_{0}\in X$ be a limit point of $X$, and let $f:X\to \mathbb{R}$ be a function differentiable at $x_{0}$. If $f$ is monotone increasing then $f'(x_{0})\geq 0$, if $f$ is monotone decreasing then $f'(x_{0})\leq 0$.

>[!quote] Proof: Monotone real valued functions have non-zero derivative
>We only prove the case where $f$ is monotone increasing since the other case has a symmetric proof. Since $f$ is differentiable at $x_{0}$, we know that any sequence $(a_n)^\infty_{n=0}$ consisting of elements of $X\backslash\{ x_{0} \}$ that converges to $x_{0}$ induces a sequence $(\frac{f(a_{n})-f(x_{0})}{a_{n}-x_{0}})^\infty_{n=0}$ which converges to $f'(x_{0})$. But notice that $$ \forall n, \frac{f(a_{n})-f(x_{0})}{a_{n}-x_{0}}\geq 0  $$and by taking the limit on both sides we obtain $f'(x_{0})\geq 0$.
>
>**Q.E.D.**





