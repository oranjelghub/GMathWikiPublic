---
mathLink: auto
Date created: 2024-05-22 19:04
tags:
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---  

Proved by: [[Axiom of choice]]
References: _Not applicable_
Justifications: [[Sequential definition of continuity of real valued functions]], [[Continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Proof: Equivalence between the sequential and the classic definition of continuity of real valued functions
> Given $X\subseteq \mathbb{R}$ and a function $f:X\to \mathbb{R}$ with some $x_{0}\in X$. Suppose that $f$ is continuous in $x_0$ by the classic definition. Then notice that for every real $\varepsilon>0$ there exists some $\delta$ such that $$ \left| x-x_{0} \right|\leq \delta \implies \left| f(x)-f(x_{0}) \right| \leq \varepsilon  $$ But since I can get any sequence $(x_n)^\infty_{n=m}$ that converges to $x_{0}$ consisting of elements of $X$ $\delta$-close to $x_{0}$ we must have that $f(x)$ is $\varepsilon$-close to $f(x_{0})$ and thus that $(f(x_n))^\infty_{n=m}$ converges and specifically converges to $f(x_{0})$. Since the choice of sequence is arbitrary we are done. Now suppose the converse, that $f$ is continuous at $x_0$ by the sequential definition. We will proceed by contradiction, so suppose it doesn't converge by the classic definition. Then we can define $$ E_{N}:=\left\{ x\in X: \left| x-x_{0} \right| \frac{1}{N} \land \left| f(x)-f(x_{0}) \right|>\varepsilon_{\mu}   \right\}  $$ Using some $\varepsilon_{\mu}>0$ which we know exists according to our assumption. Notice that this set is non-empty for all $N$ and we can thus define a choice function $(c_n)^\infty_{n=1}$ on $\bigcup_{n=1}^\infty E_{n}$. We notice that $\lim_{ n \to \infty }c_{n}=x_{0}$ but that clearly $\lim_{ n \to \infty }f(c_{n})\neq f(x_{0})$, a contradiction to the continuity by the sequential definition. Thus our assumption that $f$ isn't continuous in $x_{0}$ by the classic definition must be wrong and we are done.
> 
> **Q.E.D.**



