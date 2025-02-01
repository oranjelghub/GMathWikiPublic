---
mathLink: auto
Date created: 2025-01-08 21:31
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---
---  

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Trace of a matrix]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Trace of a product of matrices
> Let $F$ be a field and let $A,B \in M_{n\times n}(F)$. Then $$ \mathrm{Tr}(AB)=\mathrm{Tr}(BA) $$

>[!quote] Proof: Trace of a product of matrices
>$$ \begin{align} \mathrm{Tr}(AB)&= \sum^{n}_{i=1}(AB)_{ii} \\ &= \sum^{n}_{i=1}\sum^{n}_{j=1}a_{ij}b_{ji} \\ &= \sum^{n}_{j=1}\sum^{n}_{i=1}b_{ji}b_{ij}  \\ &= \sum^{n}_{j=1} (BA)_{jj} \\ &= \mathrm{Tr}(BA)\end{align} $$
>
>**Q.E.D.**

