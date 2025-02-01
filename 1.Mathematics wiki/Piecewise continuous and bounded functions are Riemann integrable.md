---
mathLink: auto
Date created: 2024-07-30 17:37
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Laws of Riemann integration]]
References: _Not applicable_
Justifications: [[Riemann integral]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Piecewise continuous and bounded functions are Riemann integrable
> Let $I$ be a bounded interval and let $f:I\to \mathbb{R}$ be a piecewise continuous and bounded function. Then $f$ is Riemann integrable.

>[!quote] Proof: Piecewise continuous and bounded functions are Riemann integrable
>Notice that $$ f(x)=\sum^{}_{J\in P}f(x) \chi_{J}(x)$$Where $P$ is some interval partition of $I$ such that $f$ is piecewise continuous with respect to that partition, and $\chi_{J}$ is the characteristic function with respect to $J$. Notice that for every $J\in P$, $f\chi_{J}$ is Riemann integrable over $I$. Thus $f$ is a sum of Riemann integrable functions and is itself Riemann integrable over $I$.
>
>**Q.E.D.**

