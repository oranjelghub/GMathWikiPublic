---
mathLink: auto
Date created: 2024-10-08 14:27
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Determinant of a matrix (implicit definition)]], [[Determinant of a matrix (explicit permutative definition)]], [[Elementary matrices]], [[Matrix transposition]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Determinant of a matrix (Properties)
> Let $\det:M_{n\times n}(\mathbb{R})\to \mathbb{R}$  be the determinant map with $A,B\in M_{n\times n}(\mathbb{R})$, then 
> 1. $$ \det(S_{ij}(\lambda)A)=\det (A) $$
> 2. For $E\in \mathbf{E}(A)$ $$ \det(E)=\left\{ \begin{align} &1& E&=S_{ij}(\lambda)\\ &-1& E&=C_{ij}\\ &\lambda& E&= M_{i}(\lambda) \end{align} \right.  $$
> 3. For $E\in \mathbf{E}(A)$ $$ \det(EA)=\det(E)\det(A) $$
> 4. If $A$ is a upper or lower triangle matrix, then $$ \det(A)=\prod_{1\leq i\leq n}(A)_{ii} $$
> 5. $A$ is invertible if and only if $$ \det(A)\neq 0 $$
> 6. $$ \det(AB)=\det(A)\det(B) $$
> 7. Let $E\in \mathbf{E}(A)$, then $$ \det(E^{T})=\det(E) $$
> 8. $$ \det(A^{T})=\det(A) $$

>[!quote]- Proof: Determinant of a matrix (Properties)
>1. By linearity of $\det$ we have that $$ \det(S_{ij}(\lambda)A)=\det(A)+\lambda \det(A') $$Where $A'$ contains twice the $j$'th row, meaning that $\det(A')=0$. Implying that effectively $\det(S_{ij}(\lambda)A)=\det(A)$.
>2. This is a pretty trivial one if $E=M_{i}(\lambda)$ and $E=C_{ij}$. If $E=S_{ij}(\lambda)$ then by linearity of $\det$ we have $$ \det(S_{ij}(\lambda))=\det(\mathbb I_{n})+\lambda \det(S') $$Where once again $S'$ has twice the $j$'th row, and thus $\det(S_{ij}(\lambda))=1$.
>3. We don't prove this once since it is a trivial proof of splitting into cases.
>4. We use a unrigorous proof. WLOG assume $A$ is a upper triangle matrix. Take $a_{nn}$, if it is zero then the determinant of $A$ is zero and trivially the statement is true, so assume that $a_{nn}$ is non-zero. Then we can make all the other elements in the $n$'th column zero, which does not affect the determinant by property 1. These arguments can then reapply to the $n-1$ column and row. Thus we can write $A$ as a diagonal matrix with non-zero elements (assuming $a_{ii}\neq 0$ for all $1\leq i\leq n$). It follows by the linearity of $\det$ that $$ \det(A)=\prod_{1\leq i\leq n} (A)_{ii} $$
>5. If $A$ is invertible then we can write $$ A=\prod_{1\leq i\leq k}  E_{i} $$For some sequence of elementary matrices $( E_{i} )_{1\leq i \leq k}$. By three we can thus write $$ \det(A)=\prod_{1\leq i\leq k}\det(E_{i}) $$And since every term of this multiplication is non-zero by 2, we know that $\det(A)\neq 0$. We now prove it the other way around, which we do by contraposition. So assume $A$ is not invertible, then for some sequence $(E'_{i})_{1\leq i\leq k'}$ we have that $$ \left( \prod_{1\leq i\leq k'}E'_{i} \right)A=U  $$Where $U$ is some upper triangle matrix, which should not be invertible since $A$ isn't. This means there is somewhere a $0$ on the diagonal, which by 4 would imply that $\det(A)=\frac{\det(U)}{\det\left( \prod_{1\leq i\leq k'}E'_{i} \right)}=0$.
>6. Notice that if $A$ is not invertible that the statement becomes trivial by 5. Thus assume $A$ is invertible. It follows that for some sequence of elementary matrices $(E''_{i})_{1\leq i\leq k''}$ $$ \det(AB)=\det\left( \left( \prod_{1\leq i\leq k''}E \right)B \right)=\det\left( \prod_{1\leq i\leq k''}E \right)\det(B)=\det(A)\det(B) $$
>7. Let first $E=S_{ij}(\lambda)$, then $$ \det((S_{ij}(\lambda))^{T})=1=\det(S_{ij}(\lambda))$$If $E=M_{i}(\lambda)$, then the statement follows since $M_{i}(\lambda)=(M_{i}(\lambda))^{T}$. And if $E=C_{ij}$ then $(C_{ij})^{T}=C_{ji}$, from which the statement once again follows.
>8. If $A$ is not invertible then the statement is trivial since $A^{T}$ would also not be invertible and the proof would be closed by 5. If $A$ is invertible on the other hand, the proof is closed since we can write $A$ as a product of elementary matrices, using 6 and 7, the statement follows.

