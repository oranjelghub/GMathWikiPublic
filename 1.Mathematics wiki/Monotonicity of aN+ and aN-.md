
---

mathLink: Monotonicity of $(a_{N}^+)_{N=m}^\infty$ and $(a_{N}^-)_{N=m}^\infty$

---
Date created: 2024-01-14 16:58
Tags: #Type/Notion #Topic/Real_Analysis 

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Limsup and liminf of sequences]], [[Sequences]]

---  


> [!quote] Notion: Monotonicity of $(a_{N}^+)_{N=m}^\infty$ and $(a_{N}^-)_{N=m}^\infty$
> $$\forall n:a_{n}^+\geq a_{n+1}^+ \land a_{n}^-\leq a^-_{n+1}$$

We can proof this the following way

>[!quote]-  Proof of Monotonicity of $(a_{N}^+)_{N=m}^\infty$ and $(a_{N}^-)_{N=m}^\infty$
> For any $K\geq m$ we have $a^+_K=\sup(a_n)^\infty_{n=K}$ and thus for all $n\geq K$ we have that $a_n\leq \sup(a_n)^\infty_{n=K}$. Now consider $a^+_{K+1}=\sup(a_n)^\infty_{n=K+1}$, here once again we have for all $n\geq K+1$ that $a_n\leq \sup(a_n)^\infty_{n=K+1}$. Suppose for the sake of contradiction that $a^+_K<a^+_{K+1}$ this would mean that for all $n\geq K$ we have $$a_n\leq \sup(a_n)^\infty_{n=K}\leq \sup(a_n)^\infty_{n=K+1}$$ But if this statement is true for all $n\geq K$ then it's also true for all $n\geq K+1$, but this means that $a^+_K$ bounds $(a_n)^\infty_{n=K}$ whilst being smaller than $a^+_{K+1}$, contradicting the fact that $a^+_{K+1}$ is the least upper bound of $(a_n)^\infty_{n=K+1}$. Thus we must have that $a_{K+1}^+\leq a_K^+$ thus proving that $(a^+_N)^\infty_{N=n}$ is monotonically increasing. The proof is symmetrical for $(a^-_N)^\infty_{N=n}$

We can easily use this to prove the following result as well:
$$a_{\alpha}^-\leq a_{\beta}^+$$

