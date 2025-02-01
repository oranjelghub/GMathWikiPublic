---
mathLink: auto
Date created: 2024-11-10 22:01
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Bases of vector spaces]], [[Linear dependence and independence]], [[Span of a subset of a vector space]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Bases of finite dimensional vector spaces are maximally free and minimally spanning
> Let $V$ be a $F$-vector space then the following statements are equivalent:
> 1. $\beta$ is a basis of $V$
> 2. $\beta$ is maximally free
> 3. $\beta$ minimally spans $V$

>[!quote] Proof: Bases of finite dimensional vector spaces are maximally free and minimally spanning
>We will only show  here that 1 and 2 are equivalent. Suppose $\beta$ is a basis, and suppose for the sake of contradiction that there existed some set $\beta \subset\alpha$ such that all vectors of $\alpha$ are free. Then there exists some $\alpha_{0}\in \alpha \backslash \beta$. $\beta$ is a basis thus $$ \sum^{n}_{i=1}\mu_{i}\beta_{i}=\alpha_0 $$Meaning that $\alpha$'s vectors are not actually free, thus $\beta$ must be maximally free. Now suppose that instead $\beta$ mas maximally free, we want to show that $\beta$ is a basis. To do this fix some $v\in V$. If $v\in \beta$ then $v\in \text{span}(\beta)$ and we are done, if instead $v\not \in \beta$ then $\beta \cup \{ v \}$ is not free since $\beta$ is maximally free. Thus there is some non trivial solutions to $$ \lambda v+\sum^{n}_{i=1}\mu_{i}\beta_{i}=0 $$Where $\lambda$ can't be equal to zero. But then $v$ is a linear combination of $\beta$, meaning that $v\in \beta$. The equivalence of 1 and 3 we will not show, in the spirit it is similar to the above proof.
>
>**Q.E.D.**

