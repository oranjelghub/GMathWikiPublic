---
mathLink: auto
Date created: 2024-09-11 19:34
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Archimedean property]], [[Uniformly continuous real valued functions preserve boundedness of sets]], [[Upper and lower Riemann-Stieltjes integral]]
References: _Not applicable_
Justifications: [[Uniform continuity of real valued functions]], [[Riemann-Stieltjes integral]] 

Specializations: [[Uniformly continuous functions on bounded intervals are Riemann integrable]]
Generalizations: _Not applicable_

---

> [!quote] Theorem: Uniformly continuous functions on bounded intervals are Riemann-Stieltjes integrable
> Let $X$ be a closed interval and let $\alpha:X\to \mathbb{R}$ be a $\alpha$-length on $X$, if $f:I\to \mathbb{R}$ is uniformly continuous on some bounded interval $I\subseteq X$, then $f$ is Riemann-Stieltjes integrable on $I$ with respect to $\alpha$.

>[!quote] Proof: Uniformly continuous functions on bounded intervals are Riemann-Stieltjes integrable
>Note first that since $f$ is uniformly continuous on $I$ it is also bounded on $I$. Now fix some arbitrary real $\varepsilon>0$, it follows that there is some $\delta$ such that $$ \left| x-y \right| \leq \delta \implies \left| f(x)-f(y) \right| \leq \varepsilon $$Now let $I$ have endpoints $a$ and $b$, by the Archimedean property there exists some $N$ such that $\frac{b-a}{N}<\delta$. We can thus partition $I$ in $N$ intervals, which we don't explicitly construct ,which all have length $\delta$. Denote this partitions $\{ J_{i} \}_{1\leq i\leq N}$. Now define $$ \begin{align} G^{+}:I\to \mathbb{R}: x\mapsto \sup_{x\in J_{k}}f(x) \hspace{1cm} \text{if} \;x\in J_{k}\\ G^{-}:I\to \mathbb{R}: x\mapsto \inf_{x\in J_{k}}f(x) \hspace{1cm} \text{if} \;x\in J_{k}\end{align} $$These functions are clearly well defined and piecewise constant on $I$, as such it follows that $$0\leq \overline {\int}_{I} f\;d\alpha-\underline {\int}_{I} f\;d\alpha\leq \text{p.c.} \int_{I} G^{+}-G^{-}\;d\alpha $$By definition it follows $$0\leq \overline {\int}_{I} f\;d\alpha-\underline {\int}_{I} f\;d\alpha\leq \sum^{N}_{i=1}(\sup_{x\in J_{i}}f(x)-\inf_{x\in J_{i}}f(x))\alpha[J_{i}]$$Which by uniform continuity of $f$ on $I$ gives us $$0\leq \overline {\int}_{I} f\;d\alpha-\underline {\int}_{I} f\;d\alpha\leq \sum^{N}_{i=1}(\sup_{x\in J_{i}}f(x)-\inf_{x\in J_{i}}f(x))\alpha[J_{i}]\leq \varepsilon \sum^{N}_{i=1}\alpha[J_{i}]\leq \varepsilon \alpha[I]$$And since $\varepsilon$ is arbitrary, it follows that $f$ is Riemann-Stieltjes integrable on $I$.
>
>**Q.E.D.**




