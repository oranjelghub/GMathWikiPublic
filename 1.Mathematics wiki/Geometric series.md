
---

mathLink: auto

---
Date created: 2024-02-24 11:27
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Induction]], [[Zero test for series]]
References: _Not applicable_
Justifications: [[Infinite series]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Convergence of geometric series
> Let $x$ be a real number. If $\left| x \right|\geq 1$ then the series $\sum^{\infty}_{n=0}x^{n}$ is divergent, otherwise if $\left| x \right|<1$ then the series $\sum^{\infty}_{n=0}x^{n}$ converges, more precisely $$ \sum^{\infty}_{n=0}x^{n}=\frac{1}{1-x} $$

>[!quote] Proof: Convergence of geometric series
>First by the zero test we know that if $\left| x \right|\geq 1$ then the series converges because so does the associated sequence. Now to prove the convergence consider the partial sums $$ S_{N}=\sum^{N}_{n=0} x^n$$ We we will show through induction that this is equal to $$ S_{N}= \frac{{1-x^{N+1}}}{1-x} $$ The base case is trivial, assuming it is true for $K$ we want to show it implies that it holds for $K+1$. Notice that $$ S_{K}= \frac{{1-x^{K+1}}}{1-x}\implies S_{K}+x^{K+1} =\frac{{1-x^{K+1}}}{1-x} +x^{K+1}=\frac{{1-x^{K+2}}}{1-x}$$ This proves our formula. Thus $$ \lim_{ N \to \infty } S_{N}=\lim_{ N \to \infty } \frac{{1-x^{N+1}}}{1-x} $$ And since each term of this algebraic expression is convergent ($\lim_{ n \to \infty }x^n=0$ since $\left| x \right|<1$) we can use limit laws to obtain $$ \sum^{\infty}_{n=0}x^{n}=\frac{1}{1-x} $$
>
>**Q.E.D.**



