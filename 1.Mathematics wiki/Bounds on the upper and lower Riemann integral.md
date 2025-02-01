---
mathLink: auto
Date created: 2024-07-19 21:13
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Supremum and infimum]]
References: _Not applicable_
Justifications: [[Upper and lower Riemann integral]], [[Piecewise constant integral]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Bounds on the upper and lower Riemann integral
> Let $f:I \to \mathbb{R}$ be a bounded function on some bounded interval $I$, then for some $M$ $$ -M\mu(I)\leq \underline {\int}_{I} f\leq \overline {\int}_{I} f\leq M\mu(I) $$

>[!quote] Proof: Bounds on the upper and lower Riemann integral
>Since $f$ is a bounded function we have that $\left| f(x) \right|\leq M$ for some $M$ and for all $x\in I$. Now let $g^{+}(x):=M$ and $g^{-}(x):=-M$, then $g^{+}$ majorizes $f$ and is piecewise constant on $I$ whilst $g^{-}$ minorizes $f$ and is also piecewise constant on $I$. Per definition it follows that $$ \text{p.c.} \int_{I} g^{-}=-M\mu(I)\leq \underline {\int}_{I} f \land \overline {\int}_{I} f\leq M\mu(I)=\text{p.c.} \int_{I} g^{+} $$To end the proof we need to show that $\underline {\int}_{I}f\leq \overline {\int}_{I}f$. Let $g:I\to \mathbb{R}$ be some piecewise constant function on $I$ which majorizes $f$ and let $h:I\to \mathbb{R}$ be a piecewise constant function on $I$ which minorizes $f$. It follows that $$ \text{p.c.} \int_{I} h\leq \text{p.c.} \int_{I} g $$Taking the supremum in $h$ gives us $$ \underline {\int}_{I} f\leq \text{p.c.} \int_{I} g $$Taking the infimum in $g$ gives us $$ \underline {\int}_{I} f\leq \overline {\int}_{I} f $$
>
>**Q.E.D.**

