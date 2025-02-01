
---

mathLink: auto

---
Date created: 2023-11-13 12:41
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




- If $(a_n)^\infty_{n=1}$ and $(b_n)^\infty_{n=1}$ are equivalent sequences, then one of them is Cauchy if and only if the other one is Cauchy.
	We want to to prove that $|b_k-b_j|\leq\varepsilon$ for any epsilon greater than zero. We first write $|b_k-b_j|=|b_k-a_k+a_k-a_j+a_j-b_j|$ which according to the triangle inequality gives us $|b_k-a_k+a_k-a_j+a_j-b_{j}|\leq |b_k-a_{k}| +|a_k-a_{j}|+ |a_j-b_{j}|\leq 3\varepsilon$. To make this cleaner and finalize the proof we notice that $|a_k-a_{j}|\leq \frac{\varepsilon}{3}$ for some $j,k\geq N_1$ and $|a_n-b_{n}|\leq \frac{\varepsilon}{3}$ for some $n\geq N_2$. Thus for all $j,k,n\geq max(N_1,N_2)$ the two conditions are true. And thus $|b_k-b_{j}|\leq \varepsilon$ where $k,j\geq max(N_1,N_2)$.
	