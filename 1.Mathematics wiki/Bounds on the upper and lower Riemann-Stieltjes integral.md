---
mathLink: auto
Date created: 2024-08-07 01:07
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Supremum and infimum]]
References: _Not applicable_
Justifications: [[Upper and lower Riemann-Stieltjes integral]], [[Alpha-length of intervals]]

Specializations: [[Bounds on the upper and lower Riemann integral]]
Generalizations: _Not applicable_

---

> [!quote] Theorem: Bounds on the upper and lower Riemann-Stieltjes integral
> Let $X$ be a closed interval and let $\alpha:X\to \mathbb{R}$ be a $\alpha$-length on $X$. Let $I\subseteq X$ be a bounded interval and $f:I\to \mathbb{R}$ a bounded function. Then for some real $M$ $$ -M\alpha[I]\leq \underline {\int}_{I}f\;d\alpha\leq \overline {\int}_{I} f\;d\alpha\leq M\alpha[I] $$

>[!quote] Proof: Bounds on the upper and lower Riemann-Stieltjes integral
>Since $f$ is bounded we know $\left| f(x) \right|\leq M$ for some real $M$. Defining $g^{+}(x):=M$ and $g^{-}(x):=-M$ we have by definition that $$ -M\alpha[I]=\text{p.c.} \int_{I} g^{-}\;d\alpha\leq \underline {\int}_{I} f \;d\alpha \land \overline {\int}_{I} f \;d\alpha\leq \text{p.c.} \int_{I} g^{+}\;d\alpha=M\alpha[I] $$It only remains to show that $\underline {\int}_{I}f\;d\alpha\leq \overline {\int}_{I} f\;d\alpha$. Take some piecewise constant function on $I$ called $h^{+}$ that majorizes $f$, and do the same for some $h^{-}$, then clearly $$ \text{p.c.} \int_{I} h^{-}\;d\alpha\leq \text{p.c.} \int_{I} h^{+}\;d\alpha $$Take the infimum in $h^{+}$ and the supremum in $h^{-}$ grants us $$ \underline {\int}_{I}f\;d\alpha\leq \overline {\int}_{I} f\;d\alpha $$ Closing the proof.
>
>**Q.E.D.**
