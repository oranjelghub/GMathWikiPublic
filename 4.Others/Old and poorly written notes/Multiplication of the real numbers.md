
---

mathLink: auto

---
Date created: 2023-11-13 16:13
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


In the same fashion we can define multiplication of reals. Let $x=\text{LIM}_{n\rightarrow \infty}\;a_n$ and $y=\text{LIM}_{n\rightarrow \infty}\;b_n$:$$xy:=\text{LIM}_{n\rightarrow \infty}\;a_nb_n$$ And once again we have to check that this definition is well defined and that the operation is closed.
	To check that the operation is closed we have to prove that $xy$ is real. We do this by noticing that $|a_jb_j - a_kb_k| = |a_jb_j - a_jb_k + a_jb_k - a_kb_k| \leq |a_j||b_j-b_k| + |b_k||a_j - a_k|\leq\varepsilon$. Now since both sequences are bound we know that for some $M$ we have $|a_j||b_j-b_k| + |b_k||a_j - a_{k}|\leq M_1|b_j-b_k| + M_2|a_j - a_k|\leq\varepsilon$. And since once again the sequences are Cauchy we can impose that the terms inside the absolute value are less or equal to $\frac{\varepsilon}{2M}$, for some $j,k\geq max(N_1,N_2)$. And thus $M_1|b_j-b_k| + M_2|a_j - a_{k}|\leq M_{1}\frac{\varepsilon}{2M_1} + M_{2}\frac{\varepsilon}{2M_2}\leq\varepsilon$. And thus we have that $a_nb_n$ is Cauchy meaning that $xy$ is real. To then show substitution we need to show that $xy=xy\land x=x'$ and this can be done by showing that the sequences $a_nb_n$ and $a'_{n}b_n$ are equivalent. $|a_nb_n-a'_nb_n|\leq\varepsilon$ which simplifies to $|a_nb_n-a'_nb_{n}|= |b_n||a_n-a'_{n}| \leq\varepsilon$ and knowing that $b_n$ is bounded by $M_b$ and that for some $n\geq N$ $a_n$ and $a'_n$ are $\frac{\varepsilon}{M_b}$-close we have $|b_n||a_n-a'_{n}| \leq M_b\frac{\varepsilon}{M_b} \leq\varepsilon$ for all $n\geq N$. And thus we know that the sequences are equivalent.  
