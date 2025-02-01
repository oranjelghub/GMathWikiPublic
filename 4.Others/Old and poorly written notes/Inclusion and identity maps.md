
---

mathLink: auto

---
Date created: 2023-11-24 22:41
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

[[Properties of inclusion and identity maps (Proof)]]

> [!quote] Definition
> Lorem ipsum dolor sit amet





If $X$ is a subset of $Y$ , let $\imath_{X→Y} : X → Y$ be the inclusion [[Functions|map]] from $X$ to $Y$ , defined by mapping $x \mapsto x$ for all $x ∈ X$, i.e., $\imath_{X→Y} (x) := x$ for all $x ∈ X$. The map $\imath_{X→X}$ is in particular called the identity map on $X$.

## Properties

- For any $f:A \rightarrow B$ we got: $$f=f\circ \imath_{A\rightarrow A} = \imath_{B\rightarrow B}\circ f \hspace{1cm} (1)$$
- For [[Sets|sets]] $X$,$Y$,$Z$ we got: $$X\subseteq Y \subseteq Z \implies \imath_{Y \rightarrow Z}\circ\imath_{X\rightarrow Y}=\imath_{X\rightarrow Z}\hspace{1cm} (2)$$
- if $f : A → B$ is a bijective function, then: $$f\circ f^{−1} = \imath_{B→B} \;\land\; f^{−1} \circ f = \imath_{A→A} \hspace{1cm}(3)$$
- if $X$ and $Y$ are disjoint sets, and $f : X → Z$ and $g : Y → Z$ are functions, then there is a unique function $h : X \cup Y → Z$ such that: $$h \circ \imath_{X→X\cup Y} = f \;\land\; h \circ \imath_{Y →X\cup Y} = g\hspace{1cm}(4)$$


