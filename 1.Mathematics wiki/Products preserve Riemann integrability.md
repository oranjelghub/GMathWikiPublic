---
mathLink: auto
Date created: 2024-07-29 17:51
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Max and min preserve Riemann integrability]], [[Laws of Riemann integration]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Piecewise constant integral]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Products preserve Riemann integrability
> Let $I$ be a bounded interval, and let $f:I\to \mathbb{R}$ and $g:I\to \mathbb{R}$ be Riemann integrable functions. Then $fg$ is also Riemann integrable

>[!quote]- Proof: Products preserve Riemann integrability
>Decompose the functions $f$ and $g$ into their positive and negative parts such that $$ fg=f^{+}g^{+}+f^{+}g^{-}+f^{-}g^{+}+f^{-}g^{-} $$Notice that $f^{+}$,$f^{-}$,$g^{+}$,$g^{-}$ are all Riemann integrable since for example $f^{+}:=\max(0,f)$. The functions can all we written in terms of a min or max operator, which preserves Riemann integrability. To close this proof it would now suffice to show that each function of the sum above is also Riemann integrable, so we cover the first case in detail. Namely we show that $f^{+}g^{+}$ is Riemann integrable. Notice that $f$ is bounded by some $M_{1}$ and $g$ by some $M_{2}$, then $$ f^{+}(x)\leq M_{1}\land g^{+}(x)\leq M_{2} $$Now fix some arbitrary $\varepsilon >0$, and take some piecewise constant functions $\underline{f^{+}}$ and $\overline{f^{+}}$such that $$ \int_{I} f-\varepsilon\leq \int_{I} \underline{f^{+}}\leq \int_{I} \overline{f^{+}}\leq \int_{I} f+\varepsilon $$Notice we may assume without loss of generality that $\underline{f^{+}}$ is non-negative on $I$, since we may always define $\tilde{\underline{f^{+}}}:=\max(\underline{f^{+}},0)$, which would still be piecewise constant and minorize $f^{+}$ as wanted. Similarly we may assume that $\overline{f^{+}}\leq M_{1}$, this being said we have $$ 0\leq \underline{f^{+}}\leq f^{+}\leq \overline{f^{+}}\leq M_{1}$$This entire construction can be done again but this time for $g^{+}$, and since $\underline{f^{+}g^{+}}$ is piecewise constant as well and minorizes $f^{+}g^{+}$ whilst $\overline{f^{+}g^{+}}$ is piecewise constant and majorizes $f^{+}g^{+}$ we have $$ 0\leq \overline {\int}_{I} f^{+}g^{+}-\underline {\int}_{I} f^{+}g^{+}\leq \int_{I} \overline{f^{+}g^{+}}-\underline{f^{+}g^{+}} $$Implying $$ 0\leq \overline {\int}_{I} f^{+}g^{+}-\underline {\int}_{I} f^{+}g^{+}\leq \int_{I} \overline{f^{+}g^{+}}+\overline{f^{+}}\underline{g^{+}}-\overline{f^{+}}\underline{g^{+}}-\underline{f^{+}g^{+}}=\int_{I} \overline{f^{+}}(\overline{g^{+}}-\underline{g^{+}}) +\underline{g^{+}}(\overline{f^{+}}-\underline{f^{+}})$$And we get $$ 0\leq \overline {\int}_{I} f^{+}g^{+}-\underline {\int}_{I} f^{+}g^{+}\leq M_{1}2\varepsilon+M_{2}2\varepsilon$$And since $\varepsilon$ is arbitrary we must have that $f^{+}g^{+}$ is Riemann integrable. Now the other three cases follow by using the same argument and being a bit more carefull around the signs of the functions, but otherwise it's a symmetric argument. Thus $fg$ can be written as a finite sum of Riemann integrable functions and is thus Riemann integrable as well.
>
>**Q.E.D.**

