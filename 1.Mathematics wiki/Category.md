
---

mathLink: auto

---
Date created: 2023-12-05 12:41
Tags: #Type/Object #Topic/Category_Theory 

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Classes]]

---  

A category is an abstract object, often referred to as a frame for certain mathematics.

> [!quote] Definition: Category
> A category $C$ is a [[Classes|class]] of objects denoted $\text{ ob}(C)$ and a [[Classes|class]] of structure preserving maps called morphisms denoted $\text{mor}(C)$.

Notice that categories and category theory in general doesn't use axioms. It assumes that one defines a specific category using axioms, like ZFC for example, in such a manner that it falls under the definition of a category.

We also have a law of composition, identity and associativity that must hold: 

>[!quote]- Law of composition 
>Given three objects $A$,$B$,$C$ and morphisms $A\to B$ and $B\to C$, the composition must exist. 
>
>![[diagram-20231205 (2).svg#invert_B]]

>[!quote]- Law of identity
>For every object $A$ there is a morphism $\text{id}_{A}$ that maps $A$ to itself.
>
>![[diagram-20231205 (4).svg#invert_B]]

>[!quote]- Law of associativity
>Given morphisms $f$,$g$,$h$ we must have that: $$ f\circ(g\circ h)=(f\circ g)\circ h
$$

