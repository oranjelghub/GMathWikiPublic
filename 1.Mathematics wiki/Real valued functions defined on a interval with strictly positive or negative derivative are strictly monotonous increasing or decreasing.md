---
mathLink: auto
Date created: 2024-07-11 21:43
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Mean value theorem]]
References: _Not applicable_
Justifications: [[Differentiation of real valued functions]], [[Monotone real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Real valued functions defined on a interval with strictly positive or negative derivative are strictly monotonous increasing or decreasing
> Let $a<b$ be real and let $f:[a,b]\to \mathbb{R}$ be a differentiable function. If $f'(x)>0$ for all $x\in [a,b]$ then $f$ is strictly monotone increasing. Similarly, if $f'(x)<0$ for all $x\in [a,b]$ then $f$ is strictly monotone decreasing.

>[!quote] Proof: Real valued functions defined on a interval with strictly positive or negative derivative are strictly monotonous increasing or decreasing
>We only prove the case where $f'(x)>0$ for all $x\in [a,b]$ as the proof for the other case is symmetric. Fix any arbitrary $x,y$ such that $y<x$, notice that $f|_{[y,x]}$ is also differentiable on $[y,x]$ and that thus by the mean value theorem we can argue that for some $c\in [y,x]$ $$ f'(c)=f'|_{[y,x]} (c)=\frac{f|_{[y,x]}(x)-f|_{[y,x]}(y)}{x-y}=\frac{f(x)-f(y)}{x-y} $$Implying that $\frac{f(x)-f(y)}{x-y}>0$, and since $x>y$ we must thus have $f(x)>f(y)$. In other words $f$ is strictly monotone increasing.
>
>**Q.E.D.**


