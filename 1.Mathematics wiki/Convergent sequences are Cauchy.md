
---

mathLink: auto

---
Date created: 2023-11-27 13:53
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Metric spaces]], [[Convergence of sequences]], [[Limit of a sequence]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  


> [!quote] Theorem: Convergent sequences are Cauchy
> Given the $\lim_{n\rightarrow\infty}a_n=L$, $(a_n)^\infty_{n=m}$ is Cauchy

The proof goes as follows:

>[!quote] Proof: Convergent sequences are Cauchy
>We want to show that: $$\forall\varepsilon, \varepsilon>0,\exists N:\forall n\geq N\;\text{we have}\;d(a_n,a_m)\leq\varepsilon$$ By the triangle inequality we have: $$d(a_n,a_m)\leq d(a_n,L)+d(L,a_m)$$ Thus it suffices for the right hand side to be less or equal to epsilon in order to have the desired statement. Since we have convergence: $$d(a_n,a_m)\leq d(a_n,L)+d(L,a_m)\leq \frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon$$ And we thus have the desired statement.
>
>**Q.E.D.**


