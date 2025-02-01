---
mathLink: auto
Date created: 2024-07-10 18:47
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Mean value theorem]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Differentiation of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Real valued differentiable functions with bounded derivative are Lipschitz continuous
> Let $a<b$ be real numbers and $f:[a,b]\to \mathbb{R}$ be a function such that $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$, and such that there exists a real $M>0$ for which $$ \forall x\in (a,b), \left| f'(x) \right| \leq M $$Then $f$ is Lipschitz continuous with Lipschitz constant $M$.

>[!quote] Proof: Real valued differentiable functions with bounded derivative are Lipschitz continuous
>Fix two arbitrary real $x,y$ between $a$ and $b$, assume WLOG that $y<x$. Since $f|_{[y,x]}$ is differentiable on $(y,x)$ and continuous on $[y,x]$ we may apply the mean value theorem to claim that there exists some $z\in (y,x)$ such that $$ f'(z)=f'|_{[y,x]}(z)= \frac{f(x)-f(y)}{x-y} $$Implying $$ \left| f'(z) \right| = \left| \frac{f(x)-f(y)}{x-y} \right| \leq M $$Giving us that $\left| f(x)-f(y) \right|\leq M\left| x-y \right|$, and since the choice of $x,y$ was arbitrary this holds for all $x,y\in [a,b]$ and we have that $f$ is Lipschitz continuous with Lipschitz constant $M$.
>
>**Q.E.D.**




