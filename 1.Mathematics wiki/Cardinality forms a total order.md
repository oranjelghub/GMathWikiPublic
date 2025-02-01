---
mathLink: auto
Date created: 2024-05-06 16:15
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Zorn's lemma]]
References: _Not applicable_
Justifications: [[Cardinality forms a partial order]], [[Axiom of choice]], [[Totally ordered set]], [[Cardinality forms a partial order]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Cardinality forms a total order
> Given two sets $A$ and $B$, if there does not exist an injection from $A$ to $B$, then there exists one from $B$ to $A$

This proof requires choice.

>[!quote] Proof: Cardinality forms a total order
>Let $P(X)$ denote the property: there exists a injective function from $X\to A$. We define $$ \mathcal{U}:=\{ X\in \mathcal{P}(B):P(X) \text{ is true} \} $$ Notice that $\mathcal{U}$ is non-empty. Now consider $(\mathcal{U},\subseteq)$ and take some totally ordered subset $T\subseteq \mathcal{U}$, notice that every $T$ is bounded above by $\bigcup T$, which by Zorn's lemma implies that there exists at least one maximal element in $\mathcal{U}$, denote it $\mathcal{J}$ and denote one injection $\mathcal{J}\to A$ as $\mathcal{L}$. We now argue that $\mathcal{ J}=B$. Which we will show by contradiction, so suppose $\mathcal{J}\neq B$. This means that $B\backslash\mathcal{J}$ is non empty so pick $b\in B\backslash\mathcal{J}$. Suppose we try to define a function $f:B\backslash\mathcal{J}\to A$, since there does not exist a injection $B\backslash\mathcal{J}\to A$ we know that $$ \forall a\in A\;\exists j\in J: f(b)=a=\mathcal{L}(j) $$ Now notice that this would imply that $\mathcal{L}$ is also surjective, and thus bijective. But this would contradict the original assumption that there does not exist an injection from $A\to B$, thus the assumption that $\mathcal{J}\neq B$ must be false and we know that there exists some injection from $B$ to $A$.
>
>**Q.E.D.**

