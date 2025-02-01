---
mathLink: auto
Date created: 2024-07-03 12:50
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Heine-Borel theorem for the real line]], [[Existence of a unique increasing bijection from the natural numbers to one of its inifnite subsets]]
References: _Not applicable_
Justifications: [[Uniform continuity of real valued functions]], [[Continuity of real valued polynomials]], [[Sequential definition of uniform continuity of real valued functions]], [[Cauchy sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Continuous real valued functions on a closed interval are uniformly continuous on that interval
> Let $a<b$ be real numbers, and let $f:X\to \mathbb{R}$ be a function continuous on $[a,b]$. Then $f$ is uniformly continuous.

>[!quote] Proof: Continuous real valued functions on a closed interval are uniformly continuous on that interval
>Suppose for the sake of contradiction that $f$ isn't uniformly continuous. Then by the sequential definition there must exist two equivalent sequences $(x_n)^\infty_{n=0}$ and $(y_n)^\infty_{n=0}$ such that $(f(x_n))^\infty_{n=0}$ and $(f(y_{n}))^\infty_{n=0}$ aren't equivalent. This means there exists an $\varepsilon >0$ such that the set $$ E:= \{ n\in \mathbb{N}: \left| f(x_{n})-f(y_{n}) \right| >\varepsilon \} $$ Is non-empty. It is obvious that $E$ is infinite, more precisely $E$ is countable. Thus there exists some unique increasing bijection $g:\mathbb{N}\to E$ and we get that for all $n\in \mathbb{N}$, $\left| f(x_{g(n)})-f(y_{g(n)}) \right|>\varepsilon$. Since $(x_{g(n)})^\infty_{n=0}$ is a bounded sequence on a closed set we may apply Heine-Borel and find some convergent subsequence $(x_{g(\sigma(n))})^\infty_{n=0}$ with a limit $L\in [a,b]$. We use the same subsequence for the other sequence $(y_{g(\sigma(n))})^\infty_{n=0}$, and we get that $$ \begin{align} \lim_{ n \to \infty } x_{n}-y_{n} &= 0 \\ \lim_{ n \to \infty } x_{g(\sigma(n))}-y_{g(\sigma(n))} &= 0  \\ \lim_{ n \to \infty } y_{g(\sigma(n))}&=L \end{align} $$ Thus by continuity of $f$ we get $\lim_{ n \to \infty }f(x_{g(\sigma(n))})=\lim_{ n \to \infty }f(y_{g(\sigma(n))})=f(L)$, but this would imply that $$ \lim_{ n \to \infty } f(x_{g(\sigma(n))})- f(y_{g(\sigma(n))})=0 $$ A contradiction.
>
>**Q.E.D.**


