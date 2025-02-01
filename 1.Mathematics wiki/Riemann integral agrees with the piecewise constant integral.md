---
mathLink: auto
Date created: 2024-07-20 19:50
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Piecewise constant integral]], [[Riemann integral]], [[Upper and lower Riemann integral]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Riemann integral agrees with the piecewise constant integral
> Let $f:I\to \mathbb{R}$ be a piecewise constant function on a bounded interval $I$. Then $f$ is Riemann integrable and $$ \int_{I} f  = \text{p.c.} \int_{I} f$$

>[!quote] Proof: Riemann integral agrees with the piecewise constant integral
>First note that $f$ is obviously a bounded function. Notice that $f$ majorizes and minorizes itself, and since $\underline {\int}_{I}f\leq \overline {\int}_{I}f$, we have by definition of the upper and lower integral$$ \sum^{}_{J\in P}c_{J}\mu(J)\leq\underline {\int}_{I}f\leq \overline {\int}_{I}f\leq \sum^{}_{J\in P}c_{J}\mu(J)  $$For some partition $P$ of $I$. Which means $$ \underline {\int}_{I} f=\sum^{}_{J\in P}c_{J}\mu(I)=\overline {\int}_{I} f $$And we have that $f$ is Riemann integrable and that $$ \int_{I} f=\text{p.c.} \int_{I} f $$
>
>**Q.E.D.**