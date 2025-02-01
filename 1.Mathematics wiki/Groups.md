---
mathLink: auto
Date created: 2023-10-23 18:58
tags:
  - Type/Object
  - Topic/Abstract_Algebra
cssclasses:
---

---  

Types: [[Cyclic groups]]
Examples: [[Dihedral group]], [[Modular group]], [[General linear group]], [[N fold reals]]
Construction: [[Homomorphisms]], [[Group isomorphism]]
Generalization: _Not applicable_

Properties: [[Properties of groups]], [[Order of a group and group elements]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Ordered pairs and n-tuples]], [[Sets]], [[Functions]], [[Binary operations]]

---  

> [!quote] Definition: Group
> A group is a algebraic structure that is represented by a set $G$ and a [[Binary operations|binary operation]] on $G$ such that:
> - The operation is associative
> - The operation has an identity $e$
> - The operation has an inverse for every element in $G$

We often denote a group as an ordered pair constituted from a [[Sets|set]] and a [[Binary operations|binary operation]] $(G,f)$. From this we also define the notion of an Abelian group:

>[!quote] Definition: Abelian group
>A group $(G,f)$ is said to be Abelian if and only $(G,f)$ is a group and $f$ is commutative: $f(a,b)=f(b,a)$

We also quickly mention the often used notation used in books when handling arbitrary [[Binary operations]].

>[!quote]- Notion: Notation regarding operations
>We denote the following for an arbitrary operation $f$ of a group where $f(a,b)=a\circ b$
>- $a\circ b=ab$ 
>- $a\circ a\circ\ldots\circ a=a^n$
>- $a^{-1}\circ a^{-1}\circ\ldots\circ a^{-1}=a^{-n}$
>- $x^0=e$

From this we can prove a lot of the classic properties of [[Exponentiation]] using techniques such as a recursive definition or the [[General law of associativity]]. Now since **SOME** of the properties require additional conditions we will explicitly list them.
- $x^{a+b}=x^{a}+x^b$ and $(x^a)^b=x^{ab}$
- $x^{-a}=(x^a)^{-1}$

Both of the above properties generalize to any integers



