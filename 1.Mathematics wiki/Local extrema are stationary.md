---
mathLink: auto
Date created: 2024-07-09 00:18
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Equivalence between the sequential and the classic definition of the limit of a function at a point]]
References: _Not applicable_
Justifications: [[Differentiation of real valued functions]], [[Left and right limits of real valued functions]], [[Sequential definition of limit of a function at a point]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Local extrema are stationary
> Let $a<b$ be real numbers, and let $f:(a,b)\to \mathbb{R}$ be a function. If $x_{0}\in (a,b)$, $f$ is differentiable at $x_{0}$, and $f$ attains a local maximum or minimum, then $f'(x_{0})=0$.

>[!quote] Proof: Local extrema are stationary
>First we may assume WLOG that $f$ attains a local maximum in $x_{0}$. This means there is some $\delta>0$ such that $f|_{[x_{0}-\delta,x_{0}+\delta]}$ attains a maximum in $x_{0}$. Note that $f|_{[x_{0}-\delta,x_{0}+\delta]}$ is also differentiable at $x_{0}$ and that $f'(x_{0})=f'|_{[x_{0}-\delta,x_{0}+\delta]}(x_{0})$. This means that the limit $$ \lim_{ x \to x_0:x\in  [x_{0}-\delta,x_{0}+\delta]} \frac{f(x)-f(x_{0})}{x-x_{0}} $$exists and is equal to some $L\in \mathbb{R}$, specifically we know that the left and right limit agree and are both equal to $L$. By the sequential definition  this means that for all sequences $(a_n)^\infty_{n=0}$ consisting only of elements in $[x_{0}-\delta,x_{0}+ \delta]\cap(x_{0},+\infty)$ such that $a_{n}\to x_{0}$ when $n\to \infty$ we have that $$ \frac{f(a_{n})-f(x_{0})}{a_{n}-x_{0}}\to L \hspace{1cm} \text{when}\hspace{1cm} n\to \infty$$But notice that for all $n\in \mathbb{N}$ we have that $a_{n}-x_{0}\geq 0$ and since $f$ attains a local maximum in $x_{0}$ we also know that $f(a_{n})-f(x_{0})\leq 0$ implying that for all $n\in \mathbb{N}$ we have $$ \frac{f(a_{n})-f(x_{0})}{a_{n}-x_{0}}\leq 0 $$ Taking the limit on both sides obtains us the statement $L\leq 0$. The same argument can be applied, this time on the left limit, to show that $L\geq 0$, finally implying that we must have $L=0$.
>
>**Q.E.D.**
