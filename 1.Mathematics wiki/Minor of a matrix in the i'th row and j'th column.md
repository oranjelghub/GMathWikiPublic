---
mathLink: Minor of a matrix in the $i$'th row and $j$'th column
Date created: 2024-10-19 21:57
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: _Not applicable_ 
Examples: _Not applicable_
Construction: [[Cofactor of a matrix in the i'th row and j'th column]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Determinant of a matrix (explicit permutative definition)]]

---

> [!quote] Definition: Minor of a matrix in the i'th row and j'th column
> Let $A\in M_{n\times n}(F)$, then we define the minor in the $i$'th row and $j$'th column by $$ m_{ij}:= \det(A_{\cancel{ ij }}) $$ Where $A_{\cancel{ ij }}$ is defined by $$ (A_{\cancel{ ij }})_{lk} := \left\{ \begin{align}  &(A)_{lk}  & l<i \land k<j \\ & (A)_{l(k+1)} & l< i \land k\geq j \\ & (A)_{(l+1)k} & l\geq i \land k< j \\ &(A)_{(l+1)(k+1) } & l\geq i \land k\geq j\end{align} \right.  $$



