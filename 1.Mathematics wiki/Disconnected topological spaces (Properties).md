---
mathLink: auto
Date created: 2024-07-15 00:55
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Topology
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Connected and disconnected topological spaces]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem:
> 1. Let $(T,\tau)$ be a topological space and $(S,\theta)$ a topological subspace of $T$. If $S$ is disconnected and $A,B\subseteq S$ form a disconnection of $S$ then $$ \text{Cl}_{S}\:A \cap B = \emptyset$$

>[!quote] Proof
>1. We argue by contradiction. Suppose there was some $x\in \text{Cl}_{S}\:A$ such that $x\in B$. Since $B$ is open and contains $x$ we must have by the definition of adherent point that $B\cap A \neq \emptyset$, but this is an immediate contradiction to the fact that $A,B$ is a disconnection of $S$.



