
---

mathLink: auto

---
Date created: 2023-11-29 17:49
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Least upper bounds]], [[Supremum and infimum of sets of extended reals]]
References: _Not applicable_
Justifications: [[Sequences]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Monotone bounded sequences converge
> Given $(a_n)^\infty_{n=m}$ with $a_n\leq a_{n+1}$ and a bound $M$, $a_n$ converges to $\sup(a_n)^\infty_{n=m}$

The proof goes as follows:

>[!quote] Proof: Monotone bounded sequences converge
>Since $(a_n)^\infty_{n=m}$ is bounded $\sup(a_n)^\infty_{n=m}$ exists in $\mathbb{R}$ because $\mathbb{R}$ has the LUB property. Now fix some arbitrary positive real number $\varepsilon$. Using the properties of suprema's of sequences we know that $$ \exists K\geq m:\sup(a_n)^\infty_{n=m} -\varepsilon< a_{K}<\sup(a_n)^\infty_{n=m}+\varepsilon  $$ Further more, the monotonicity of $(a_n)^\infty_{n=m}$ implies that $$\exists K\geq m: \forall k\geq K,\;\sup(a_n)^\infty_{n=m} -\varepsilon< a_{k}<\sup(a_n)^\infty_{n=m}+\varepsilon $$ Which after some algebraic manipulations gives us $$\forall \varepsilon >0\; \exists K\geq m:\forall k\geq K,\; \left| a_{k}-\sup(a_n)^\infty_{n=m} \right|\leq \varepsilon $$ Meaning $(a_n)^\infty_{n=m}$ does converge and converges to $\sup(a_n)^\infty_{n=m}$.
>
>**Q.E.D.**

