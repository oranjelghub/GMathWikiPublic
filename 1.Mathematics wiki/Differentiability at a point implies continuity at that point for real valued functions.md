---
mathLink: auto
Date created: 2024-07-04 19:01
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Limit laws for real valued functions]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Differentiation of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Differentiability at a point implies continuity at that point for real valued functions
> Let $X\subseteq \mathbb{R}$ and $f:X\to \mathbb{R}$ be a function differentiable at some limit point $x_{0}\in X$, then $f$ is also continuous at $x_{0}$.

>[!quote] Proof: Differentiability at a point implies continuity at that point for real valued functions
>To show that $f$ is continuous it suffices to show that $$\lim_{ x \to x_0:x\in X\backslash \{ x_{0} \} }f(x)-f(x_{0})=0$$ To show this notice that we can multiply by $1$ as follows $$ \lim_{ x \to x_0:x\in X\backslash\{ x_{0} \} }f(x_{0})-f(x)  \frac{x_{0}-x}{x_{0}-x}$$And since $f$ is differentiable and $\lim_{ x \to x_0:x\in X\backslash\{ x_{0} \} }x_{0}-x$ exists, we may apply the product rule for limits and deduce that $$ \lim_{ x \to x_0:x\in X\backslash\{ x_{0} \} }f(x_{0})-f(x)  \frac{x_{0}-x}{x_{0}-x}= f'(x_{0})*0=0$$ Meaning that indeed $f$ is continuous at $x_{0}$
>
>Q.E.D.

