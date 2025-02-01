---
mathLink: auto
Date created: 2024-11-11 14:48
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Dimension of a vector space]], [[Bases of vector spaces]], [[Span of a subset of a vector space]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Dimension of sum of vector spaces
> LLet $V$ be a finite dimensional vector space. Then if $U$ and $W$ are some vector subspaces of $V$, we have $$ \dim (U+W)+\dim (U\cap W)=\dim U + \dim W $$

>[!quote] Proof: Dimension of sum of vector spaces
>We define $\dim U=r$, $\dim W=s$ and $\dim U\cap W=t$. We know that $t\leq s$ and $t \leq r$. Now take some basis $\beta$ of $U\cap W$. We can expand that basis with $r-t$ vectors to a basis $\beta_{U}$ of $U$ or with $s-t$ vectors to a basis $\beta_{W}$ of $W$. We now claim that $\beta_{U}\cup\beta_{W}$ is a basis of $U+W$. It is pretty obvious that $\beta_{U}\cup\beta_{W}$ spans $U+W$. We now also want to show they are all free, in other words we want to show that $$ \sum^{t}_{i=1}\alpha_{i}v_{i}+\sum^{r}_{j=1}\beta_{j}u_{j}+\sum^{s}_{k=1}\gamma_{k}w_{k}=0 $$If and only if all the coefficients are zero. We can write this as $$\sum^{s}_{k=1}\gamma_{k}w_{k}=-\sum^{t}_{i=1}\alpha_{i}v_{i}-\sum^{r}_{j=1}\beta_{j}u_{j}$$This implies that $\sum^{s}_{k=r+1}\gamma_{k}w_{k}\in U \cap W$ and since $\beta$ is a basis of $U\cap W$ we know that we can write the left sum as $$ \sum^{s}_{k=1}\gamma_{k}w_{k}=\sum^{t}_{i=1}\lambda_{i}v_{i} $$ Implying that $\sum^{s}_{k=1}\gamma_{k}w_{k}-\sum^{t}_{i=1}\lambda_{i}v_{i}=0$. But all the vectors in this sum are just the basis vectors $\beta_{W}$. Thus all coefficients must be zero, specifically all the $\gamma$'s. We are now left with $$ \sum^{t}_{i=1}\alpha_{i}v_{i}=\sum^{r}_{j=1} \beta_{j}u_{j}$$We can apply the same argument to prove that all k$\alpha$ and $\beta$ must be zero. This means that the vectors of $\beta_{U}\cup\beta_{W}$ are free. It now follows directly that $$  \dim (U+W)+\dim (U\cap W)=\dim U + \dim W$$
>
>**Q.E.D.**

