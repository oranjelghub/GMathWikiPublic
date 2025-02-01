
---

mathLink: auto

---
Date created: 2024-01-31 12:12
Tags: #Type/Theorem #Type/Proof #Topic/Real_Analysis 

Proved by: [[Comparison principle of sequences]], [[Limsup and liminf of sequences (Properties)]]
References: _Not applicable_
Justifications: [[Sequences]], [[Ordering of the real numbers]]

Specializations: _Not applicable_
Generalizations: [[Comparison principle of sequences]]

---  

> [!quote] Theorem: Squeeze test of sequences
>  Let $(a_n)^\infty_{n=m}$, $(b_n)^\infty_{n=m}$ and $(c_n)^\infty_{n=m}$ be sequences of real numbers such that $$a_n\leq b_n \leq c_n$$ for all $n\geq m$. Suppose also that $(a_n)^\infty_{n=m}$ and $(c_n)^\infty_{n=m}$ both converge to the same limit $L$. Then $(b_n)^\infty_{n=m}$ converges to $L$

>[!quote] Proof: Squeeze test of sequences
> Since a sequence converging to $L$ implies that $L^-=L=L^+$ we have that by the comparison principle $$\begin{align} L\leq \limsup_{n\to \infty}b_n\leq L\\ L\leq \liminf_{n\to \infty}b_n\leq L\\ \end{align}$$ But since the $L^+$ and $L^-$ of $(b_n)^\infty_{n=m}$ are equal this implies that $(b_n)^\infty_{n=m}$ itself converges to $L$.

