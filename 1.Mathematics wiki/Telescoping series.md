
---

mathLink: auto

---
Date created: 2024-02-14 16:33
Tags: #Type/Theorem #Type/Proof #Topic/Real_Analysis 

Proved by: [[Induction]]
References: _Not applicable_
Justifications: [[Infinite series]], [[Convergence of sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Telescoping series
> Given a sequence of real numbers $(a_n)^\infty_{n=0}$ converging to $0$ we have that $$ \sum^{\infty}_{n=m}(a_{n}-a_{n+1})=a_{0} $$ Alternatively if the series does not converge to zero but still converges to some real number $L$ then we have that $$ \sum^{\infty}_{n=m}(a_{n}-a_{n+1})=a_{0}-L $$
> 

>[!quote] Proof: Telescoping series
>First we can trivially show by induction that every partial sum $S_{N}$ is equal to $a_{0}-a_{N+1}$. We now claim that $$ \forall \varepsilon >0 \; \exists M\geq 0: \forall N\geq M,\; \left| a_{0}-L -S_{N}\right|  \leq \varepsilon$$ By the equivalence for the partial sums we just gave we see it is sufficient for $a_{N+1}$ to be epsilon close to $L$ for all $N\geq M$ which we know is possible thanks to the fact that $(a_n)^\infty_{n=0}$ converges to $L$
>
>**Q.E.D.**



