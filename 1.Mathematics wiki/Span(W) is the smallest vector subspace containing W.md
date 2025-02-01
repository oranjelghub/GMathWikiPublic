---
mathLink: $\text{Span}(W)$ is the smallest vector subspace containing $W$
Date created: 2024-10-26 14:46
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Vector spaces]], [[Vector subspaces]], [[Span of a subset of a vector space]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: $\text{Span}(W)$ is the smallest vector subspace containing $W$
> Let $V$ be a vector space over some field $F$, and let $W\subseteq V$. Then for any vector subspace $D$ of $V$ containing $W$, we have $$ \text{span}(W)\subset_{\text{vec}}D $$ 

>[!quote] Proof: $\text{Span}(W)$ is the smallest vector subspace containing $W$
>Notice that is suffices to show that $$ \text{span}(W)=\bigcap_{U\in \{ D\in \mathcal{P}(V) \mid D\subset_{\text{vec}}V \land W\subseteq D \}}U $$To do this we first prove that $\text{span}(W)\subset\bigcap_{U\in \{ D\in \mathcal{P}(V) \mid D\subset_{\text{vec}}V \land W\subseteq D \}}U$. Let $w\in \text{span}(W)$, then for some scalars $\lambda_{i}\in F$ and vectors $w_{i}\in W$ we have $w=\sum^{n}_{i=1}\lambda_{i}w_{i}$. Since every $U$ in the intersection is a vector space itself, which also contains $W$ we know that it must be closed under it's operations. In other words $\sum^{n}_{i=1}\lambda_{i}w_{i}\in U$ for every $U$ in the intersection. Thus $\text{span}(W)\subset\bigcap_{U\in \{ D\in \mathcal{P}(V) \mid D\subset_{\text{vec}}V \land W\subseteq D \}}U$. We now prove the inclusion the other way around. Suppose $u\in \bigcap_{U\in \{ D\in \mathcal{P}(V) \mid D\subset_{\text{vec}}V \land W\subseteq D \}}U$. Then specifically $u\in \text{span}(W)$ since $\text{span}(W)$ contains $W$ and is a vector subspace of $V$. This proves the equality.
>
>**Q.E.D.**
