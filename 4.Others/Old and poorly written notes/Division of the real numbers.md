
---

mathLink: auto

---
Date created: 2023-11-13 16:17
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



- If a sequence is Cauchy then $(a^{-1}_{n})$ is also Cauchy
	Since $a_n$ is Cauchy and bounded away from zero we have $|a_n-a_m|\leq\varepsilon$ and $|a_k|\geq c$ for all $k$. By definition we show that $|a^{-1}_n-a^{-1}_m|= |\frac{a_m-a_n}{a_ma_n}|\leq\frac{|a_m-a_n|}{c^2}$ and since $a_n$ is Cauchy we know it will eventually be $c^2\varepsilon$ close for some $m,n\geq N$ and thus $|a^{-1}_n-a^{-1}_m|= |\frac{a_m-a_n}{a_ma_n}|\leq\frac{|a_m-a_n|}{c^2}\leq\varepsilon$. Which proves $a^{-1}_n$ is Cauchy.
	
	**Q.E.D.**

Now we can effectively define reciprocation. Let $x$ be a non-zero real number. Let $(a_n)^\infty_{n=1}$ be a Cauchy sequence bounded away from zero such that $x=\text{LIM}_{n\rightarrow \infty}\;a_n$. Then we define it's reciprocal: $$x^{-1}:=\text{LIM}_{n\rightarrow \infty}\;a^{-1}_n$$All that is now left is to show that this definition is well defined and that it is consistent for all rationals. 
	Consider the following product $P:=\text{LIM}_{n\rightarrow \infty}\;a^{-1}_n\times\text{LIM}_{n\rightarrow \infty}\;a_n\times\text{LIM}_{n\rightarrow \infty}\;b^{-1}_n$ which is clearly equal to $\text{LIM}_{n\rightarrow \infty}\;b^{-1}_n$ and the same can be done the other way around.

This definition of reciprocation is obviously also consistent with the [[Rational numbers]].

Once this is done we can simply define division on the reals. $$\frac{x}{y}:=x\times y^{-1}$$ From which the classic cancellation laws follow. With all this out of the way we can end this section by stating that the real numbers form a [[Fields|field]].
