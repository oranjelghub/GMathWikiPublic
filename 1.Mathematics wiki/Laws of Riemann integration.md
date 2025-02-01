---
mathLink: auto
Date created: 2024-07-22 18:38
tags:
  - Type/Theorem
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Laws of integration of the piecewise constant integral]], [[Bounds on the upper and lower Riemann sum]], [[Bounds on the upper and lower Riemann integral]]
References: [[Laws of Riemann integration (Proof)]]
Justifications: [[Riemann integral]], [[Laws of Riemann integration]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Laws of Riemann integration
> Let $I$ be a bounded interval and $f:I\to \mathbb{R}$ and $g:I\to \mathbb{R}$ be Riemann integrable functions on $I$.
> 1. $f+g$ is Riemann integrable on $I$ and $$ \int_{I} f+g=\int_{I} f+\int_{I} g $$
> 2. For $c\in \mathbb{R}$, $cf$ is Riemann integrable on $I$ and $$ \int_{I} cf=c\int_{I} f  $$
> 3. If $f(x)\geq g(x)$ for all $x\in I$ then $$ \int_{I} f\geq \int_{I} g $$
> 4. Let $J$ be a bounded interval that contains $I$, and let $F:J\to \mathbb{R}$ be a function $$ F(x):=\left\{\begin{align} &f(x)&\hspace{1cm} &x\in I\\ &0&\hspace{1cm} &x\not\in I\end{align}  \right. $$Then $F$ is Riemann integrable on $J$ and $$ \int_{J} F=\int_{I} f $$
> 5. Suppose $\{ J,K \}$ is a partition of $I$ into two intervals, then $f|_{J}$ and $f|_{K}$ are both Riemann integrable on their respective domain and $$ \int_{I} f=\int_{J} f|_{J}+\int_{K} f|_{K} $$

