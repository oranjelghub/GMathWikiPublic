
---

mathLink: auto

---
Date created: 2023-10-22 11:28
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



#### *Partial functions*

Let $X$, $Y$ be [[Sets|sets]]. We define a partial function from $X$ to $Y$ to be any function $f : X' \rightarrow Y'$ whose domain $X'$ is a subset of $X$, and whose range $Y'$ is a subset of $Y$ . We note here that the collections of partial functions from a function $f$ is indeed a [[Sets|set]] 


##### Proof

Suppose we have $X'\subseteq X$ and $Y'\subseteq Y$. According to the [[Power sets|power set]] axiom and the definition of [[Cartesian product|cartesian products]] we can construct the following well defined set $\mathcal{P}(X)\times\mathcal{P}(Y)=\{(X',Y'):X'\in\mathcal{P}(X)\land Y'\in\mathcal{P}(Y)\}$. Now using the axiom of replacement we can construct the following set: $\{Y'^{X'}:P(Y'^{X'},(X',Y'))\land (X',Y'))\in \mathcal{P}(X)\times\mathcal{P}(Y)\}$. This is the set of all power sets of partial functions. In order to construct a set with only all the partial functions we take the arbitrary [[Union, intersection and difference of sets|union]] which gives us a valid set, namely: $\bigcup\{Y'^{X'}:P(Y'^{X'},(X',Y'))\land (X',Y'))\in \mathcal{P}(X)\times\mathcal{P}(Y)\}$.

**Q.E.D.**