---
mathLink: Fixed point theorem in $\mathbb R$
Date created: 2024-06-12 16:46
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Intermediate value theorem]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Fixed point theorem in $\mathbb{R}$
> Let $a<b$ and $f:[a,b]\to[a,b]$ be a continuous function on $[a,b]$, then there $f$ has a fixed point. In other words $$ \exists k\in [a,b]: f(k)=k $$

>[!quote] Proof: Fixed point theorem in $\mathbb{R}$
>Notice that we have $a\leq f(x)\leq b$ and $-b\leq x\leq -a$, define $g(x):=f(x)-x$ and notice that by combining the two inequalities we get $$ a-b\leq g(x) \leq b-a$$ Since $a-b\leq 0\leq b-a$ and $g$ is also continuous on $[a,b]$ we have by the intermediate value theorem that $$\exists k\in [a,b]: g(x)=0$$ Which implies that $f(k)=k$.
>
>**Q.E.D.**
