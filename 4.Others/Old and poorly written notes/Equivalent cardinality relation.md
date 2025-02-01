
---

mathLink: auto

---
Date created: 2023-12-21 14:16
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







The notion of having equal cardinality is an equivalence relation: Let $X$, $Y$ , $Z$ be sets. Then $X$ has equal cardinality with $X$. If $X$ has equal cardinality with $Y$ , then $Y$ has equal cardinality with $X$. If $X$ has equal cardinality with $Y$ and $Y$ has equal cardinality with $Z$, then $X$ has equal cardinality with $Z$.
	1. The bijection $x\mapsto x$ proves this
	2. If $X$ has the same cardinality as $Y$ then there is a bijection. By definition we then know that there is an inverse to that bijection which itself is a bijection. And thus we have a bijection from $Y$ to $X$ proving the statement
	3. We know there exists two bijections, one from $X$ to $Y$ and one from $Y$ to $Z$, since the composition of a bijection is also a bijection we have that there exists a bijection from $X$ to $Z$ thus proving the statement.

We can now formally define cardinality. Let $n$ be a natural number. A set $X$ is said to have cardinality $n$, if and only if it has equal cardinality with $\{i ∈ N : 1 ≤ i ≤ n\}$. We also say that $X$ has $n$ elements if and only if it has cardinality $n$.
	One can use the set $\{i ∈ N : i<n\}$ instead of $\{i ∈ N : 1 ≤ i ≤ n\}$, since these two sets clearly have equal cardinality. 