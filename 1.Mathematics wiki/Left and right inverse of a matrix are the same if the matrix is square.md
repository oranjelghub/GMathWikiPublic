---
mathLink: auto
Date created: 2024-09-06 22:13
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Left and right inverse of a matrix]] , [[Matrix multiplication]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Left and right inverse of a matrix are the same if the matrix is square
> Let $A\in M_{n\times n}(F)$ and let $B$ be some left inverse of $A$ and $C$ some right inverse of $A$, then $$ C=B $$

>[!quote] Proof: Left and right inverse of a matrix are the same if the matrix is square
>By the definition of left and right inverse it follows that $$ \begin{align}B&=B*\mathbb{I}_{n}\\ &=B*(A*C)\\&=(B*A)*C\\&=\mathbb{I}_{n}*C\\&=C \end{align}$$
>
>**Q.E.D.**

