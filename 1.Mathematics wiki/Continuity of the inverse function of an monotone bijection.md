---
mathLink: auto
Date created: 2024-06-12 19:45
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Intermediate value theorem]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Monotone real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Continuity of the inverse function of an monotone bijection
> Let $a<b$ and $f:[a,b]\to \mathbb{R}$ be a function which is continuous and strictly monotone increasing on $[a,b]$. Then $f$ is a bijection to $[f(a),f(b)]$ and the inverse map $f^{-1}:[f(a),f(b)]\to [a,b]$ is also continuous and strictly monotone increasing.

>[!quote] Proof: Continuity of the inverse function of an monotone bijection
>We first prove that $f$ is bijective. Injectivity follows directly from the strict monotonicity of $f$, whilst the surjectivity is guaranteed by the intermediate value theorem. Thus $f$ is a bijection to $[f(a),f(b)]$. Then we can easily see that $f^{-1}$ must be strictly monotone increasing as well, since suppose this wasn't the case. Then for some $c,d\in [f(a),f(b)]$ which satisfy $c<d$ we must have $f^{-1}(d)<f^{-1}(c)$, but then by strict monotonicity of $f$ we must have $d<c$, a contradiction. Thus $f^{-1}$ is strictly monotone increasing as well. To show the continuity of $f^{-1}$ on $[f(a),f(b)]$ we fix some $y\in [f(a),f(b)]$, which by bijectivity of $f$ has some predecessor $x\in [a,b]$. Now fixing some arbitrary $\varepsilon>0$. Notice that there obviously exists a $\delta>0$ such that we have $[y-\delta,y+\delta]\subseteq [f(x-\varepsilon),f(x+\varepsilon)]$. Now notice that for every $f(k)$ that satisfies $\left| y-f(k) \right|\leq \delta$ we have that $f(x-\varepsilon)\leq f(k)\leq f(x+\varepsilon)$ which by strict monotonicity of $f^{-1}$ implies that $\left| k-x \right|\leq \varepsilon$, meaning that $f^{-1}$ is continuous at $y$. Since the choice of $y$ is arbitrary, we know that $f^{-1}$ is continuous on $[f(a),f(b)]$, this closes the proof. 
>
> **Q.E.D.**



