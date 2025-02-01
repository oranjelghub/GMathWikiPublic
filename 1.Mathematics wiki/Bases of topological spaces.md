
---

mathLink: auto

---
Date created: 2023-12-26 22:27
Tags: #Type/Notion #Topic/Topology 

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: [[Preimage of base elements as condition for continuity]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications:  [[Topological spaces]]

---  

Just like the [[Bases of vector spaces]], we encapsulate the same idea in the topological context as follows:

> [!quote] Notion: Basis of a topological space
> A set $\mathcal B$ is said to form a basis for the topological space $(T,\tau)$ if and only if every $\tau_{i}\in \tau$ can be written as a union of elements of $\mathcal B$: $$\forall \tau_{i}\in \tau \;\exists \mathcal F \subseteq  \mathcal B: \tau_{i}=\bigcup \mathcal F$$

We can generate a topology by considering the following set and topology:

>[!quote] Notion: Generated topology
>By defining the generated topology $\tau(\mathcal B)$
>$$\tau(\mathcal{B}):=\{U:U=\bigcup_{B\in\mathcal F}B,\; \text{for some}\; \mathcal F \subseteq \mathcal{B}\}$$
>with the additional condition
>$$ \forall t \in T\;\forall B_{1},B_{2}\in \mathcal B\;\exists B_{3}\in \mathcal B: t\in B_{3}\subseteq B_{1}\cap B_{2}$$
>We can create the topological space
>$$(\bigcup \mathcal  B, \tau(\mathcal B)) $$


