---
mathLink: auto
Date created: 2025-02-11 21:35
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Measure_Theory
cssclasses:
---
---  

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Sigma-algebra]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Sigma-algebra (Properties)
> Let $\Omega$ be some set and $\sigma$ some sigma algebra on $\Omega$. Then the following claim hold:
> 1. $$ \emptyset \in \sigma $$
> 2. $$ \forall n \in \mathbb{N}: A_{n} \in \mathcal{A} \implies \bigcap_{n\in \mathbb{N}}A_{n} \in \mathcal{ A} $$
> 3. $$ A,B \in \sigma \implies B\backslash A \in \sigma $$

>[!quote] Proof: Sigma-algebra (Properties)
>1 follows from the fact that $\Omega \backslash\Omega = \emptyset$. 2 follows from the definition of a sigma algebra by writing $$ \bigcap_{n \in \mathbb{N}}A_{n} = \left( \bigcup_{n \in \mathbb{N}}A_{n}^{c} \right)^{c} $$ 3 follows directly from writing $B \backslash A$ as $B \cap A ^{c}$.
>
>**Q.E.D.**
