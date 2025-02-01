
---

mathLink: auto

---
Date created: 2023-11-15 12:15
Tags: #Type/Notion #Type/Unfinished 

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

---  



> [!quote] Notion:
> Lorem ipsum dolor sit amet





- Interspersing
	- Interspersing of integers by rationals. For all rational numbers $x$ there exists a unique number $n$ such that $n\leq x\leq n+1$.
		Since $x$ is rational we have that $a/b$ for some integers $a$ and $b$, suppose $a$ is positive (if it isn't the case then one can just change the fraction to $-a/(-b)$). Then we can rewrite $a$ in terms of $b$ according to the Euclidian algorithm. $x=\frac{a}{b}=\frac{mb+r}{b}=m+\frac{r}{b}$ and since $r<b\implies \frac{r}{b}<1$ we have that $m\leq m+\frac{r}{b} <m+1\implies m\leq x <m+1$. We now have to prove the uniqueness of our answer. Suppose that there were two integers $n$ and $n'$ such that $n\leq x<n+1$ and $n'\leq x<n'+1$. Now also suppose for the sake of contradiction we have that $n\neq n'$, then according to trichotomy we have that $n'<n$ or $n'>n$. The proof is synonymous for both cases so let's arbitrarily suppose that $n'<n$. Then we have by transitivity and by the fact that addition preserves order that $n'<n\leq x<n'+1<n+1$. But if $n'<x$ then $n'+1\leq x$ but we just said that $x<n'+1$ and thus we have a contradiction.
		
		**Q.E.D.**
	- Interspersing of rationals by rationals. If $x$ and $y$ are two rationals such that $x<y$, then there exists a third rational $z$ such that $x<z<y$.
		Let $z:=\frac{x+y}{2}$ then we have that $\frac{x}{2}<\frac{y}{2}\implies \frac{x}{2}+\frac{y}{2}<y\implies \frac{x+y}{2}<y$. The exact same can be done on the other side to show that $x<\frac{x+y}{2}$. And thus we know that there exists a $z$.
		
		**Q.E.D.** 





