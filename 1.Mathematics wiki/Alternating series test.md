
---

mathLink: auto

---
Date created: 2024-02-11 17:02
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Completeness of the real numbers]]
References: _Not applicable_
Justifications: [[Infinite series]], [[Induction]], [[Completeness of the real numbers]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Alternating series test
> Let $(a_n)^\infty_{n=m}$ be a sequence of non-negative real numbers which is decreasing ($a_{n+1}\leq a_{n}$). Then the series $\sum^{\infty}_{n=m}(-1)^{n}a_{n}$ is convergent if and only if $\lim_{ n \to \infty }a_{n}=0$.

>[!quote] Proof: Alternating series test
>First suppose $\sum^{\infty}_{n=m}(-1)^{n}a_{n}$ converges, then we automatically know that $\lim_{ n \to \infty }(-1)^{n}a_{n}=0$ but notice that this on it's own also implies that $a_{n}$ converges to $0$, thus the first implication is done. Now we do the other implication, suppose that $\lim_{ n \to \infty }a_{n}=0$, we want to show that $\sum^{\infty}_{n=m}(-1)^{n}a_{n}$ converges. First notice that $$ S_{N+2}=S_{N}+(-1)^{N+1}a_{N+1}+(-1)^{N+2}a_{N+2}=S_{N}+(-1)^{N+1}(a_{N+1}-a_{N+2}) $$ And since the sequence $a_n$ is decreasing an always positive this implies that $S_{N}\leq S_{N+2}$ when $N$ is odd and $S_{N}\geq S_{N+2}$ when $N$ is even. With a simple induction this extends to $S_{N}\geq S_{N+2k}$ for all natural numbers $N\geq m$ and all natural numbers $k$. Now suppose $N$ is even. Notice that $$ S_{N+2k+1}\geq S_{N+1}=S_{N}-a_{N+1} $$ and $$ S_{N+2k+1}=S_{N+2k}-a_{N+2k+1}\leq S_{N+2k} $$ Combining all of this gives us $$ S_{N}-a_{N+1}\leq S_{N+2k+1}\leq S_{N+2k}\leq S_{N} $$ for all $k$. In particular this allows us to say that $$ \forall n\geq N,\; S_{N}-a_{N+1}\leq S_{n}\leq S_{N}\leq S_{N}+a_{N+1} $$ Implying that $$ \forall n\geq N,\; \left| S_{n}-S_{N} \right| \leq a_{N+1}  $$ But since we can get $a_n$ epsilon small because it converges to $0$ this says us that $S_{n}$ is Cauchy, meaning it converges and also meaning that $\sum^{\infty}_{n=m}(-1)^{n}a_{n}$ converges
>
>**Q.E.D.**



