
---

mathLink: auto

---
Date created: 2023-10-22 11:25
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


##### Cancellation of bijective inverses

Let $f : X → Y$ be a bijective function, and let $f^{−1} : Y → X$ be its inverse. Then we can conduct the following cancelations:
- $\forall x\in X :f^{-1}(f(x))=x$
	Suppose $y=f(x)$ then by the definition of inversion we have $f(f^{-1}(y))=f(x)$ which gives us $f(f^{-1}(f(x)))=f(x)$ and since $f$ is injective we get $f^{-1}(f(x))=x$.
- $\forall y\in Y: f(f^{-1}(y))=y$
	Suppose $f(x)=y$ , since $f$ is bijective we can denote $x$ as $f^{-1}(y)$ thus giving us $f(f^{-1}(y))=y$

We can also conclude from this that $f^{-1}$ is also invertible and that $(f^{-1})^{-1}=f$.
	If $g$ is the inverse of $f^{−1}$, then we have $f^{−1}(g(y))=y$, and applying $f$ to both sides yields $g(y)=f(y)$ and so $(f^{−1})^{−1}=f$.
Furthermore the inverse of a composition of bijections is the same as the composition of the inverses: $(g \circ f)^{−1} = f^{−1} \circ g^{−1}$
	This proof uses [[Inclusion and identity maps]].
	We defined inversion as such: $f^{-1}(y)=x$ which we know implies the cancelation laws, in order for this function to be the proper inverse it has to abide both those cancelation laws. We start first by showing that $f(f^{-1}(y))=y$, which in our case is $(g \circ f)\circ f^{−1} \circ g^{−1}$ which with associativity gives us $g\circ\imath_{Y\rightarrow Y}\circ g^{-1}$ which according to properties of identity maps we get $g\circ g^{-1}$ which then is equal to $\imath_{X\rightarrow X}$ which closes the first case. Now we shall also prove that $f^{-1}(f(x))=x$.  $(f^{−1} \circ g^{−1})\circ (g \circ f)$ which equals $f^{−1} \circ (g^{−1}\circ g) \circ f=f^{−1} \circ \imath_{X\rightarrow X} \circ f=f^{−1} \circ f=\imath_{Y\rightarrow Y}$ . This closes the proof.
	**Q.E.D.**
And we also notice that the inverse of a bijection is always bijective.  
	To show that $f^{-1}$ is bijective, note that if $f^{−1}(a)=f^{−1}(b)$, then applying $f$ to both sides yields $a=b$ by axiom of substitution, hence $f^{-1}$ is injective. Furthermore, $f^{-1}(f(x))=x$, hence $f^{-1}$ is surjective.
