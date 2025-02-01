---
mathLink: auto
Date created: 2024-09-10 19:35
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: _Not applicable_ 
Examples: _Not applicable_
Construction: [[LU-decomposition of invertible matrices]]
Generalization: _Not applicable_

Properties: [[Upper and lower triangle matrices are closed under matrix multiplication]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Matrices]]

---

> [!quote] Definition: Upper and lower triangle matrices
> Let $A\in M_{m\times n}(F)$, we say that $A$ is a upper triangle matrix if and if $$ \forall 1\leq i\leq m\; \forall 1\leq j\leq n,\; j<i\implies (A)_{ij}=0 $$Similarly $A$ is said to be a lower triangle matrix if and only if $$   \forall 1\leq i\leq m\; \forall 1\leq j\leq n,\; i<j\implies (A)_{ij}=0$$

Notice that all elementary matrices, with exception to the row switching elementary matrix $C_{ij}$, are lower triangle matrices. Also an example of a upper triangle matrix: $$ \begin{bmatrix}
0& a_{12}&a_{13}\\0&0& a_{23}\\ 0&0&0\end{bmatrix} $$

