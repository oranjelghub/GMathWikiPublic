---
mathLink: auto
Date created: 2024-07-06 17:31
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Differentiation of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Newton's approximation
> Let $X\subseteq \mathbb{R}$ and $f:X\to \mathbb{R}$ be a function. Let $x_{0}\in X$ be a limit point of $X$, then $f$ is differentiable at $x_{0}$ with derivative $L$ if and only if $$ \forall \varepsilon>0 \exists \delta>0: \forall x\in X, \left| x-x_{0} \right| \leq \delta \implies \left| f(x)-\left( f(x_{0})+L(x-x_{0}) \right) \right| \leq \varepsilon \left| x-x_{0} \right|  $$

>[!quote] Proof: Newton's approximation
>We first prove it from left to right so assume that $f$ is differentiable at $x_{0}$ with derivative $L$. It follows that $$ \forall \varepsilon>0 \exists \delta>0: \forall x\in X\backslash\{ x_{0} \}, \left| x-x_{0} \right| \leq \delta \implies \left| \frac{f(x)-f(x_{0})}{x-x_{0}} -L\right|\leq  \varepsilon  $$ We multiply by $\left| x-x_{0} \right|$ on both sides $$\forall \varepsilon>0 \exists \delta>0: \forall x\in X\backslash\{ x_{0} \}, \left| x-x_{0} \right| \leq \delta \implies \left| f(x)-f(x_{0})-L(x-x_{0}) \right|\leq \varepsilon \left| x-x_{0} \right|  $$You may note that this also holds for $x_{0}$ itself and thus for all $x\in X$, which proves our theorem in the first direction. Now suppose the converse and Newton's approximation holds. Then specifically $$  \forall \varepsilon>0 \exists \delta>0: \forall x\in X\backslash \{ x_{0} \}, \left| x-x_{0} \right| \leq \delta \implies \left| f(x)-\left( f(x_{0})+L(x-x_{0}) \right) \right| \leq \varepsilon \left| x-x_{0} \right| $$ Where we can now divide both sides by $\left| x-x_{0} \right|$ (which is non-zero since $x\in X\backslash \{ x_{0} \}$) to obtain $$ \forall \varepsilon>0 \exists \delta>0: \forall x\in X\backslash\{ x_{0} \}, \left| x-x_{0} \right| \leq \delta \implies \left| \frac{f(x)-f(x_{0})}{x-x_{0}} -L\right|\leq  \varepsilon  $$ Meaning that indeed $f$ is differentiable at $x_{0}$ with derivative $L$.

