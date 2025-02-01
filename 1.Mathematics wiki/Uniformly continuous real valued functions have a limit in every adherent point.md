---
mathLink: auto
Date created: 2024-06-22 01:12
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Completeness of the real numbers]], [[Uniformly continuous real valued functions preserve Cauchyness of sequences]]
References: _Not applicable_
Justifications: [[Cauchy sequences]], [[Uniform continuity of real valued functions]], [[Sequential definition of uniform continuity of real valued functions]], [[Sequential definition of limit of a function at a point]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Uniformly continuous real valued functions have a limit in every adherent point
> Let $X\subseteq \mathbb{R}$ and $f:X\to \mathbb{R}$ a function that is uniformly continuous on $X$. Let $x_{0}$ be an adherent point of $X$, then $\lim_{ x \to x_0:x\in X }f(x)$ exists.

>[!quote] Proof: Uniformly continuous real valued functions have a limit in every adherent point
>Let $(\alpha_n)^\infty_{n=0}$ be a sequence that consists of elements of $X$ which converges to $x_{0}$, since convergent sequence are Cauchy, $(\alpha_n)^\infty_{n=0}$ is a Cauchy sequence. It follows that $(f(\alpha_{n}))^\infty_{n=0}$ is a Cauchy sequence since uniformly continuous functions preserve Cauchyness, and since $\mathbb{R}$ is complete, it follows that $\lim_{ n \to \infty }f(\alpha_{n})=L$ for some real $L$. Now suppose that $(\alpha'_n)^\infty_{n=0}$ is some other sequence that also consists of elements of $X$ which converge to $x_{0}$, then it must be an equivalent sequence to $(\alpha_n)^\infty_{n=0}$, and since sequential equivalence is preserved under uniformly continuous functions by the sequential definition we know that $(f(\alpha_{n}))^\infty_{n=0}$ and $(f(\alpha'_{n}))^\infty_{n=0}$ are equivalent sequence, meaning they have the same limit. This shows that $\lim_{ x \to x_0:x\in X }f(x)=L$ by the sequential definition of limits of real valued functions.
>
>**Q.E.D.**


