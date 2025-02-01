
---

mathLink: auto

---
Date created: 2024-01-31 12:07
Tags: #Type/Theorem  #Type/Proof  #Topic/Real_Analysis  

Proved by: [[Limsup and liminf of sequences]]
References: _Not applicable_
Justifications: [[Sequences]], [[Ordering of the real numbers]]

Specializations: [[Squeeze test of sequences]]
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Comparison principle of sequences
>   Given two sequences $(a_n)^\infty_{n=m}$ and $(b_n)^\infty_{n=m}$ for which for all $n\geq m$, $a_n\leq b_n$, the following holds $$ \begin{align} sup(a_n)^\infty_{n=m}&\leq \sup(b_n)^\infty_{n=m}\\ \inf(a_n)^\infty_{n=m}&\leq \inf(a_n)^\infty_{n=m}\\ \limsup_{n\to\infty}(a_n)^\infty_{n=m}&\leq \limsup_{n\to\infty}(b_n)^\infty_{n=m}\\ \liminf_{n\to\infty}(a_n)^\infty_{n=m}&\leq \liminf_{n\to\infty}(b_n)^\infty_{n=m}\\ \end{align}$$

>[!quote] Proof: Comparison principle of sequences
> Notice that $$a_n\leq b_n\leq \sup(b_n)^\infty_{n=m}\implies \sup(a_n)^\infty_{n=m}\leq \sup(b_n)^\infty_{n=m}$$ because otherwise we would have a contradiction against the definition of the supremum of $a_n$. Similarly we have $$\limsup_{n\to\infty}a_n\leq\sup(a_n)^\infty_{n=m}\leq\sup(b_n)^\infty_{n=m}\implies \limsup_{n\to\infty}a_n\leq \limsup_{n\to\infty}b_n$$ to once again avoid a contradiction. The proofs is symmetric for the limit inferior and infimum. The rest is similar. 
> 
> **Q.E.D.**


