
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



#### *Empty set function*

We also note a special case of a function, namely the empty function, which is defined as follows: $$f_\emptyset:\emptyset\rightarrow X$$There is not need to specify a property as the function doesn't actually map any elements into $X$. We also note that for every set $X$ the corresponding empty function is unique.

We notice that the empty function is always injective since it's satisfies the property of injective functions in a vacuous manner. If the set $X$ is also equal to $\emptyset$ then, once again by vacuous truth, we have that the function is bijective.


##### Proof of the uniqueness of an empty function

Suppose that for an arbitrary set $X$ there were more than one distinct empty set functions. We know that according to function equality 2 functions are equal if all the elements of the domains get mapped to the same elements in the range. But since both functions map no elements at all since their domain is the empty set we can conclude that they thus both map the domains elements to the same elements in the range. Meaning that effectively the two functions are equal and that the empty set function associated to a set $X$ is unique.

**Q.E.D.**