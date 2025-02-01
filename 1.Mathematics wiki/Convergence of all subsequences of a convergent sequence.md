
---

mathLink: auto

---
Date created: 2024-01-31 13:06
Tags: #Type/Theorem  #Type/Proof  #Topic/Real_Analysis 

Proved by:  _Not applicable_
References:  _Not applicable_
Justifications: [[Limit of a sequence]], [[Subsequences]]

Specializations:  _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Convergence of all subsequences of a convergent sequence
> Let $(a_n)^\infty_{n=m}$ be a sequence of real numbers converging to some limit $L$, then we have $$\lim_{ n \to \infty } a_{n}=L \iff  \forall f \; \text{that induce a subsequence}\;, \lim_{ n \to \infty }a_{f(n)}=L $$

>[!quote] Proof: Convergence of all subsequences of a convergent sequence
>We split the proof into the two implication. $(\Longrightarrow)$ By definition we have that $$\forall \varepsilon_{>0}\; \exists N: \forall n\geq N, |a_{n}-L |\leq \varepsilon$$ Since $\forall n\in \mathbb N, n\leq f(n)$ (because otherwise we can extract a contradiction using backwards induction to show that $f(0)<0$) $$\forall \varepsilon_{>0}\; \exists N: \forall n\geq N, |a_{f(n)}-L |\leq \varepsilon$$ Thus every subsequences converges as well. $(\Longleftarrow)$, if every subsequence converges then the one induced by $f(n)=n$ also converges meaning that by definition the sequence $(a_n)^\infty_{n=m}$ converges.
>
>**Q.E.D.**

