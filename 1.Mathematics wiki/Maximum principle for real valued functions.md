---
mathLink: auto
Date created: 2024-05-27 18:14
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Heine-Borel theorem for the real line]], [[Squeeze test of sequences]], [[Boundedness of continuous real valued functions on a,b]]
References: _Not applicable_
Justifications: [[Axiom of choice]], [[Closed subsets]], [[Bounded sets in R]], [[Limit of a sequence]], [[Continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Maximum principle for real valued functions
> Let $a<b$ be real numbers and let $f:[a,b]\to \mathbb{R}$ be continuous on $[a,b]$. Then $f$ attains a maximum for some $x_{max}\in [a,b]$ and a minimum for some $x_{min}\in [a,b]$.

>[!quote] Proof: Maximum principle for real valued functions
>We shall just show that $f$ attains its maximum somewhere; the proof that it attains its minimum also is similar. We know that since $f$ is continuous on a bounded and closed interval that it is bounded. In other words  $m_{+}:=\sup f([a,b])$ is finite. It follows that for all $x$ in $X$ that $f(x)\leq m_{+}$. We define $$ E_{N}:=\{ x\in X: m_{+}- \frac{1}{N}<f(x)\leq m_{+} \}  $$ By the axiom of choice we may define some choice function $(c_n)^\infty_{n=1}$ on $\bigcup_{i=1}^{\infty}E_{i}$. Since $c_{n}$ is a sequence in a closed and bounded set, according to the Heine-Borel theorem, it must have some convergent subsequence $(c_{\sigma(j)})^\infty_{j=1}$ whos limit is contained in the original set. We denote $\lim_{ j \to \infty }c_{\sigma(j)}:=x_{max}\in [a,b]$. Combining this with the fact that $$ m_{+}-\frac{1}{j}\leq m_{+}-\frac{1}{\sigma(j)}<f(c_{\sigma(j)}) $$ We obtain $$ m_{+}-\frac{1}{\sigma(j)}\leq f(c_{\sigma(j)})\leq m_{+} $$ And since $f$ is continuous on $[a,b]$ we we can take the limit to infinity on all sides with respect to $j$ and we obtain $$ m_{+}\leq f(x_{max})\leq m_{+} $$ Thus there exists a $x_{max}\in [a,b]$ such that $f$ attains a maximum in $x_{max}$. This closes the proof.
>
>**Q.E.D.**

A better proof exists using compactness.