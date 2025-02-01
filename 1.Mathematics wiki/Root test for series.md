
---

mathLink: auto

---
Date created: 2024-03-11 17:50
Tags: #Type/Theorem #Type/Proof  #Topic/Real_Analysis 

Proved by: [[Geometric series]], [[Zero test for series]]
References: _Not applicable_
Justifications: [[Infinite series]]

Specializations: _Not applicable_
Generalizations: [[Ratio test for series]]

---  

> [!quote] Theorem: Root test
> Let $\sum^{\infty}_{n=m}a_{n}$ be a series of real numbers and define $\alpha:=\limsup_{ n \to \infty }|a_{n}|^{1/n}$.
> 1. If $\alpha<1$, then the series $\sum^{\infty}_{n=m}a_{n}$ is absolutely convergent.
> 2. If $\alpha>1$, then the series $\sum^{\infty}_{n=m}a_{n}$ is divergent.
> 3. If $\alpha=1$, we cannot assert any conclusion.

>[!quote] Proof: Root test
>First suppose $\alpha<1$ then we know there exists some $\varepsilon$ such that $\alpha+\varepsilon<1$. Using the properties of limit superiors we know that there exists some $N\geq m$ such that for all $n\geq N$ $$ |a_{n}|^{1/n} \leq \alpha+\varepsilon<1$$ Implying $$ \forall n\geq N;|a_{n}|\leq (\alpha+\varepsilon)^n $$ Since $\alpha+\varepsilon<1$ we know this geometric series converges and we have that $$ \forall M\geq N;\sum^{M}_{n=N}|a_{n}|\leq \sum^{\infty}_{n=N}(\alpha+\varepsilon)^{n}$$ Thus the partial sums of $|a_{n}|$ are increasing and bounded and thus absolutely converge.
>Now suppose $\alpha>1$. Once again according to properties of superior limits we know that for every $N\geq m$ there is some $\mu\geq N$ such that $$ |a_{\mu}|\geq 1^n $$ But this means that the sequence does not converge to zero as putting $\varepsilon=0,9$ guarantees that does not exist any $N$ to satisfy the conditions of convergence. Since the sequence doesn't converge to $0$, we know the series diverges. The final part can be done by finding two examples of series that both have $\alpha=1$ but where one of them absolutely converges and the other one diverges.
>
>**Q.E.D.**


