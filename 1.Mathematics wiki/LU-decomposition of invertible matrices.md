---
mathLink: auto
Date created: 2024-10-21 18:17
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Elementary matrices]], [[Row equivalence]], [[Upper and lower triangle matrices]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: LU-decomposition of invertible matrices
> Let $A\in \text{GL}_{n}(F)$ be a matrix that can be brought into row echelon form without switching rows. Then there exists a unique lower triangle matrix $L$ and upper triangle matrix $U$ such that $$ A=LU $$

>[!quote] Proof: LU-decomposition of invertible matrices
>We first prove the existence of such a decomposition. Since $A$ can be brought into row echelon form with row switches there exists some sequence of elementary matrices $(E_{i})_{1\leq i\leq k}$ such that $$ \overset{\curvearrowleft}{\prod^k_{i=1}}E_{i} A=U$$Where $U$ is the row echelon form of $A$, which is clearly a upper triangle matrix. We can now invert every convert the collection of elementary matrices to obtain $$ A=\overset{\curvearrowright}{\prod^{k}_{i=1}}E^{-1}_{i}U $$It is easy to show that each one of these inverse elementary matrices is a lower triangle matrix, thus the whole product is one as well. So we may write $$ A=LU $$We proceed to prove the uniqueness of this decomposition. Suppose that for two lower triangle matrices $L_{1}$,$L_{2}$ and two upper triangle matrices $U_{1}$,$U_{2}$ we have $$ L_{1}U_{1}=A=L_{2}U_{2} $$Since $A$ is invertible, we know that these four matrices must be invertible as well. So we may write $$ L_{2}^{-1}L_{1}=U_{2}U_{1}^{-1} $$Notice that on the left we have a two lower triangle matrices and on the right two upper triangle matrices. Thus they must both just have a non-zero diagonal with all the other entries being zero. **Apparently it can be argued that this diagonal only consist of the   entry $1$, which means that $$L_{2}^{-1}L_{1}=\mathbb{I}_{n}=U_{2}U_{1}^{-1}$$In other words $L_{2}=L_{1}$ and $U_{1}=U_{2}$.** 
>
>**Q.E.D.**