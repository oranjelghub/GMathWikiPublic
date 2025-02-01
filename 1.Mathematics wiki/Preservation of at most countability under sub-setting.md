
---

mathLink: auto

---
Date created: 2024-03-14 16:04
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis #Topic/Set_Theory 

Proved by: [[Decreasing bijection on infinite subsets of N]]
References: _Not applicable_
Justifications: [[Cardinality of a set]], [[Natural numbers]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Preservation of at most countability under sub-setting
> If $X$ is an at most countable set and $Y\subseteq X$ then $Y$ is also at most countable.

>[!quote] Proof: Preservation of at most countability under sub-setting
>Since $X$ is at most countable we know there is some bijection $f:X\to \mathbb{N}$, notice that the following restriction preserves the bijectivity of the map $$ f':Y\to f(Y): x\mapsto f(x) $$ So $Y$ has the same cardinality as $f(Y)$, but since every subset of the natural numbers is at most countable by: [[Decreasing bijection on infinite subsets of N]], we also know that $f(Y)$ and $Y$ are at most countable.
>
>**Q.E.D.**



