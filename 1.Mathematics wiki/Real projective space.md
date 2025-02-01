
---

mathLink: auto

---
Date created: 2024-01-15 11:46
Tags: #Type/Object #Topic/Topology 

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: [[Topological spaces]]

---  

This topological space is defined as follows

> [!quote] Definition: Real projective space
> We define the real projective space by the set 
> $$ \mathbb RP^n:=\{l\subset \mathbb R^{n+1}: l\;\text{is a straight line through the origin}\} $$
>  where we consider a set $S\subset \mathbb RP^n$ to open if and only if $\bigcup_{l\in S} l\backslash\{0\}$ is open in $\mathbb R^{n+1}\backslash\{0\}$.

The reason we omit zero is because one can quickly check that not doing so endows the space with the indiscrete topology, which is not very interesting.
