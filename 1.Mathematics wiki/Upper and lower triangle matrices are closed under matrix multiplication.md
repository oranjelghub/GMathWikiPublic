---
mathLink: auto
Date created: 2024-09-10 19:44
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: [[Matrix multiplication]]
References: _Not applicable_
Justifications: [[Upper and lower triangle matrices]] 

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Upper and lower triangle matrices are closed under matrix multiplication
> Let $A,B,C,D\in M_{n\times n}(F)$ such that $A$ and $B$ are upper triangle matrices and $C$ and $D$ are lower triangle matrices, then $A*B$ is a upper triangle matrix and $C*D$ is a lower triangle matrix.

 >[!quote] Proof: Upper and lower triangle matrices are closed under matrix multiplication
 >We only analyse the case $A*B$ since the proof for $C*D$ is symmetric. Let $1\leq i\leq n$ and $1\leq j\leq n$ and $j<i$, then $$ (A*B)_{ij}=\sum^{n}_{k=1}a_{ik}b_{kj}=\sum^{j}_{k=1}0b_{kj}+\sum^{n}_{k=j+1} a_{ik}0=0$$Thus $A*B$ is a upper triangle matrix.
 >
 >**Q.E.D.**
 
 