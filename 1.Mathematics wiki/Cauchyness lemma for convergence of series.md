
---

mathLink: auto

---
Date created: 2024-02-10 16:16
Tags: #Type/Theorem  #Type/Proof  #Topic/Real_Analysis 

Proved by: [[Completeness of the real numbers]]
References: _Not applicable_
Justifications: [[Infinite series]], [[Cauchy sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Cauchyness lemma for convergence of series
> Let $\sum^{\infty}_{n=m} a_{n}$ be a formal infinite series. $\sum^{\infty}_{n=m}a_{n}$ converges if and only if for every real $\varepsilon>0$ there exists $N\geq m$ such that for all other natural numbers $p,q\geq N$ $$ \left| \sum^{q}_{n=p}a_{n} \right| \leq \varepsilon $$

>[!quote] Proof: Cauchyness lemma for convergence of series
>If the series converges then the associated sequence of partial sums must be Cauchy thus $$ \forall \varepsilon>0, \exists N\geq m: \forall p,q\geq N+1,\; \left| S_{q}-S_{p-1} \right| \leq \varepsilon$$ (We chose $p,q\geq N+1$ so that the statement is true for $p=N+1$) We can assume without loss of generality that $q\geq p$ and thus we have $$\left| S_{q}-S_{p-1} \right| \leq \varepsilon \implies \left| \sum^{q}_{n=p}a_{n} \right| \leq \varepsilon$$ To prove the inverse implication just reverse the arguments to show the partial sum sequence is Cauchy, combining it with the completeness of the reals to prove that it converges.
>
>**Q.E.D.**


