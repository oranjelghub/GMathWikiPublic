---
mathLink: auto
Date created: 2025-01-17 19:15
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---
---  

Proved by: [[Induction]]
References: _Not applicable_
Justifications: [[Eigenvalues and eigenvectors of a linear transformation]], [[Linear dependence and independence]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Eigenvectors with different eigenvalues are free
> Let $V$ be a $n$-dimensional $\mathbb{C}$-vector space and $L:V\to V$ a linear transformation. Suppose $\{ v_{i} \}_{1\leq i\leq k}$ is a set of eigenvectors with all different eigenvalues. Then $\{ v_{i} \}_{1\leq i\leq k}$ is free.

>[!quote] Proof: Eigenvectors with different eigenvalues are free
>We proceed by induction on $k$. If $k=1$ then the set is obviously free. Suppose for the induction hypothesis that $\{ v_{i} \}_{1\leq i\leq k}$ is free where all the vectors are eigenvectors with different eigenvalues. Suppose we now add another eigenvector vector $v_{k+1}$ with eigenvalue $\lambda_{k+1}$. We want to show that $\{ v_{i} \}_{1\leq i\leq k+1}$ is free. Suppose that $$ \sum^{k+1}_{i=1}\alpha_{i}v_{i}=0 $$We want to prove that all the $\alpha_{i}$ must be zero. Notice that if $\alpha_{k+1}$ is zero then the statement directly follows form the induction hypothesis. So it suffices to proof that $\alpha_{k+1}\neq 0$ leads to a contradiction. If $\alpha_{k+1}\neq 0$ then we may write $$ v_{k+1}=\sum^{k}_{i=1}- \frac{\alpha_{i}}{\alpha_{k}}v_{i} $$We may apply $L$ on both sides once and also just multiply by the eigenvalue $\lambda_{k+1}$. This leaves us with $$ \begin{align} L(v_{k+1})&=\sum^{k}_{i=1}- \frac{\alpha_{i}\lambda_{i}}{\alpha_{k}}v_{i} \\   \lambda_{k+1} v_{k+1}  &= \sum^{k}_{i=1}- \frac{\alpha_{i}\lambda_{k+1}}{\alpha_{k}}v_{i}\end{align} $$If we now subtract both these equations from each other we get $$ 0=\sum^{k}_{i=1}- \frac{\alpha_{i}}{\alpha_{k}}(\lambda_{i}-\lambda_{k+1})v_{i} $$But since all the eigenvalues are different their difference is non-zero. It follows by the induction hypothesis that all $\alpha_{i}$ must be zero. But then $v_{k+1}=0$ and thus not a eigenvector, which is a contradiction. This closes the induction.
>
>**Q.E.D.**

