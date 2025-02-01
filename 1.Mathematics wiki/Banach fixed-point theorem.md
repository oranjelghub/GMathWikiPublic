---
mathLink: auto
Date created: 2024-05-25 19:10
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
  - Topic/Topology
cssclasses:
---

---

Proved by: [[Induction]], [[Continuity of contractive maps]], [[Geometric series]], [[Sequential definition of continuity of functions in arbitrary metric spaces]]
References: _Not applicable_
Justifications: [[Contractions]], [[Metric spaces]], [[Completeness of metric spaces]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Banach fixed-point theorem
> Let $(X,d)$ be a complete metric space and let $\Phi$ be a contraction on $X$, then there exists a unique point $\hat{x}\in X$ such that $\Phi(\hat{x})=\hat{x}$, furthermore $$\forall x\in X, \lim_{ n \to \infty }\bigcirc^n_{i=1}\Phi(x)=\hat{x}$$

>[!quote] Proof: Banach fixed-point theorem
>Fix some $x_{0}\in X$, we write $\bigcirc^n_{i=1}\Phi(x_{0})=\Phi^{n}(x_{0})=\chi_{n}$. We can show by induction that $$ \forall n\in \mathbb{N}, d(\chi_{n},\chi_{n+1})\leq q^{n}d(\chi_{0},\chi_{1}) $$ Where $q$ is the contraction factor of the contraction. Now notice that for any $m\geq 0$ and for any $n> m$, we have by the triangle inequality $$ d(\chi_{n},\chi_{m})\leq \sum^{n-m}_{i=1}d (\chi_{n-i},\chi_{n-i+1})$$ Applying the previously discussed property we have that $$ d(\chi_{n},\chi_{m})\leq d(\chi_{0},\chi_{1})\sum^{n-m}_{i=1}q^{n-i}=  q^{m}d(\chi_{0},\chi_{1})\sum^{n-m}_{i=1}q^{n-m-i}=q^{m}d(\chi_{0},\chi_{1})\sum^{n-m-1}_{k=0}q^{k}$$ Now notice that this series is increasing and thus bounded above by $\sum^{\infty}_{k=0}q^{k}$, which is convergent because it is a geometric series, more specifically $$ d(\chi_{n},\chi_{m})\leq q^{m}d(\chi_{0},\chi_{1})\sum^{n-m-1}_{k=0}q^{k}\leq \frac{q^{m}}{1-q}d(\chi_{0},\chi_{1}) $$ And since $(q^{n})^\infty_{n=0}$ converges to $0$ we have that for all $\varepsilon$ there exists an $M$ such that $\frac{q^{m}}{1-q}d(\chi_{0},\chi_{1})\leq \varepsilon$. Now notice that for all $J,K\geq M$ we have for some $j,k$  that $M+j=J$ and $M+k=K$, now WLOG assume that $k\leq j$ then by induction once again $$ d(\chi_{M+j},\chi_{M+k})\leq q^{k}d(\chi_{M+j-k},\chi_{M})\leq\frac{q^{m}}{1-q}d(\chi_{0},\chi_{1})\leq \varepsilon$$ In other word $\chi_{n}$ is a Cauchy sequence. Thus it must have some limit inside $X$ by the completeness of $(X,d)$, we call it $\hat{x}$. It now follows by the continuity of contractive maps that $$\Phi(\hat{x})=\Phi(\lim_{ n \to \infty } \chi_{n})=\lim_{ n \to \infty } \Phi(\chi_{n})=\lim_{ n \to \infty } \chi_{n+1}=\hat{x}$$ Thus $\hat{x}$ is a fixed point. To prove it is unique assume that there existed two fixed points. Then $$ d(\hat{x},x^{*})=d(\Phi(\hat{x}),\Phi(x^{*}))\leq qd(\hat{x},x^{*}) $$ This implies that $1\leq q$, and by contrapositive this must mean that $\hat{x}$ is unique since $q<1$.
>
>**Q.E.D.**
