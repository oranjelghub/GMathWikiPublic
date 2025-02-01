---
mathLink: auto
Date created: 2024-10-26 17:37
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: [[Induction]]
References: _Not applicable_
Justifications: [[Vector spaces]], [[Vector subspaces]], [[Sum and direct sum of vector spaces]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Criterium for direct sum of vector spaces
>Let $\{ U_{i} \}_{1\leq i\leq n}$ and $W$ be a collection of vector subspaces of some $F$-vector space $V$. Then $W=\bigoplus^{n}_{i=1}U_{i}$ if and only if 
>1. $$ W=\sum^{n}_{i=1}U_{i} $$
>2. $$ \forall k\in \mathbb{N}^{*}_{\leq n}: U_{k}\cap\left( \sum^{k-1}_{i=1}U_{i}+\sum^{n}_{i=k+1}U_{i} \right) =\{ 0 \}$$

>[!quote] Proof: Criterium for direct sum of vector spaces
>We first prove it from left to right. Since $W=\bigoplus^{n}_{i=1}U_{i}$ we clearly have that $W=\sum^{n}_{i=1}U_{i}$. We now want to show that $(2)$ holds. Fix some $j$ and fix some $v$ in $U_{j}\cap\left( \sum^{j-1}_{i=1}U_{i}+\sum^{n}_{i=j+1}U_{i} \right)$. Then $$ v=u_{j}=\sum^{j-1}_{i=1}u_{i}+\sum^{n}_{i=j+1}u_{i} $$ But since $W=\bigoplus^{n}_{i=1}U_{i}$ we must have that the sum representing $v$ is unique, which would only remain true if and only if $u_{i}=0$ for all $1\leq i\leq n$. This directly implies that $v=0$ and that $U_{j}\cap\left( \sum^{j-1}_{i=1}U_{i}+\sum^{n}_{i=j+1}U_{i} \right)=\{ 0 \}$. We now prove it the other way around. Suppose that our sums for some vector $v\in W$ were not unique, in other words $$ v=\sum^{n}_{i=1}u_{i}=\sum^{n}_{i=1}u'_{i} $$ Now fix some $1\leq j\leq n$, we have $$ u_{j}-u'_{j} =\sum^{j-1}_{i=1}u'_{i}-u_{i}+\sum^{n}_{i=j+1}u'_{i}-u_{i}$$ But since the intersection is $\{ 0 \}$, we have $u_{j}=u'_{j}$ and since $j$ is arbitrary this holds for every $1\leq i\leq n$. In other words, the sum is unique and $W=\bigoplus ^{n}_{i=1}U_{i}$
>
>**Q.E.D.**

