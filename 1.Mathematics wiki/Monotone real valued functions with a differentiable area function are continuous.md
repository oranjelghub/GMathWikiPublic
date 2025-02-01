---
mathLink: auto
Date created: 2024-09-23 15:37
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Left and right limits of real valued functions]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Differentiation of real valued functions]], [[Continuity of real valued functions]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Monotone real valued functions with a differentiable area function are continuous
> Let $I$ be a bounded interval and $f:I\to \mathbb{R}$ be a monotone function and $$ F(x):= \int_{[a,x_{0}]} f $$ Let $x_{0}\in I$, if $F$ is differentiable at $x_{0}$, then $f$ is continuous at $x_{0}$.

>[!quote] Proof: Monotone real valued functions with a differentiable area function are continuous
>Assume for the sake of contradiction that $f$ is not continuous at $x_{0}$, then denote $$ 0<\epsilon:=\left| f(x_{0}^{+})-f(x_{0}^{-}) \right|  $$(We know the left and right limits exist since $f$ is monotone) and $$ L:= \frac{f(x_{0}^{+})+f(x^{-}_{0})}{2} $$Now for any $\varepsilon<\epsilon$, we have $$ f(x^{-}_{0})\leq L-\varepsilon\leq L+\varepsilon\leq f(x^{+}_{0}) $$Since $f$ is monotone, for all $x<x_{0}$ we have $f(x)\leq L-\varepsilon$ and if $x_{0}<x$ then $L+\varepsilon\leq x_{0}$. It follows that $$ \int_{[x,x_{0}]}f\leq (L-\varepsilon)(x_{0}-x)\leq  (L+\varepsilon)(x_{0}-x) \leq \int_{[x_{0},x]} f $$And since $F$ is Lipschitz-continuous we have $$ \lim_{ x \to x_0^{-} } \frac{F(x_{0})-F(x)}{x_{0}-x} <L<\lim_{ x \to x_0^{+} } \frac{F(x)-F(x_{0})}{x-x_{0}}$$But this implies that $F$ is not differentiable at $x_{0}$, a contradiction.
>
>**Q.E.D.**
