---
mathLink: auto
Date created: 2024-08-04 18:15
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Series over finite sets (Properties)]], [[Common refinement of bounded intervals]]
References: _Not applicable_
Justifications: [[Alpha-length of intervals]], [[Piecewise constant Riemann-Stieltjes integral]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Piecewise constant Riemann Stieltjes integrals are well-defined
> Let $X$ be a closed interval and let $\alpha:X\to \mathbb{R}$ be a $\alpha$-length on $X$. Let $I\subseteq$ be a bounded interval and let $f:I\to \mathbb{R}$ be a piecewise constant function. If $P$ and $P'$ are two partitions such that $f$ is piecewise constant with respect to them, then $$ \sum^{}_{J\in P}	c_{J}\alpha[J]=\sum^{}_{J\in P'}c_{J}\alpha[J] $$

>[!quote] Proof: Piecewise constant Riemann Stieltjes integrals are well-defined
>It suffices to show that $$ \sum^{}_{J\in P}c_{J}\alpha[J]=\sum^{}_{J\in P\#P'}c_{J}\alpha[J] $$Thus $$ \begin{align} \sum^{}_{J\in P\# P'}c_{J}\alpha[J] =\sum^{}_{(K,L)\in P\times P'} c_{K\cap L}\alpha[K\cap L] \end{align} $$By Fubini's theorem we know that $$ \sum^{}_{(K,L)\in P\times P'} c_{K\cap L}\alpha[K\cap L]=\sum^{}_{K\in P}\sum^{}_{L\in P'} c_{K\cap L}\alpha[K\cap L]$$And since for all $K$ and $L$, $c_{K}=c_{K\cap L}$, we get $$ \sum^{}_{K\in P}\sum^{}_{L\in P'} c_{K\cap L}\alpha[K\cap L]=\sum^{}_{K\in P}c_{K}\sum^{}_{L\in P'}\alpha[K\cap L] $$But notice that $\{ K\cap L: L\in P' \}$ forms a partition of $K$, since $\alpha$-length is finitely additive it follows that $$ \sum^{}_{K\in P}c_{K}\sum^{}_{L\in P'}\alpha[K\cap L]=\sum^{}_{K\in P}c_{K}\alpha[K] $$Thus $$\sum^{}_{J\in P}	c_{J}\alpha[J]=\sum^{}_{J\in P'}c_{J}\alpha[J] $$
>
>**Q.E.D.**
