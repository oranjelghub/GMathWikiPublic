---
mathLink: auto
Date created: 2023-12-22 14:51
tags:
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---  

Proved by: [[Dimension of a vector space (Properties)]]
References: [[Bases of vector spaces]], [[Linear dependence and independence]]
Justifications: [[Dimension of a vector space (Properties)]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Proof:
> 2. We can algorithmically construct a finite basis for $U$, using a algorithm which will terminate since $U\subset_{\text{vec}}V$. Thus $\dim U \leq \dim V$.
> 3. We first prove that $\dim U =\dim V \implies U=V$. The inclusion $U\subset V$ is obvious since $U$ is a vector subspace of $V$. Now take some basis $\beta$ of $U$, since $\beta$ is free and $\left| \beta \right|=\dim V$, $\beta$ is also a basis for $V$. Implying that any vector of $v$ can we written as a linear combination of vectors of $U$. Thus $V\subset U$ and we are done. The other implication is trivial.
> 4. 
> **Q.E.D.**

