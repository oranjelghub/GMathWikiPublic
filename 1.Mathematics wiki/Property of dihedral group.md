
---

mathLink: $\sigma^i\tau=\tau\sigma^{-i}$

---
Date created: 2023-11-23 21:26
Tags: #Type/Proof  #Topic/Abstract_Algebra 

Proved by: [[Functions]], [[Dihedral group]]
References: _Not applicable_
Justifications: [[Modular arithmetic]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

We want to prove the following property concerning reflections and rotations in the [[Dihedral group]].

> [!quote] Proof: $\sigma^i\tau=\tau\sigma^{-i}$
>We  have to prove that $\sigma\tau=\tau\sigma^{-1}$. We do this by analyzing where an arbitrary $1\leq k\leq n$ may get mapped to. In the case of $\tau$, we first notice that for every $k$ we have that $k=\gamma+k'$ (where $\gamma$ is the vertex of the reflection), which we can justify by the fact that there exists a rotation $\sigma_k$ such that $\sigma_k(\gamma)=k$. We thus have that $\tau(k)=\gamma-k'$ by definition of $\tau$. On the right hand side we have the inverse of a rotation. Suppose the original rotation is one by $\alpha$, then we have that $\sigma^{-i}(k)=k-i\alpha$. Combining these two results we get the intermediate result: $$\sigma(\gamma-k')=\tau(k-i\alpha)$$ Once again applying $\sigma$ on the left gives us $\gamma-k'+i\alpha$ and on the right hand side we notice that $k-i\alpha=\gamma+k'-i\alpha=\gamma+(k'-i\alpha)$ and under $\tau$ we have that $$\tau(\gamma+(k'-i\alpha))=\gamma-k'+i\alpha$$ This gives us $RHS=LHS$ and closes the proof.
>
>**Q.E.D.**

---

**_Remark_**: All the above arithmetic is [[Modular arithmetic|modular]].