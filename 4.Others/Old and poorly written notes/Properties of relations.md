




---

mathLink: auto

---
Date created: 2023-10-24 15:21
Tags: #Type/Unfinished 

%%For Definition/Example of a notion/object%%

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

%%For Proposition/Theorem of a notion/object including both`statement`/`proof` regarding `object`/`notion` it links to %%

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---  



> [!quote] Definition
> Lorem ipsum dolor sit amet









- $(R^{-1})^{−1} = R$ 
- $\text{Dom}(R^{-1}) = \text{Ran} (R)$
- $\text{Ran}(R^{-1}) = \text{Dom}(R)$ 
- $T\circ (S \circ R) = (T \circ S) \circ R$ 
- $(S\circ R)^{-1} = R^{−1}\circ S^{-1}$

There are also 3 other notions that are relevant to relations.

- Reflexivity: $\forall a\in A: (a,a)\in R$ or $R=R^{-1}$
- Symmetry: $\forall x,y\in A:(x,y)\in R\implies (y,x)\in R$ or $\imath_A \subseteq R$ where is is kind of an identity relation, like the [[Inclusion and identity maps]].
- Transitivity: $\forall x,y,z \in A: (x,y)\in R\land (y,z) \in R\implies (x,z)\in R$  or $R\circ R\subseteq R$ 

Suppose $R$ is a relation on a set $A$. Then $R$ is called a partial order on $A$(or just a partial order if $A$ is clear from context) if it is reflexive, transitive, and antisymmetric. It is called a total order on $A$ (or just a total order) if it is a partial order, and in addition it has the following property: $∀x ∈ A ∀y ∈ A:xRy ∨ yRx$ 
Suppose $R$ is a partial order on a set $A$, $B ⊆ A$, and $b ∈ B$. Then $b$ is called an $R$-smallest element of $B$ (or just a smallest element if $R$ is clear from the context) if $∀x ∈ B:bRx$. It is called an $R$-minimal element (or just a minimal element) if $¬∃x ∈ B:xRb ∧ x = b$.

#comeback  on the bit of ordered relations.