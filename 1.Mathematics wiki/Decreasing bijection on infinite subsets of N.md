
---

mathLink: Decreasing bijection on infinite subsets of $\mathbb{N}$

---
Date created: 2024-03-13 16:36
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis #Topic/Set_Theory 

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Cardinality of a set]], [[Natural numbers]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Decreasing bijection on infinite subsets of $\mathbb{N}$
> Let $X$ be a infinite subset of $\mathbb{N}$, then there exists some unique bijections $f:\mathbb{N}\to X$ such that $f(n)<f(n+1)$. Thus $X$ is countable.

>[!quote] Proof: Decreasing bijection on infinite subsets of $\mathbb{N}$
>Define the sequence $(a_n)^\infty_{n=0}$ by $$ \begin{align} a_{n}&:=\min\{ x\in X: \forall m<n, x\neq a_{m}  \}\\ a_{0} &:= \min(X) \end{align} $$ Since $X$ is infinite we also have that $\{ x\in X: \forall m<n, x\neq a_{m}  \}$ is infinite, because if that wasn't the case then $\{ x\in X: \forall m<n, x\neq a_{m}  \}$ would be bounded by some $M\in \mathbb{N}$ implying that $X\subseteq [\![0,M]\!]_{\mathbb{N}}$ and on it's turn implying the finiteness of $X$, a contradiction. Thus $\{ x\in X: \forall m<n, x\neq a_{m}  \}$ is also always non-empty and thus our sequence is well defined. It is pretty obvious that $(a_n)^\infty_{n=0}$ is strictly increasing as stating the inverse quickly leads to contradiction. In particular $(a_n)^\infty_{n=0}$ forms a injective function. Now we want to show that it is also surjective by a contradiction. Let $x\in X$, suppose that for all natural numbers $n$ we have $a_{n}\neq x$. Thus this implies $$ \forall n\in \mathbb{N}; x\in \{ x\in X: \forall m<n, x\neq a_{m}  \} $$ Which by definition of $a_n$ also means that for all $n$, $a_{n}\leq x$ and since $(a_n)^\infty_{n=0}$ is a increasing function of natural numbers we have $$ \forall n\in \mathbb{N};  n\leq a_{n}\leq x$$ But then this also holds for $x+1$, meaning that $x+1\leq x$, a contradiction. Thus the sequence must be surjective and consequently bijective. We only miss uniqueness of $(a_n)^\infty_{n=0}$ to finish up the proof. Suppose the was some other increasing bijection $(b_n)^\infty_{n=0}$ from $\mathbb{N}$to $X$. Then the set $\{ n\in \mathbb{N}:b_{n}\neq a_{n} \}$ is non empty and define $m:=\min\{ n\in \mathbb{N}:b_{n}\neq a_{n}  \}$. Thus in particular $b_{m}\neq a_{m}$ and for all $n<m$, $a_{n}=b_{n}$. But we also must have (otherwise we get a direct contradiction) $$ g(m)=\min\{ x\in X:\forall t<m ;x\neq a_{t} \}=a_{m} $$ A contradiction, thus $(a_n)^\infty_{n=0}$ is unique as well.
>
>**Q.E.D.**

