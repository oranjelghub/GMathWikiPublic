---
mathLink: auto
Date created: 2024-04-30 16:42
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Sets]], [[Power sets]], [[Functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Cantor's theorem
> There does not exist a bijection $f$ from a set $X$ to it's power set $\mathcal{P}(X)$.

>[!quote] Proof: Cantor's theorem
>Suppose for the sake of contradiction that there existed some bijection $f:X\to \mathcal{P}(X)$. Define $$ A:= \{ x\in X: x\notin f(x) \} $$ Since $A\in \mathcal{P}(X)$ we know that $f^{-1}(A)\in X$. We now ask what the membership status of $f^{-1}(A)$ is regarding $A$. If $f^{-1}(A)\in A$ then by definition of $A$ we have that $f^{-1}(A)\notin A$, and if $f^{-1}(A) \not\in A$ then by definition of $A$ we have that $f^{-1}(A)\in A$. Which are both contradictive, and thus our original assumption must be wrong.
>
>**Q.E.D.**


