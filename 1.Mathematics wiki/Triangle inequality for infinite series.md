
---

mathLink: auto

---
Date created: 2024-02-10 17:13
Tags: #Type/Theorem #Type/Proof #Topic/Real_Analysis 

Proved by: [[Comparison principle of sequences]]
References: _Not applicable_
Justifications: [[Infinite series]], [[Finite series (Properties)]], [[Absolute and conditional convergence of series]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Triangle inequality for infinite series
> If $\sum^{\infty}_{n=m}a_{n}$ is a absolutely convergent series of real numbers then we have $$ \left| \sum^{\infty}_{n=m}a_{n} \right| \leq \sum^{\infty}_{n=m}\left| a_{n} \right| $$

>[!quote] Proof: Triangle inequality for infinite series
>Since we know that absolute convergence implies conditional convergence we have that the sequence $\alpha_{N}:=\left| \sum^{N}_{n=m}a_{n} \right|$ and $\beta_{N}:=\sum^{N}_{n=m}\left| a_{n} \right|$ both converge. Using the fact that $\alpha_{N} \leq  \beta_{N}$ we have that $$\alpha_{N} \leq  \beta_{N} \implies \lim_{ N \to \infty }\alpha_{N} \leq \lim_{ N \to \infty } \beta_{N} \implies \left| \sum^{\infty}_{n=m}a_{n} \right| \leq \sum^{\infty}_{n=m}\left| a_{n} \right| $$
>
>**Q.E.D.**


