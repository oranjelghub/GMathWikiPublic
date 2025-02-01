---
mathLink: auto
Date created: 2024-07-10 18:13
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Local extrema are stationary]], [[Maximum principle for real valued functions]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Differentiation of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Rolle's theorem
> Let $a<b$ be real numbers and let $f:[a,b] \to \mathbb{R}$ be a function such that $f$ is continuous on $[a,b]$, differentiable on $(a,b)$ and $f(a)=f(b)$. Then there exists $c\in (a,b)$ such that $f'(c)=0$.

>[!quote] Proof: Rolle's theorem
>First since the statement is trivial for constant functions we may assume that $f$ is non-constant. Since $f$ is continuous on $[a,b]$ we may argue by the maximum principle that there exists some maximum $x^{+}$ and some minimum $x^{-}$, both element of $[a,b]$. Now as long as either $x^{+}$ or $x^{-}$ is in $(a,b)$ we are done, since then $f'(x^{+})=0$ or $f'(x^{-})=0$ because both are extrema and $f$ is differentiable on $(a,b)$. We now claim that this is indeed always the case, either $x^{+}$ or $x^{-}$ is in $(a,b)$. We prove this by contradiction, assume that both are in $[a,b]\backslash(a,b)$ then one can easily verify that the $f$ is constant, but we assumed that $f$ was non-constant. Thus we must have either $x^{+}$ or $x^{-}$ in $(a,b)$ and we are done.
>
>**Q.E.D.**


