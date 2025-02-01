---
mathLink: auto
Date created: 2024-10-21 18:57
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: [[Laplace or cofactor expansion]]
References: _Not applicable_
Justifications: [[Left and right inverse of a matrix]], [[Determinant of a matrix (explicit permutative definition)]], [[Adjugate matrix]], [[Cofactor of a matrix in the i'th row and j'th column]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Explicit formula for the inverse of a matrix
> Let $A\in M_{n\times n}(F)$ with $\det (A)\neq 0$, then $$ A^{-1}=\frac{1}{\det(A)}\text{adj}(A) $$

>[!quote] Proof: Explicit formula for the inverse of a matrix
>It suffices to show that $$ A \cdot \text{adj}(A)=\text{adj}(A)\cdot A=\det(A)\mathbb{I}_{n} $$We only prove that $A \cdot \text{adj}(A)=\det(A)\mathbb{I}_{n}$ since the other part is symmetric. Notice that for diagonal elements $$ (A\cdot \text{adj}(A))_{ii}=\sum^{n}_{k=1}a_{ik}\mathfrak C_{ik}=\det(A) $$For non diagonal elements on the other hand we are going to show that $(A\cdot \text{adj}(A))_{ij}=0$. Consider $$ (A\cdot \text{adj}(A))_{ij}=\sum^{n}_{k=1}a_{ik}\mathfrak C_{jk} $$Notice that this is exactly the determinant of our matrix $A$ if $R_{j}$ was replaced by $R_{i}$. But that matrix would have zero determinant, thus $\sum^{n}_{k=1}a_{ik}\mathfrak C_{jk}=0$ and $(A\cdot \text{adj}(A))_{ij}=0$. This proves that $$ A \cdot \text{adj}(A)=\det(A)\mathbb{I}_{n} $$
>
>**Q.E.D.**

