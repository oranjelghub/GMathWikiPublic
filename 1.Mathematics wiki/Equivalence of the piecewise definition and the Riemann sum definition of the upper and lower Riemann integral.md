---
mathLink: auto
Date created: 2024-07-20 21:57
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Supremum and infimum]]
References: _Not applicable_
Justifications: [[Upper and lower Riemann integral]], [[Upper and lower Riemann integral in terms of Riemann sums]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Equivalence of the piecewise definition and the Riemann sum definition of the upper and lower Riemann integral
> Let $f:I\to \mathbb{R}$ be a bounded function on a bounded interval $I$. Then $$ \overline {\int}_{I} f=\inf \{ U(f,P): P\text{ is a partition of }I  \}  $$and $$ \underline {\int}_{I} f= \sup\{ L(f,P): P\text{ is a partition of }I \}  $$Where $\underline {\int}_{I}f$ and $\overline {\int}_{I}f$ are define as described here: [[Upper and lower Riemann integral]]

>[!quote]- Proof: Equivalence of the piecewise definition and the Riemann sum definition of the upper and lower Riemann integral
>We will only prove that $\overline {\int}_{I} f=\inf \{ U(f,P): P\text{ is a partition of }I  \}$ as the proof for the other part of the theorem is symmetric. We know that $U(f,P)$ has certain bounds, namely $$ U(f,P)\leq \text{p.c.} \int_{I} g $$Where $g$ is a piecewise constant function with respect to $P$ which majorizes $f$. Taking the infimum in $g$ obtains us $$U(f,P)\leq \overline {\int}_{I}f$$And then obviously $$ \inf\{ U(f,P): P\text{ is a partition of }I \}\leq \overline {\int}_{I} f $$Furthermore if we define for all $J\in P$ the function $h^{+}(J):=\sup_{x\in J}f(x)$ and the function $h(x):=h^{+}(J)$ whenever $x\in J$, we get $$ \overline {\int}_{I} f\leq \text{p.c.} \int_{I} h=U(f,P) $$Taking the infimum in $U(f,P)$ we obtain $$ \overline {\int}_{I} f\leq \inf\{ U(f,P): P\text{ is a partition of }I \} $$Thus we must have $$ \overline {\int}_{I} f=\inf\{ U(f,P): P\text{ is a partition of }I \} $$
>
>**Q.E.D.**
