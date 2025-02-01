
---

mathLink: auto

---
Date created: 2023-11-21 11:48
Tags: #Type/Notion #Topic/Topology #Type/Proof 

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: [[Adherent points]]
Justifications: [[Convergence of sequences]], [[Open balls]]

---  

As an equivalent to definition of [[Adherent points|adherence]], we define a notion of sequential adherence.

> [!quote] Notion: Sequential adherence
> Given a [[Metric spaces|metric space]] $(X,d)$ and $Y\subseteq X$, $x\in X$ is said to be [[Adherent points|adherent]] to $Y$ if and only if there exists a [[Convergence of sequences|convergent]] [[Sequences|sequence]]  $(a_n)^\infty_{n=m}$ where $a_i\in X$ and where $(a_n)^\infty_{n=m}$ converges to $x$.

This statements requires a proof.

>[!quote] Proof: Equivalence of the standard definition of adherence and sequential adherence.
>Given $(X,d)$ and $Y\subseteq X$. Suppose we have $\lim_{n\rightarrow \infty}a_n=x$, then $\forall r\exists N\forall (n\geq N):a_n\in B_r(x)\implies B_r(x)\cap Y\neq \emptyset$, implying $x$ is adherent to $Y$. Now suppose that $x$ is adherent to $Y$, then we know that for every $n\geq 1$, there exists some point $x_n\in B_{\frac{1}{n}}(x)$ where $x_n\in Y$. We invoke some choice function $c:\mathbb{N}\to \bigcup_{n\in \mathbb{N}} B_{\frac{1}{n}}(x)$  and notice that $\lim_{ n \to \infty }x_{n}=x$.
>
>**Q.E.D.**

It follows from this that closed subsets always contain their own limit given a convergent sequence of it's own elements. Conversely it also holds that if every convergent sequence made out of elements of $X$ has a limit in $X$ that $X$ is closed.
