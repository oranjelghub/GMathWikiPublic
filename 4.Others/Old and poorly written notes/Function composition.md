
---

mathLink: auto

---
Date created: 2023-10-22 11:21
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



## *Function composition* 

Let $f:X\rightarrow Y$ and $g:Y \rightarrow Z$ be two functions such that the range of $f$ is de domain of $g$ . We then define their composition $g\circ f:X\rightarrow Z$ as such:$$(g\circ f)(x):=g(f(x))$$If range and domain don't match up then we leave the composition undefined. Composition also obeys the axiom of substitution.

Composition is an operation that is not commutative (easily proven by an arbitrary example) but is still associative.


##### Proof that function composition obey the axiom of substitution

To prove that the axiom of substitution holds we have to prove that if $f=f'$ and $g=g'$ then $g \circ f=g'\circ f'$. By definition of equality we first have $f(x)=f'(x)$ for all $x$ in the domain. By the substitution axiom of equality we have that $g(f(x))=g(f'(x))$ but since $g=g'$ it is going to map the elements of the domain of $g$ to the same elements in the range of $g$ so we can write $g(f(x))=g'(f'(x))$. But according to the definition of composition we get $g \circ f =g' \circ f'$.

**Q.E.D.**


##### Proof that function composition is associative

Suppose we have $f:Z \rightarrow W$ , $g:Y \rightarrow Z$ , $h: X\rightarrow Y$
Since $g \circ h$ is a function from $X$ to $Z$, $f \circ(g \circ h)$ is a function from $X$ to $W$. Similarly $f \circ g$ is a function from $Y$ to $W$, and hence $(f \circ g) \circ h$ is a function from X to $W$. Thus $f \circ (g \circ h)$ and $(f \circ g) \circ h$ have the same domain and range. In order to check that they are equal, we see from the definition of function equality that we have to verify that $(f \circ (g\circ h))(x) = ((f \circ g)\circ h)(x)$ for all $x ∈ X$. But by definition of composition $(f \circ (g \circ h))(x) = f((g \circ h)(x)) = f(g(h(x)) = (f \circ g)(h(x)) = ((f \circ g) \circ h)(x)$ as desired.

**Q.E.D.**




- Let $f : X → Y$ and $g : Y → Z$ be functions. If $f$ and $g$ are both injective, then so is $g \circ f$.
	Basic proof
- Let $f : X → Y$ and $g : Y → Z$ be functions. If $f$ and $g$ are both surjective, then so is $g \circ f$.
	Basic proof
-  Let $f : X → Y$ and $g : Y → Z$ be functions. If $g\circ f$ is injective then so is $f$ but also that $g$ may not be injective.
	If $g\circ f$ is injective then we know that $a\neq b \implies g\circ f (a) \neq g \circ f (b)$. Now suppose that $f$ actually isn't injective, then we know that for some $c \neq d$ we have $f(c)=f(d)$. But then according to the axiom of substitution we have $g\circ f (c)=g\circ f(d)$ but this implies $g\circ f$ isn't injective which is a contradiction. For the case of $g$ we now use the fact that $f$ is injective. Suppose $g$ isn't injective, then $a\neq b \implies f(a)\neq f(b) \implies g(f(a))=g(f(b))$ for some $a,b$. But this would be a contradiction since the composition is injective. Now one may say that $g$ must be injective, BUT THATS WRONG. In fact we didn't prove $g$ was injective, we proved that $g$ is injective over $f$'s range as domain for $g$. There could be $y\in Y$ that is not in $f$'s range but still causes $g$ to fail at injection. Thus $g$ doesn't have to be injective in general.
	
	**Q.E.D.**
- Let $f : X → Y$ and $g : Y → Z$ be functions. If $g\circ f$ is surjective then so is $g$ but also that $f$ may not be surjective.
	We know that $g\circ f$ is surjective thus $\forall z \in Z:\exists x\in X: g\circ f(x)=z$. So we have $z=g\circ f (x) = g(f(x))$. Now suppose $g$ isn't surjective, then for some $z'$ there is no $y$ such that $g(y)=z'$. But this would mean that it doesn't matter what elements $f$ maps in $Y$, as if in the full domain $g$ isn't surjective, this would mean that $g\circ f$ is also not surjective which is a contradiction. $f$ on the other hand doesn't have to be surjective, since every $z$ can have multiple predecessors in $Y$ , as long as $f$'s range contains at least 1 predecessor of every $z$ then the composition and $g$ will remain surjective.
	
	**Q.E.D.**