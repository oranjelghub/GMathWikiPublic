---
mathLink: auto
Date created: 2024-08-01 18:06
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Laws of Riemann integration]], [[Monotone bounded functions on bounded intervals are Riemann integrable]]
References: _Not applicable_
Justifications: [[Infinite series]], [[Riemann integral]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Integral test for series
> Let $f:\mathbb{R}^{+}\to \mathbb{R}$ be a monotone decreasing and non-negative function. Then $\sum^{\infty}_{n=0}f(n)$ is convergent if and only if $$ \sup_{N>0}\int_{[0,N]} f<\infty $$

>[!quote] Proof: Integral test for series
>Since $f$ is monotone decreasing, for all $x\in [n,n+1)$ $$ f(n)\geq f(x)\geq f(n+1) $$Defining $g: \mathbb{R}^{+}\to \mathbb{R}$ and $h:\mathbb{R}^{+}\to \mathbb{R}$ by $$ g(x):= n \text{ when } x\in [n,n+1)\land h(x):=n+1 \text{ when } x\in [n,n+1) $$And since $f$ is bounded, it is integrable on $[n,n+1)$ and we get $$ f(n)=\int_{[n,n+1)}g\geq \int_{[n,n+1)}f\geq \int_{[n,n+1)}h=f(n+1)    $$When taking the sum over $0\leq n\leq N-1$ $$ \sum^{N-1}_{n=0}f(n)\geq \int_{[0,N]} f \geq \sum^{N-1}_{n=0}f(n+1)=\sum^{N}_{n=1}f(n)$$Now notice that if $\sum^{\infty}_{n=0}f(n)$ is convergent then it converges to $\sup \left( \sum^{K}_{k=0}f(k) \right)^{\infty}_{K=1}$ and we must have that $\sup_{N>0}\int_{[0,N]}f$ is finite. Conversely, if $\sup_{N>0}\int_{[0,N]}f$ is finite then clearly the partial sums are bounded and, since they are increasing, the series converges.
>
>**Q.E.D.**


