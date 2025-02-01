
---

mathLink: auto

---
Date created: 2023-11-26 23:35
Tags: #Type/Notion #Topic/Linear_Algebra 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Span of a subset of a vector space]], [[Linear dependence and independence]]
Generalization: _Not applicable_

Properties: [[Test for linear combinations]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: _Not applicable_

---  

We define linear combinations of vectors as follows:

> [!quote] Notion: Linear combinations of vectors
> Let $V$ be a [[Vector spaces|vector space]] over a [[Fields|field]] $F$. A linear combination of vectors of $V$ is defined as: $$\sum_{1\leq i\leq n}f_i*v_i$$

Where obviously $f_i$ is a scalar in $F$ and $v_i$ is a vector in $V$. We sometimes specify the set of vectors used, and say that we have a linear combination of the vectors $V'$.

We thus say a vector $v$ is a linear combination of vectors $V'$ if there exists $\text{card}(V')$ scalars $f$ such that: $$v=\sum_{1\leq i\leq\text{card}(V')}f_i*v_i$$We can then also denote the set off all linear combinations of vectors of $V'$: $$\text{Span}(V')=\left\{v:v=\sum_{1\leq i\leq\text{card}(V')}f_i*v_i \;\text{with}\; v_i\in V'\land (f_i)_{1\leq i\leq n}\in \prod_{1\leq i\leq n} F\right\}$$
