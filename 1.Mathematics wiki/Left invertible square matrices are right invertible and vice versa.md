---
mathLink: auto
Date created: 2024-09-10 18:47
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: [[Elementary matrices are invertible]], [[Invertible matrices can we written as a product of inverses of elementary matrices]]
References: _Not applicable_
Justifications: [[Left and right inverse of a matrix]], [[Row equivalence]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Left invertible square matrices are right invertible and vice verse
> Let $A\in M_{n\times n}(F)$ then $B$ is a left inverse of $A$ if and only if $B$ is a right inverse of $A$.

>[!quote] Proof: Left invertible square matrices are right invertible and vice verse
>Notice that since $A$ is left invertible that the only solution to $AX=0$ is the trivial one, since $$ AX=0 \implies X=\mathbb{I}_{n}*X=(B*A)*X=B*0=0$$Meaning that $A$ must be row equivalent to $\mathbb{I}_{n}$, otherwise a contradiction would follow to the amount of solutions of $AX=0$. This means that $A$ can be written as $$ A=\prod^{k}_{i=1} (E_{i})^{-1} $$For some sequence $(E_{i})^k_{i=1}$ of elementary matrices. It follows that $A$ has right inverse $$ \prod^{k}_{i=1}E_{n-i+1} $$And since $A$ is square and has a right and left inverse, we must have $B= \prod^{k}_{i=1}E_{k-i+1}$ and it follows that indeed $B$ is a right inverse of $A$. We can prove the statement the other way around by noticing that $AB=\mathbb{I}_{n}$ also implies that $B$ has left inverse $A$, thus the same arguments apply and $BA=\mathbb{I}_{n}$, which proves $A$ has a left inverse $B$.
>
>**Q.E.D.**

