
---

mathLink: auto

---
Date created: 2023-11-13 16:11
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

We can now develop a notion of [[Addition]]. Let $x=\text{LIM}_{n\rightarrow \infty}\;a_n$ and $y=\text{LIM}_{n\rightarrow \infty}\;b_n$ then we define their sum as follows: $$x+y:=\text{LIM}_{n\rightarrow \infty}\;(a_n+b_{n})$$In order for this definition to be valid we have to show that it obeys the axiom of substitution and that our operation is closed (it is not a requirement so to speak but this is how we want it to behave).
	Closure can easily be shown by first applying the definition of Cauchy for the sum of two Cauchy sequences. $|a_k+b_k-a_j-b_j|\leq \varepsilon\implies |a_k-a_j|+|b_k-b_j|\leq\varepsilon$ and since the sequences are Cauchy we have that for some $k,j\geq{max}(N_1,N_2)$ both sums will be $\frac{\varepsilon}{2}$-close. And thus $|a_k+b_k-a_j-b_{j}|\leq\frac{\varepsilon}{2}+\frac{\varepsilon}{2}\leq \varepsilon$. Which proves closure. For substitution we would have to show that $x+y=x'+y\land x=x'$ and this can easily be done using the property of epsilon closeness that states that: Let $ε, δ > 0$. If $x$ and $y$ are $ε$-close, and $z$ and $w$ are $δ$-close, then $x + z$ and $y + w$ are $(ε + δ)$-close. Just replace $x$ and $y$ by $x$ and $x'$ whilst we replace $z$ and $w$ by two times $y$ which proves that $x+y$ and $x'+y$ are both $(\varepsilon +0)$-close proving the equality.

From this we can also quickly notice that $x+y=y+x$ since $a_n+b_n=b_n+a_n$.




