
---

mathLink: auto

---
Date created: 2024-03-20 17:28
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Monotone bounded sequences converge]], [[Supremum and infimum of sequences]]
References: _Not applicable_
Justifications: [[Supremum and infimum]], [[Infinite series]], [[Cardinality of a set]], [[Series on countable sets]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Convergence of countable series by suprema of the partial sums
> Let $X$ be an at most countable set, and let $f:X\to \mathbb{R}$ be a function. Then the series $\sum^{}_{x\in X}f(x)$ is absolutely convergent if and only if $$ \sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}  < \infty$$

The idea here is that we can't immediately appeal to partial sums as those inherently depend on what finite subset we choose to convert to a normal sum through a bijection. Thus we look at the suprema's of the partial sums considering the different choices of finite sets.

>[!quote]- Proof: Convergence of countable series by suprema of the partial sums
>We first prove it from left to right. The case where $X$ is finite is quiet trivial as it would imply there are only $2^{\left| X \right|}$ possible subsets to consider, all being finite. Thus it follows that $\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}$ is some finite subset of $\mathbb{R}$ with a finite supremum. Thus we may consider $X$ to be countable. This means we have a bijection $g:\mathbb{N}\to X$ and $g^{-1}:X\to \mathbb{N}$. Now to show that $\sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}$ is finite we will prove it is bounded. Notice that since $g^{-1}(A)$ is some finite subset of $\mathbb{N}$ with the same cardinality as $A$ it follows that there exists some $M$ such that $g^{-1}(A)\subseteq [\![0,M]\!]$ (Since finite subsets of $\mathbb{N}$ are bounded). Using the fact that the series is absolutely convergent we get that  $$\sum^{}_{x\in A}\left| f(x) \right| = \sum^{}_{n\in g^{-1}(A)}\left| f(g(n)) \right|  \leq \sum^{}_{n\in [\![0,M]\!] } \left| f(g(n)) \right| \leq \sum^{\infty}_{n=0}\left| f(g(n)) \right| =\sum^{}_{x\in X}\left| f(x) \right| $$ Since putting $\sum^{}_{x\in X}\left| f(x) \right|< \sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}$ leads to an obvious contradiction we must have $$  \sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}\leq \sum^{}_{x\in X}\left| f(x) \right|  $$ Implying it's finiteness. Now we prove it from right to left. Once again we assume $X$ is countable, using the same two bijections, we have that every partial sum $\sum^{M}_{n=0}\left| f(g(n)) \right|$ is equal to the sum over the set $g([\![1,M]\!])\subset X$. Thus we know that for all $M$ and for all $K\geq M$ $$ \sum^{M}_{n=0}\left| f(g(n)) \right| \leq \sum^{K}_{n=0}\left| f(g(n)) \right| \leq \sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}  $$ In other words the sequence of partial sums is increasing and bounded, thus the sum $\sum^{\infty}_{n=0}\left| f(g(n)) \right|$ is indeed absolutely convergent.
>
>**Q.E.D.**

Note that one could show pretty easily that if the sum is indeed absolutely convergent, then we have that $$ \sum^{}_{x\in X}\left| f(x) \right| =\sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}  $$
