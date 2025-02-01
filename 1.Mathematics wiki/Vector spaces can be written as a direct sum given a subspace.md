---
mathLink: auto
Date created: 2023-12-22 14:33
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by:  _Not applicable_
References: _Not applicable_
Justifications: [[Vector subspaces]], [[Sum and direct sum of vector spaces]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Vector spaces can be written as a direct sum given a subspace
> Let $V$ be a finite dimensional vector space and let $W$ be a subspace of $V$. Then there exists a subspace $U$ such that: $$V= W \oplus U$$

>[!quote] Proof: Vector spaces can be written as a direct sum given a subspace
>We know that $W$ has a basis $\{ w_{i} \}_{1\leq i\leq n}$ we know that this is not a maximal subset of $V$ meaning that there exists a vector $w_{n+1}$ such that $\{ w_{i} \}_{1\leq i\leq n+1}$ is a set of linearly independent vectors. Since we have that the dimension of $V\backslash\{ w_{i} \}$ is a strictly reducing sequence we must have that this process of picking vectors eventually terminates. Giving us a set of vectors $\{ w_{i} \}_{n+1\leq i\leq m}$ which forms a basis for a vector subspace $U$. We can now easily notice that $V= W \oplus U$.
>
>**Q.E.D.**

