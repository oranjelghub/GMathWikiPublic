
---

mathLink: auto

---
Date created: 2024-02-17 11:10
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Convergence of sequences]], [[Completeness of the real numbers]]
References:  _Not applicable_
Justifications: [[Series on finite sets are well-defined]], [[Series over finite sets]]

Specializations: _Not applicable_
Generalizations: [[Interchanging limit and sum]]

---  

> [!quote] Theorem: Interchanging limit and sum (finite case)
> If the sequence of real numbers $(a_n(x))^\infty_{n=m}$ is convergent for all $x\in X$ where $X$ is some finite set then $$\lim_{ n \to \infty } \sum^{}_{x\in X}a_{n}(x)=\sum^{}_{x\in X}\lim_{ n \to \infty } a_{n}(x)$$

>[!quote] Proof: Interchanging limit and sum (finite case)
>Supposing that the sequence $\left( \sum^{}_{x\in X}a_n(x) \right)^\infty_{n=m}:=(\Omega_{n})^\infty_{n=m}$ converges proves the statement as we can then use induction to extend the rule for the limit of a sum to the limit of a $n$ sum. We thus prove the convergence of $\Omega_{n}$. Notice that we have for arbitrary $j$ and $k$ and a bijection $h:[\![1,\#X]\!]\to X$ $$ \left|  \Omega_{j}-\Omega_{k}\right| = \left|  \sum^{\#X}_{i=1}a_{j}(h(i))-a_{k}(h(i))\right| \leq \sum^{\#X}_{i=1}\left| a_{j}(h(i))-a_{k}(h(i)) \right|  $$ Since for all $n$ and $x$, $(a_n(x))^\infty_{n=m}$ is convergent, we fix some real $\varepsilon >0$ and have that $$ \forall h(i)\in X\; \exists \mu_{i}: \forall j,k \geq \mu_{i},\; \left| a_{j}(h(i))-a_{k}(h(i)) \right|\leq \frac{\varepsilon}{\#X}  $$ Now we define $$ \mathcal M :=\max\{ \mu_{i}: i\in [\![1,\#X]\!] \}$$ And thus have for all $i\in [\![1,\#X]\!]$ and $j,k\geq \mathcal M$,  $\left| a_{j}(h(i))-a_{k}(h(i)) \right|\leq \frac{\varepsilon}{\#X}$. Which by properties of sums gives us $$   \sum^{\#X}_{i=1}\left| a_{j}(h(i))-a_{k}(h(i)) \right|\leq \sum^{\#X}_{i=1} \frac{\varepsilon}{\#X}=\varepsilon$$ Thus to sum up $$\forall \varepsilon >0 \; \exists \mathcal M\geq m:\forall j,k\geq \mathcal M,\; \left| \Omega_{j}-\Omega_{k} \right| \leq \varepsilon $$ Thus the sequence is Cauchy, and since $\mathbb{R}$ is complete the sequence also converges in $\mathbb{R}$. Using now also the extended formula for the limit of a $n$ sum (provable through induction), we have $$  \lim_{ n \to \infty } \sum^{}_{x\in X}a_{n}(x)=\sum^{}_{x\in X}\lim_{ n \to \infty } a_{n}(x)$$
>
>**Q.E.D.**

