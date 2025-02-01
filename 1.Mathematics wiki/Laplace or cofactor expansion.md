---
mathLink: auto
Date created: 2024-10-20 16:32
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Determinant of a matrix (explicit permutative definition)]], [[Determinant of a matrix (Properties)]], [[Minor of a matrix in the i'th row and j'th column]], [[Cofactor of a matrix in the i'th row and j'th column]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Laplace or cofactor expansion
> Let $A\in M_{n\times n}(F)$, then we can "expand" the $i$'th row and get  $$\det(A)=\sum^{n}_{j=1}a_{ij}\mathfrak C_{ij}$$ Where $\mathfrak C_{ij}$ is the cofactor in the $i$'th row and $j$'th column and $m_{ij}$ is the minor in the $i$'th row and $j$'th column. Similar can be said by expanding to the $j$'th row of $A$.  In other words $$ \det(A)=\sum^{n}_{i=1}a_{ij}\mathfrak C_{ij} $$

>[!quote] Proof: Laplace or cofactor expansion 
>We prove the expansion in the $i$'th row. Define the family of sets $\{ P_{k} \}_{1\leq k\leq n}$ by $$ P_{k}:=\{ \sigma\in S_{n}: \sigma(i)=k \} $$All these sets are disjoint and $\bigcup_{1\leq k\leq n}P_{k}=S_{n}$. We can thus write $$ \det(A)=\sum^{n}_{j=1}\sum^{}_{\sigma\in P_{j}} \text{sgn}(\sigma)\prod_{1\leq l\leq n} a_{l\sigma(l)}$$Notice that $a_{i\sigma(i)}$ is a constant term in each of these products and that $\sigma(i)=j$, thus $$ \det(A)=\sum^{n}_{j=1}a_{ij}\sum^{}_{\sigma\in P_{j}} \text{sgn}(\sigma)\prod_{1\leq l\leq n: l\neq i} a_{l\sigma(l)}$$We also know that applying a column or row operation on $A$ switches the sign of the determinant, more notably, with $i-1$ row switches and $j-1$ column switches. We can obtain a matrix with first row $R_{i}$ and first column $K_{j}$, with in the corner the matrix $A_{\cancel{ ij }}$. Notice now that$^{1}$ $$ \sum^{}_{\sigma\in P_{j}} \text{sgn}(\sigma)\prod_{1\leq l\leq n: l\neq i} a_{l\sigma(l)}=(-1)^{i+j}\det(A_{\cancel{ ij }})=(-1)^{i+j}m_{ij}$$
>
>**Q.E.D.**

**_Remark_**$^1$: I am not a fan at all of this final step. I don't fully get why the additional row and column operations are absolutely necessary and why we can't just say that the left hand side is directly equal to $m_{ij}$. This probably stems out of the fact that the used documentation is a bit handwavey with the proof and thus I don't see where the error is. The corrective term of $(-1)^{i+j}$ is absolutely necessary though. The used documentation is Lineaire Algebra (Paul Igodt en Wim Veys).