---
mathLink: auto
Date created: 2024-09-17 17:48
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Newton's approximation]], [[Laws of Riemann integration]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Lipschitz continuity of real valued functions]], [[Differentiation of real valued functions]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: First fundamental theorem of calculus
> Let $a<b$ be real numbers and $f:[a,b]\to \mathbb{R}$ a Riemann integrable function. Let $F:[a,b]\to \mathbb{R}$ be the function $$ F(x):=\int_{[a,x]}f  $$Then $F$ is Lipschitz continuous, and furthermore, if for some $x_{0}\in [a,b]$, $f$ is continuous at $x_{0}$, then $F$ is differentiable at $x_{0}$ with $F'(x_{0})=f(x_{0})$

>[!quote] Proof: First fundamental theorem of calculus
>Let $x<y$ be elements of $[a,b]$, then $$ F(y)-F(x)=\int_{[a,y]} f-\int_{[a,x]} f=\int_{[x,y]} f $$And since $f$ is bounded for by some real number $M$ (since $f$ is Riemann integrable) $$ \int_{[x,y]} f\leq \int_{[x,y]} M=M(y-x) $$Similarly, it follows that $$ -M(y-x)\leq \int_{[x, y]} f  $$And thus $$ \left| F(y)-F(x) \right|\leq M(y-x)  $$More generally, regardless of ordering of $x$ and $y$, we have $$ \left| F(x)-F(y) \right|\leq M\left| x-y \right|   $$Meaning that $F$ is Lipschitz continuous. Now suppose $x_{0}\in [a,b]$ and $f$ is continuous at $x_{0}$, then for all $\varepsilon>0$ there exists some $\delta>0$ such that $$ \forall x\in[x_{0}-\delta,x_{0}+\delta]\cap[a,b],\; f(x_{0})-\varepsilon\leq f(x)\leq f(x_{0})+\varepsilon \hspace{2cm} \text{(1)}$$We now show that $F$ is differentiable at $x_{0}$ and has derivative $f(x_{0})$ by using Newtons approximation, so we show that $$ \left| F(y)-F(x_{0})-f(x_{0})(y-x_{0}) \right|\leq \varepsilon \left| y-x_{0} \right|   $$To do this we fix some arbitrary $y\in [x_{0}-\delta,x_{0}+\delta]\cap[a,b]$ and split into three cases depending on the ordering of $y$ with respect to $x_{0}$. We only show the case $y>x_{0}$, since $y=x_{0}$ is trivial and $y<x_{0}$ is symmetric. So notice that $$ F(y)-F(x_{0})=\int_{[x_{0},y]} f $$And since $y,x_{0}\in [x_{0}-\delta,x_{0}+\delta]\cap[a,b]$ we can integrate the three terms of the inequality of $\text{(1)}$ over $[y,x_{0}]$ and obtain $$ (f(x_{0})-\varepsilon)(y-x_{0})\leq \int_{[x_{0},y]} f\leq (f(x_{0})+\varepsilon)(y-x_{0}) $$And so in particular $$ \left| F(y)-F(x_{0})-f(x_{0})(y-x_{0}) \right|\leq \varepsilon \left| y-x_{0} \right|  $$This closes the proof.
>
>**Q.E.D.**

