
---

mathLink: auto

---
Date created: 2023-11-15 15:53
Tags: #Type/Theorem  #Topic/Real_Analysis 

Proved by:[[Cauchy sequences]], [[Positive and negative real numbers]]
References:  _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

The theorem states the following:

> [!quote] Theorem:
> Let $(a_n)^\infty_{n=1}$ be a [[Sequences|sequence]] of non-negative rationals. Then $\text{LIM}_{n\rightarrow\infty}\;a_n$ is a non-negative [[Real numbers|real]]

And the proof goes as follows:

>[!quote] Proof: Closure of the non-negative reals
>Suppose for the sake of contradiction that $x:=\text{LIM}_{n\rightarrow\infty}\;a_n$ with $x$ being negative and all $a_n$ positive. Then by definition of negativity we have $x=\text{LIM}_{n\rightarrow\infty}\;b_n$ for some Cauchy sequence that is bounded away from zero negatively, i.e. $b_i\leq -c<0$. Now since $a_n$ and $b_n$ are equivalent we must have that $|a_n-b_n|\leq \frac{c}{2}$ for some $N$ and all $n\geq N$. We thus have $|a_n-b_n|\leq \frac{c}{2}\implies a_n-b_n\leq \frac{c}{2}\implies a_n\leq \frac{c}{2}+b_n\leq -c +\frac{c}{2}=\frac{-c}{2}$ but this is a contradiction as $a_n>0$ for all $n$.
>
>**Q.E.D.**








