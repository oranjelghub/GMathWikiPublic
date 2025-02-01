
---

mathLink: auto

---
Date created: 2023-11-27 15:20
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Convergent sequences are Cauchy]], [[Cauchy sequences]]
References: _Not applicable_
Justifications: [[Subsequences]], [[Real numbers]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  


> [!quote] Theorem: Real convergent sequences are bounded
> Given a convergent sequences of [[Real numbers]] $(a_n)^\infty_{n=m}$ we have that: $$\exists M \in\mathbb N:\forall n\geq m \;\text{we have}\;|a_n|\leq M$$

The proof goes as follows:

>[!quote] Proof: Real convergent sequences are bounded
>Given a convergent sequence $(a_n)^\infty_{n=m}$ we know $a_n$ is Cauchy. Without loss of generality choose an arbitrary real $\varepsilon >0$. We know there exists a $N\in \mathbb N$ for which: $$\forall n,m\geq N:|a_n-a_m|\leq \varepsilon$$. Now consider the finite subsequence $(a_n)^N_{n=m}$. One can easily show by induction a finite sequence of real numbers is bounded. Thus: $$\exists M:\forall n, 1\leq n< N\;\text{we have}\;|a_n|\leq M$$ The other  subsequence $(a_n)^\infty_{n=N}$ is also bounded, suppose we fix $m:=N$, then: $$|a_n|\leq\varepsilon +a_N$$ Thus the sequence in general is bounded by $\text{max}(M,\varepsilon+a_N)$ and since the choice of epsilon is arbitrary we prove that a bound always exists.
>
>**Q.E.D.**

