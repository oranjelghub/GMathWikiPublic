
---

mathLink: auto

---
Date created: 2024-01-31 12:18
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Comparison principle of sequences]], [[Convergent sequences are Cauchy]]
References: _Not applicable_
Justifications: [[Real numbers]], [[Cauchy sequences]]

Specializations: _Not applicable_
Generalizations: [[Completeness of metric spaces]]

---  

> [!quote] Theorem: Completeness of the real numbers
> Every Cauchy sequence $(a_{n})^{\infty}_{n=m}$ in $\mathbb R$ converges in $\mathbb R$ with a limit $L\in \mathbb R$

>[!quote] Proof: Completeness of the real numbers
>Since the sequence is Cauchy we have that it is by bounded, by the comparison principle this also shows us that $L^+$ and $L^-$ are finite. To show that the sequences converges it thus suffices to show that $L^-=L^+$. Let $\varepsilon_{>0}\in\mathbb R$, since the sequence is Cauchy we have that $$\forall \varepsilon \; \exists N\geq m:\forall n, a_{N}-\varepsilon\leq a_{n}\leq a_{N}+\varepsilon $$ By the basic properties of infs and sups we have $$ a_{N}-\varepsilon\leq \inf(a_{n})^\infty_{n=N}\leq \sup(a_{n})^\infty_{n=N}\leq a_{N}+\varepsilon $$ And by the comparison principle
>$$a_{N}-\varepsilon\leq L^-\leq L^+ \leq a_{N}+\varepsilon $$ Hence $$|L^+-L^- |\leq 2\varepsilon$$ And since the choice of epsilon is arbitrary we have that $L^+=L^-$, otherwise one could easily extract a contradiction. 
>
>**Q.E.D.**

