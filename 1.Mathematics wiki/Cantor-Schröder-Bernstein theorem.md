---
mathLink: auto
Date created: 2024-04-30 17:33
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Existence of an injection to a subset implies equal cardinality of the set and subset (infinite donut lemma)]]
References: _Not applicable_
Justifications: [[Cardinality of a set]], [[Sets]], [[Functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Cantor-Schröder-Bernstein theorem
> Given two sets $A$ and $B$, if there exists a injection $f:A\to B$ and a injection $g: B\to A$ then $\left| A \right|=\left| B \right|$.

>[!quote] Proof: Cantor-Schröder-Bernstein theorem
>Suppose we have our injective functions $f:A\to B$ and $g:B\to A$. Notice that $g\circ f: A\to A$ is an injection, and that more specifically $\tilde{g\circ f}:A\to g(B)$ is one as well. By the infinite donut lemma this implies that $\left| A \right|=\left| g(B) \right|$, and since we can restrict the range of $g$ such that $\tilde{g}:B\to g(B)$ is a bijection as well, we have that $\left| B \right|=\left| g(B) \right|$ and thus $\left| A \right|=\left| B \right|$
>
>**Q.E.D.**

