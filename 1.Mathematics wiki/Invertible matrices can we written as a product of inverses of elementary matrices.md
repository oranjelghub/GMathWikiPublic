---
mathLink: auto
Date created: 2024-09-10 19:20
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: [[Elementary matrices are invertible]]
References: _Not applicable_
Justifications: [[Left and right inverse of a matrix]], [[Elementary matrices]], [[Row equivalence]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Invertible matrices can we written as a product of inverses of elementary matrices
> Let $A\in M_{n\times n}(F)$ be a invertible matrix, then for some sequence of elementary matrices $(E_{i})^{n}_{i=1}$ $$ A=\prod^{n}_{i=1}(E_{i})^{-1} $$

Equivalently, the assumption that $A$ is invertible can be replaced by the assumption that $A$ is row equivalent to $\mathbb{I}_{n}$.

>[!quote] Proof: Invertible matrices can we written as a product of inverses of elementary matrices
>Notice that since $A$ is invertible that the only solution to $AX=0$ is the trivial one, since $$ AX=0 \implies X=\mathbb{I}_{n}*X=(A^{-1}*A)*X=A^{-1}*0=0$$Meaning that $A$ must be row equivalent to $\mathbb{I}_{n}$, otherwise a contradiction would follow to the amount of solutions of $AX=0$. It follows that for some sequence of elementary matrices $(E_{i})^{n}_{i=1}$ we have $$ \left( \prod^{n}_{i=1}E_{n-i+1} \right)*A=\mathbb{I}_{n} $$It obviously follows that $$ A=\prod^{n}_{i=1}(E_{i})^{-1} $$
>
>**Q.E.D.**
