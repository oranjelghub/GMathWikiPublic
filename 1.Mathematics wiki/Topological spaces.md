
---

mathLink: auto

---
Date created: 2023-12-19 01:38
Tags: #Type/Object #Topic/Topology 

Types: [[Subspace or induced topological spaces]]
Examples: [[Real numbers]], [[Sn n-dimensional sphere topological space]], [[Metric spaces]], [[General linear group topology]], [[Real projective space]]
Construction: [[Continuity (Topological)]]
Generalization: [[Topology category]]

Properties: [[Bases of topological spaces]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: _Not applicable_

---  

We define one of the most general notion of a space in modern mathematics, the topological space.

> [!quote] Definition: Topological space
> Given a [[Sets|set]] $X$, we say that $\tau_{X} \subseteq \mathcal P(X)$ forms a topology over $X$ if and only if: 
> 1. $$ \emptyset, X \in \tau_{X}  $$
> 2. $$ \bigcup_{i\in I}\tau_{i}\in \tau_{X}  $$
> 3. $$ \bigcap_{i\in I}\tau_{i}\in \tau_{X} \land \text{Card}(I)=n $$ A set together with a topology over that set forms a topological space, formally denoted as an ordered pair. $$ (X,\tau_{X})$$
> We call the elements of the topology "open sets".

Given any set $S$ in $X$, we say $S$ is closed if and only if $X\backslash S\in \tau_{X}$.

Given any set $X$ we can construct two obvious topologies. One being the indiscrete topology: $$
(X,\{ X,\emptyset \})
$$And the other being the discrete topology: $$
(X,\mathcal P(X))$$
