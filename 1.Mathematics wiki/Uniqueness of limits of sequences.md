
---

mathLink: auto

---
Date created: 2023-11-27 12:18
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Metric spaces]], [[Convergence of sequences]], [[Limit of a sequence]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  


> [!quote] Theorem: Limits of sequences are unique
> Given a [[Convergence of sequences|convergent sequence]] $(a_n)^\infty_{n=m}$ in the [[Metric spaces|metric space]] $(X,d)$, the sequence $a_n$ has exactly $1$ limit.

The proof goes as follows:

>[!quote] Proof: limits of sequences are unique
>Suppose that $a_n$ had a limit $L$ and $L'$. We then have: $$\begin{align}
>\forall \varepsilon\in \mathbb R, \varepsilon>0, \exists N\in\mathbb N:\forall n\geq N \;\text{we have}\;d(a_n,L)\leq\frac{\varepsilon}{2}\\
>\forall \varepsilon\in \mathbb R, \varepsilon>0, \exists N'\in\mathbb N':\forall n\geq N \;\text{we have}\;d(a_n,L')\leq\frac{\varepsilon}{2}
>\end{align}$$
>By triangle inequality:
>$$\forall n\geq\text{max}(N,N'):d(L,L')\leq d(L,a_n)+d(a_n,L')\leq \varepsilon$$
>To argue that $L=L'$ we notice that if it wasn't the case then $d(L,L')=c$ for some $c\in\mathbb R$, but this implies that $L$ and $L'$ will never be $\frac{c}{2}$-close, a contradiction. Thus $L=L'$.
>
>**Q.E.D.**


