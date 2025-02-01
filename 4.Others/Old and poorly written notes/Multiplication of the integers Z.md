

---

mathLink: auto

---
Date created: 2023-10-21 22:37
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



## *Multiplication in the [[Integers|integers]] $\mathbb{Z}$*

The exact multiplication process is given in the construction of the [[Integers]].

#### *Properties*

- Integers have no zero divisors, $ab=0\implies a=0 \lor b=0$
	$ab=0\implies (a'-a'')(b'-b'')=0-0\implies a'+b''+0=a''+b'+0\implies a'+b''=a''+b'$. This can only be true if either $a'=a''$ or $b'=b''$ or both. But whenever one is true, we have that it's respective value was $0$. $a'=a''\implies a=0$ and $b'=b''\implies b=0$.
	
	**Q.E.D.**
- Cancellation law
	Suppose: $a=(x-y), b=(z-f), c=(\alpha -\beta)$. Then we have that $(x-y)(\alpha-\beta)=(z-f)(\alpha-\beta)$ which is equivalent to $(x\alpha+y\beta)-(y\alpha+x\beta)=(z\alpha+f\beta)-(f\alpha+z\beta)$. According to equality of integers we have $x\alpha+y\beta+f\alpha+z\beta=z\alpha+f\beta+y\alpha+x\beta\implies \alpha(f+x)+\beta(y+z)=\alpha(z+y)+\beta(f+x)$. Now suppose $\alpha > \beta$ then $\alpha=\beta +h\land h\neq 0$. And thus $\beta(y+z)+\beta(f+x)+h(f+x)=\beta(x+y)+\beta(f+x)+h(z+y)\implies h(f+x)=h(z+y)\implies f+x=z+y$.
	
	**Q.E.D.**