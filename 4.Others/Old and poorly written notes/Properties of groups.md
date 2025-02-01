
---

mathLink: auto

---
Date created: 2023-10-24 22:39
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



## *Properties of groups*

- In a group $G$ the identity element is unique.
- The inverse element is unique
- For all the elements in the group we have $(a^{-1})^{-1}=a$
- The inverse of two elements under the operation $f((a,b))^{-1}=f((b^{-1},a^{-1}))$
- In a group $G$, the right and left cancellation laws hold. 
- For any $a_1,a_2,\ldots,a_n$ the value $a_1\circ a_2\circ\ldots\circ a_n$ is uniquely defined regardless of bracketing, this is also called the general associative law.
	This can be proven by strong induction on $n$. First we know and see that for $n=1,2,3$ the product is unambiguously defined. Now suppose that the product is unambiguously defined for $a_1\circ a_2\circ\ldots\circ a_n$ then we need to show that for $n+1$ the product is also unambiguously defined. We have $a_1\circ a_2\circ\ldots\circ a_n\circ a_{n+1}=\alpha\circ a_n\circ a_{n+1}$ which is a true statement according to the base cases and our induction hypothesis. This product is thus unambiguously defined for all $n$.