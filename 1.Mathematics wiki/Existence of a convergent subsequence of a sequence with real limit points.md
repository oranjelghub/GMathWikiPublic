
---

mathLink: auto

---
Date created: 2024-01-31 13:38
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Limit points of a sequence]]
References: _Not applicable_
Justifications: [[Subsequences]], [[Sets]]

Specializations: [[Bolzano-Weierstrass theorem]]
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Existence of a convergent subsequence of a sequence with real limit points
> Let $(a_n)^\infty_{n=0}$ be a sequence of real numbers and $L\in \mathbb R$.
> $$L \; \text{is a limit point of}\; (a_n)^\infty_{n=0} \iff \exists f \;\text{subsequence inducing}\;:\lim_{ n \to \infty } a_{f(n)}=L$$

>[!quote] Proof: Existence of a convergent subsequence of a sequence with real limit points
>We split the proposition into the two implications. $(\Longleftarrow)$ Since we know that the subsequence converges to $L$ we have that for every $\varepsilon_{>0}$ and for all $N\geq m$ we have some $k$ such that $| a_{k}-L|\leq \varepsilon$ because we can put $k:=f(c), c\geq \max(N,K)$ and where $K$ is the natural number such that all the entries of the subsequence are epsilon close to $L$. $(\Longrightarrow)$ Consider the following construction $n_{j}:=\min\left\{  n>n_{j-1}:| a_{n}-L|\leq \frac{1}{j}  \right\}$ with $n_{0}:=\min\{ 0 \}$. One could trivially show by induction that this set is non empty for every $j$ thanks to the fact that $L$ is a limit point. Using now the fact that for every $\varepsilon$ exists a $j$ such that $\frac{1}{j}<\varepsilon$ we can confidently construct the subsequence $$b_{j}:=a_{n_{j}}$$ We now argue that this subsequence converges to $L$. So fix some arbitrary epsilon, which also induces some $j$ such that $\frac{1}{j}<\varepsilon$. This guarantees that $|b_{j}-L |\leq \frac{1}{j}<\varepsilon$, but also taking some $k\geq j$ we have that $\frac{1}{k}\leq \frac{1}{j}$ meaning that $$\forall k\geq j, |b_{k}-L |\leq \frac{1}{j}<\varepsilon$$ Thus proving by definition that $b_{j}$ converges to $L$.
>
>**Q.E.D.**


