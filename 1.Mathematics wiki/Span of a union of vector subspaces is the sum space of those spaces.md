---
mathLink: auto
Date created: 2024-10-26 17:19
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Span of a subset of a vector space]], [[Sum and direct sum of vector spaces]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Span of a union of vector subspaces is the sum space of those spaces
> Let $\{ U_{i} \}_{1\leq i\leq n}$ be a collection of vector subspaces of some $F$-vector space $V$. Then $$  \text{span}\left( \bigcup^{n}_{i=1} U_{i} \right)=\sum^{n}_{i=1}U_{i}$$

>[!quote] Proof: Span of a union of vector subspaces is the sum space of those spaces
>We prove this by proving the two subset inclusions. First we show that $\text{span}\left( \bigcup^{n}_{i=1} U_{i} \right)\subseteq\sum^{n}_{i=1}U_{i}$. Let $w\in \text{span}\left( \bigcup^{n}_{i=1}U_{i} \right)$, then for some collection of vectors and scalars $$ w=\sum^{k}_{i=1}\lambda_{i}v_{i} $$We write $P_{j}:=\{ \lambda_{i}v_{i} \mid v_{i}\in U_{j} \}$. We thus may write $$ w=\sum^{n}_{j=1}\sum^{}_{v\in P_{j}} v$$And since all the $U_{i}$ are vector subspaces we have that $$ w=\sum^{n}_{j=1}u_{j} \hspace{1.5cm} \forall j:u_{j}\in U_{j} $$Then clearly $w\in \sum^{n}_{i=1}U_{i}$. The other inclusions follows directly from the definition of $\text{span}()$.
>
>**Q.E.D.**

