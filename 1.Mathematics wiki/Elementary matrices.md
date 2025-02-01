---
mathLink: auto
Date created: 2024-08-30 21:31
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Row equivalence]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Matrix multiplication]]

---

Let $A\in M_{n\times m}(F)$ and $\lambda \in F$ non-zero. We define the following elementary row operations as 

>[!quote]- Definition: Switching the $i$'th and $j$'th row 
>$$A\mapsto C_{ij}A$$ Where $C_{ij}\in M_{n\times n}(F)$ and $$ C_{ij}=\begin{bmatrix}1&&&&&&&\\&\ddots&&&&&&\\&&0&&&1&&&\\&&&\ddots&&&&\\&&1&&&0&&\\&&&&&&\ddots&\\&&&&&&&1\end{bmatrix}$$With coefficients given by $$ (C_{i,j})_{k,l}=\left\{\begin{matrix}{0}&{k\neq i,k\neq j,k\neq l}\\{1}&{k\neq i,k\neq j,k=l}\\{0}&{k=i,l\neq j}\\{1}&{k=i,l=j}\\{0}&{k=j,l\neq i}\\{1}&{k=j,l=i}\\\end{matrix}\right. $$

>[!quote]- Definition: Multiplying the $i$'th row by a scalar
>$$ A\mapsto M_{i}(\lambda) $$Where $M_{i}(\lambda)\in M_{n\times n}(F)$ and $$ M_{i}(\lambda)=\begin{bmatrix}1&&&&&&\\&\ddots&&&&&\\&&1&&&&\\&&&\lambda&&&\\&&&&1&&\\&&&&&\ddots&\\&&&&&&1\end{bmatrix} $$With coefficients given by $$ (M_{i}(\lambda))_{kl}=\left\{\begin{matrix}0&k\neq l\\1&k=l,k\neq i\\\lambda &k=l,k=i\end{matrix}\right. $$

>[!quote]- Definition: Adding the scaled $j$'th row to the $i$'th row
>$$ A\mapsto S_{ij}(\lambda)A $$
Where $S_{ij}(\lambda)\in M_{n\times n}(F)$ and $$ S_{ij}(\lambda)=\begin{bmatrix}1\\&\ddots\\&&1\\&&&\ddots\\ &&\lambda&&1  \\ &&&&&&\ddots\\&&&&&&&1\end{bmatrix} $$With coefficients given by $$ (S_{ij}(\lambda))_{kl}=\left.\left\{\begin{array}{ll}{0}&{k\neq l,k\neq i,l\neq j}\\{1}&{k=l}\\{\lambda}&{k=i,l=j}\\\end{array}\right.\right. $$

We denote the set of all elementary matrices of $A$ as
$$ \mathbf{E}(A) $$