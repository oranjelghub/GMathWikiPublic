
---

mathLink: auto

---
Date created: 2023-11-29 15:36
Tags: #Type/Notion #Topic/Real_Analysis 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Supremum and infimum of sets of extended reals]]
Generalization: [[Ordering (binary relation)]]

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Real numbers]], [[Extended real numbers]], [[Ordering of the real numbers]]

---  

We define an ordering on the [[Extended real numbers]] as follows:

> [!quote] Notion: Ordering of the extended real numbers
> Given $x,y\in \bar{\mathbb R}$, we say $x\leq y$ when one of the three following hold:
> 1. $x,y\in\mathbb R$ and $x\leq y$ in the sense of the [[Ordering of the real numbers]].
> 2. $y=+\infty$
> 3. $x=-\infty$

We define $x<y$ to be equal to the statement $x\leq y\land x\neq y$.

We can verify that this relation satisfies the following properties:

>[!quote]- Notion: Properties of the ordering of the extended real numbers
>- $x\leq x$
>- Exactly one of the following is true at all times:
>	- $x<y$
>	- $x=y$
>	- $x>y$
>- $x\leq y\land y\leq z\implies x\leq z$
>- $x\leq y\implies -x\geq -y$


