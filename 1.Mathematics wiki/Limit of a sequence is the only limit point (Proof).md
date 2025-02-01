
---

mathLink: auto

---
Date created: 2023-12-18 12:59
Tags: #Type/Proof  #Topic/Real_Analysis 

Proved by: [[Cauchy sequences]], [[Convergence of sequences]], [[Limit points of a sequence]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

We prove that a sequence that converges to $c$ has $c$ as as only limit point. 

> [!quote] Proof: Limit of a sequence is the only limit point
> Since $\lim_{ n \to \infty }a_{n}=c$ we have: $$ \forall \varepsilon >0 \exists N : \forall n\geq N, d(a_{n},c) \leq \varepsilon$$ Which clearly implies that $c$ is a limit point. Now suppose we had a second limit point $c'$. Then we have that for all $N$ there exists a $n$ such that: $$ d(a_{n},c')\leq \frac{\varepsilon}{2}$$ Now also take the necessary $N'$ such that the sequence is $\frac{\varepsilon}{2}$ close to to $c$. We can then combine the statements to say: $$ \forall n\geq \max(N,N'), d(a_{n},c)+d(c',a_{n})\leq \varepsilon$$ Which with the triangle inequality gives us:$$ d(c,c')\leq \varepsilon $$ Which implies $c=c'$.
> 
> **Q.E.D.**

