---
mathLink: Connected subsets of $\mathbb R$ (Terence Tao Analysis I)
Date created: 2024-07-15 21:32
tags:
  - Type/Object
  - Type/Proof
  - Topic/Topology
  - Topic/Real_Analysis
cssclasses:
---

---  

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: [[Connected and disconnected topological spaces]]

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: [[Connected and disconnected topological spaces]]
Justifications: [[A set is connected in R if and only if it is a interval]]

---

> [!quote] Definition: Connected subsets of R (Terence Tao Analysis I)
> A set $X\subseteq \mathbb{R}$ is said to be connected if and only if $\forall x,y \in X,\: [x,y]\subseteq X$

We provide a proof that this definition is equivalent to the classic one.

>[!quote] Proof: Equivalence between Tao connectedness and classical connectedness
>Let $X\subseteq \mathbb{R}$ be a classically connected set, then we know $X$ is a interval and intervals are obviously Tao connected. Now suppose $X$ is some Tao connected set that isn't classically connected. Then there are some open $A,B$ such that $A\cup B=X$ and $A\cap B=\emptyset$. Fix some arbitrary $a\in A$ and $b\in B$ such that $a<b$ and consider $J:=[a,b]$. Notice that if we define $A':=A\cap J$ and $B':= B\cap J$ then we have that $A',B'$ form a disconnection of $J$ since they are both open, $A'\cap B'=\emptyset$ since $A\cap B=\emptyset$ and $$ A'\cup B'=(A\cup B)\cap J =X\cap J$$But since $X$ is Tao connected we have that $X\cap J=J$. But this means that the classical disconnection of $X$ implies the classical disconnection of $J$, but $J$ is an interval and thus classically connected, a contradiction. Thus $X$ must be classically connected.
>
>**Q.E.D.**




