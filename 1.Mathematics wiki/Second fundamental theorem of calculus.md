---
mathLink: auto
Date created: 2024-09-17 20:29
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Mean value theorem]], [[Alpha-length is finitely additive]], [[First fundamental theorem of calculus]]
References: _Not applicable_
Justifications: [[Antiderivative of a real valued function]], [[Alpha-length of intervals]], [[Riemann integral]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Second fundamental theorem of calculus
> Let $a\leq b$ be real numbers, and let $f:[a,b]\to \mathbb{R}$ be a Riemann integrable. If $F:[a,b]\to \mathbb{R}$ is a antiderivative of $f$ then $$ \int_{[a,b]} f=F(b)-F(a) $$

>[!quote] Proof: Second fundamental theorem of calculus
>The claim is trivial for $a=b$ so assume that $a<b$. To prove the theorem it suffices to show that for every partition $P$ of $[a,b]$ we have $$ L(f,P)\leq F(b)-F(a)\leq U(f,P) $$We only show that $U(f,P)\geq F(b)-F(a)$ since the proof for the other part of the inequality is symmetric. So let $P$ be some partition of $[a,b]$. $F$ is continuous since it is differentiable, and consequently we consider the $\alpha$-length induced by $F$. Then $$ F(b)-F(a)=\sum^{}_{J\in P}F[{J}]=\sum^{}_{J\in P: J\neq \emptyset}F[J] $$It now suffices to show that $$ F[J]\leq \sup_{x\in J}f(x)\left| J \right|  $$For every $J\in P$, so fix such a $J$, we say it has endpoints $c<d$ (since the case $c=d$ is trivial), thus $$ F[J]=F(d)-F(c) $$By the continuity of $F$, the mean value theorem asserts that for some $e\in [a,b]$ $$ F(d)-F(c)=(d-c)F'(e)=(d-c)f(e)=\left| I \right| f(e)\leq \sup_{x\in J}f(x)\left| J \right|  $$As desired.
>
>**Q.E.D.**
