
---

mathLink: auto

---
Date created: 2024-02-19 18:50
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Triangle inequality for infinite series]]
References: _Not applicable_
Justifications: [[Infinite series]], [[Least upper bounds]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Comparison test for series
> Let $\sum^{\infty}_{n=m}a_{n}$ and $\sum^{\infty}_{n=m}b_{n}$ be two series of real numbers and suppose that $\left| a_{n} \right|\leq b_{n}$ for all $n\geq m$. Then if $\sum^{\infty}_{n=m}b_{n}$ is convergent then $\sum^{\infty}_{n=m}a_{n}$ is absolutely convergent and we also have $$ \left| \sum^{\infty}_{n=m}a_{n} \right| \leq \sum^{\infty}_{n=m}\left| a_{n} \right| \leq \sum^{\infty}_{n=m}b_{n} $$

>[!quote] Proof: Comparison test for series
>Using the fact that ${^{|a|}}S_{N}:=\sum^{N}_{n=m}|a_{n}|$ is monotonously increasing it suffices to show that it is bounded. Since $\sum^{\infty}_{n=m}b_{n}$ is convergent we have that $$ \forall N:{^{|a|}}S_{N}\leq  \sum^{N}_{n=m}b_{n}\leq \sup\left( \sum^{N}_{n=m} b_{n}\right)^\infty_{n=m}$$ Thus we have that ${^{|a|}}S_{N}$ converges and by using the triangle inequality for infinite sums which are absolutely convergent we have $$ \left| \sum^{\infty}_{n=m}a_{n} \right| \leq \sum^{\infty}_{n=m}\left| a_{n} \right| \leq \sum^{\infty}_{n=m}b_{n}  $$ 
>
>**Q.E.D.**


