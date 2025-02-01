---
mathLink: auto
Date created: 2024-05-16 18:52
tags:
  - Type/Theorem
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Sequential definition of limit of a function at a point]], [[Equivalence between the sequential and the classic definition of the limit of a function at a point]]
References: _Not applicable_
Justifications: [[Limit of a real valued function at a point]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem:
> Let $X$ be a subset of $\mathbb{R}$, let $f : X → \mathbb{R}$ and $g:X\to \mathbb{R}$ be functions, let $E$ be a subset of $X$, let $x_0$ be an adherent point of $E$. If both $f$ and $g$ are convergent at $x_{0}$ then we have that 
> 1. $f\pm g$ is convergent at $x_{0}$ and $\lim_{ x \to x_0:x\in E }(f\pm g)(x)=\lim_{ x \to x_0:x\in E }f(x)\pm\lim_{ x \to x_0:x\in E }g(x)$
> 2. $\min(f,g)$ is convergent at $x_{0}$ and $\lim_{ x \to x_0:x\in E }\min(f(x),g,(x))=\min(\lim_{ x \to x_0:x\in E }f(x),\lim_{ x \to x_0:x\in E }g(x))$
> 3. $\max(f,g)$ is convergent at $x_{0}$ and $\lim_{ x \to x_0:x\in E }\max(f(x),g,(x))=\max(\lim_{ x \to x_0:x\in E }f(x),\lim_{ x \to x_0:x\in E }g(x))$
> 4. $fg$ is convergent at $x_{0}$ and $\lim_{ x \to x_0:x\in E }f(x)g(x)=\lim_{ x \to x_0:x\in E }f(x)\lim_{ x \to x_0:x\in E }g(x)$
> 5. $\frac{f}{g}$ is convergent at $x_{0}$ (given $\lim_{ x \to x_0:x\in E }g(x)\neq 0$ and $g$ non zero on $E$) and $\lim_{ x \to x_0:x\in E } \frac{f(x)}{g(x)}= \frac{\lim_{ x \to x_0:x\in E }f(x)}{\lim_{ x \to x_0:x\in E }g(x)}$
