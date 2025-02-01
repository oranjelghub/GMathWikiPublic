---
mathLink: A set is connected in $\mathbb R$ if and only if it is a interval
Date created: 2024-07-15 15:25
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Topology
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Disconnected topological spaces (Properties)]]
References: _Not applicable_
Justifications: [[Connected and disconnected topological spaces]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: A set is connected in R if and only if it is a interval
> $X\subseteq \mathbb{R}$ is connected in $\mathbb{R}$ if and only if $X$ is a interval with endpoints $a,b\in \overline{\mathbb{R}}$.

>[!quote] Proof: A set is connected in R if and only if it is a interval
> First suppose $X$ is a interval, we want to show that $X$ is connected. We proceed by contradiction so suppose there was some disconnection $A,B$ of $X$. Then we have $A\cup B=X$ and $A\cap B=\emptyset$. Now fix some arbitrary $a\in A$ and $b\in B$ and define $J:=[a,b]$. Notice that $J$ must also be disconnected since $A_{1}:=J\cap A$ and $B_{1}:=J\cap B$ form a disconnection of $J$. Now define $c:=\sup A_{1}$, we have $c\in \overline A_{1}$ and thus $c\not\in B_{1}$ since $\overline A_{1} \cap B=\emptyset$. But if $x\in J$ and $c<x\leq b$ then by definition of $c$ we know $(x,b]\subset B_{1}$, notice that this implies that $c\in \overline B_{1}$, but then $c\not\in B_{1}$. But $c$ must be in $J$ since it is a closed set meaning it must be either in $A_{1}$ or $B_{1}$, which is not true, meaning we have a contradiction and there must not exist a disconnection for $X$. Now to prove the statement the other way, so suppose $X$ is not an interval. Then there must exist some $x,y\in X$ and $z\not\in X$ such that $x<z<y$ (Otherwise we can prove $X$ is an interval). Then notice that $A:=\{ p\in X: p<z \}$ and $B:=\{ p\in X : z<p\}$ form a valid disconnection of $X$. By contraposition this implies that if $X$ is connected then it is an interval. This closes the proof.
>
>**Q.E.D.**

