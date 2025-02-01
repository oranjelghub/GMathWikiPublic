---
mathLink: Trichotomy of the solutions to the matrix equation $AX=B$
Date created: 2024-09-01 19:36
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Matrices]], [[Matrix multiplication]], [[Fields]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Trichotomy of the solutions to the matrix equation $AX=B$
> Let $A,B\in M_{n\times m}(F)$ with $F$ a non-finite field, then the equation $$ AX=B $$ has either:
> - No solution
> - One solution
> - Infinite solutions

>[!quote] Proof: Trichotomy of the solutions to the matrix equation $AX=B$
>Notice that we only have to show that $AX=B$ has an infinite amount of solutions if it has more than 1. So assume $AX=B$ has at least solutions $X_{1}$ and $X_{2}$. We define $$ X^{(\lambda)}:=X_{1}+\lambda(X_{2}-X_{1}) $$For some $\lambda\in F$, and notice that $$ AX^{(\lambda)}=A(X_{1}+\lambda(X_{2}-X_{1}))=AX_{1}+\lambda(AX_{2}-AX_{1}) =B$$And since the choice of $\lambda$ is arbitrary and there are infinite of them, the theorem is proven.
>
>**Q.E.D.**

