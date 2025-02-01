---
mathLink: auto
Date created: 2024-12-08 14:40
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: [[Linear maps (Properties)]]
References: _Not applicable_
Justifications: [[Vector space isomorphism]], [[Linear maps]], [[Dimension of a vector space]]
Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Vector spaces are isomorphic if and only if they have the same dimension
> Let $V,W$ be two finite dimensional $F$-vector spaces. Then $\dim V= \dim W$ if and only if $V\cong W$.

>[!quote] Proof: Vector spaces are isomorphic if and only if they have the same dimension
>We start by assuming that $\dim V =\dim W$. Take a basis $\{ v_{i} \}_{1\leq i\leq n}$ of $V$ and a basis $\{ w_{i} \}_{1\leq i\leq n}$ of $W$. We can then define $L:V\to W$ by $L(v_{i}):=w_{i}$ and letting it induce it's uniquely associated linear map. It is not to hard to notice that this is a vector space isomorphism and thus. Suppose on the other hand that $V\cong W$. Then one could pretty easily show that if $\{ v_{i} \}_{1\leq i\leq n}$ is a basis that then $\{ L(v_{i}) \}_{1\leq i\leq n}$ is also a basis (where $L$ is a vector space isomorphism from $V$ to $W$). Thus $\dim V=\dim W$.
>
>**Q.E.D.**



