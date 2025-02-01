---
mathLink: auto
Date created: 2024-07-03 17:34
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Newton's approximation]], [[Absolute value]]
References: _Not applicable_
Justifications: [[Differentiation of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Chain rule for differentiation of real valued functions
> Let $X$ and $Y$ be subsets of $\mathbb{R}$, let $x_{0}\in X$ be a limit point of $X$ and let $y_{0}\in Y$ be a limit point of $Y$. Let $f:X\to Y$ be a function such that $f(x_{0})=y_{0}$, and such that $f$ is differentiable at $x_{0}$. Suppose that $g:Y\to \mathbb{R}$ is a function which is differentiable at $y_{0}$. Then $g\circ f: X\to \mathbb{R}$ is differentiable at $x_{0}$ and $$ (g\circ f)'(x)=g'(y_{0})f'(x_{0}) $$

>[!quote]- Proof: Chain rule for differentiation of real valued functions
>We would now like to show that $g\circ f$ is differentiable at $x_{0}$ with derivative $g'(y_{0})f'(x_{0})$, which we do by showing newtons approximation holds. In other words $$\forall \varepsilon>0 \exists \delta>0: \forall x\in X\backslash \{ x_{0} \}, \left| x-x_{0} \right| \leq \delta \implies \left| g(f(x))-g(f(x_{0}))-L_{1}L_{2}(x-x_{0}) \right| \leq \varepsilon \left| x-x_{0} \right| $$
>To simplify the notation we define $L_{1}:=f'(x_{0})$ and $L_{2}:=g'(y_{0})$. Notice that by Newtons approximation we have that $$ \forall \varepsilon>0 \exists \delta>0: \forall y\in Y\backslash \{ y_{0} \} \left| y-y_{0} \right| \leq \delta\implies \left| g(y)-g(y_{0})-L_{2}(y-y_{0}) \right|\leq  \varepsilon \left| y-y_{0} \right|  $$ Since $y_{0}$ is still a limit point of $f(X)$ we know that we can restrict the map $g$ to $g|_{f(X)}$, which would still be differentiable at $y_{0}$ and preserve it's derivative. This means we may rewrite the statement as $$ \forall \varepsilon>0 \exists \delta>0: \forall x\in X\backslash \{ x_{0} \} \left| f(x)-f(x_{0})\right| \leq \delta\implies \left| g(f(x))-g(f(x_{0}))-L_{2}(f(x)-f(x_{0})) \right|\leq  \varepsilon  \left| f(x)-f(x_{0})\right|  $$ Now write this delta $\delta_{g}$, since $f$ is continuous at $x_{0}$ we know there is some $\delta _f$ such that $$ \left| x-x_{0} \right| \leq \delta_{f}\implies \left| f(x)-f(x_{0}) \right| \leq \delta_{g} $$ Thus our final statement look like this $$\forall \varepsilon>0 \exists \delta_{f}>0: \forall x\in X\backslash \{ x_{0} \} \left| x-x_{0} \right| \leq \delta_{f}\implies  \left| g(f(x))-g(f(x_{0}))-L_{2}(f(x)-f(x_{0})) \right|\leq  \varepsilon  \left| f(x)-f(x_{0})\right| $$Fix some arbitrary $\varepsilon$, but also fix the $\varepsilon^{*}$ such that $\varepsilon\geq \varepsilon^{*}\left( \varepsilon^{*}+\left| L_{1} \right|+\left| L_{2} \right| \right)$ and fix it's respective $\delta_{f}$, we now do some algebra on the right hand side. Using the triangle inequality we obtain $$ \left| g(f(x))-g(f(x_{0}))-L_{1}L_{2}(x-x_{0}) \right|-\left| L_{2}(f(x)-f(x_{0})) - L_{1}L_{2}(x-x_{0}) \right| \leq  \left| g(f(x))-g(f(x_{0}))-L_{2}(f(x)-f(x_{0})) \right|\leq  \varepsilon^{*}  \left| f(x)-f(x_{0})\right|    $$ Which means $$ \left| g(f(x))-g(f(x_{0}))-L_{1}L_{2}(x-x_{0}) \right| \leq \varepsilon^{*} \left| f(x)-f(x_{0}) \right| + \left| L_{2} \right| \left| f(x)-f(x_{0})-L_{1}(x-x_{0}) \right| $$ Assuming for the sake of non triviality that $L_{2}$ is non-zero, we know that there is some $\delta'$ such that $$ \left| x-x_{0} \right| \leq \delta' \implies \left| f(x)-f(x_{0})-L_{1}(x-x_{0}) \right|\leq \varepsilon^{*}\left| x-x_{0} \right|   $$Thus $$ \left| x-x_{0} \right| \leq \min\{ \delta_{f},\delta' \} \implies \left| g(f(x))-g(f(x_{0}))-L_{1}L_{2}(x-x_{0}) \right| \leq \varepsilon^{*} \left| f(x)-f(x_{0}) \right| + \left| L_{2} \right|\varepsilon^{*}\left| x-x_{0} \right|   $$We notice that by the triangle inequality and Newtons approximation we can show that for all $\varepsilon >0$ there exists some $\delta>0$ such that $$ \left| x-x_{0} \right| \leq \delta \implies \left| f(x)-f(x_{0}) \right| \leq \left| L_{1} \right| \left| x-x_{0} \right| \varepsilon$$ We use this fact using $\varepsilon^{*}$ and it's corresponding $\delta''$ to obtain $$  \left| x-x_{0} \right| \leq \min\{ \delta_{f},\delta',\delta'' \} \implies \left| g(f(x))-g(f(x_{0}))-L_{1}L_{2}(x-x_{0}) \right| \leq \varepsilon^{*} \left| L_{1} \right| \left| x-x_{0} \right| \varepsilon^{*} + \left| L_{2} \right|\varepsilon^{*}\left| x-x_{0} \right|    $$ Which by choice of $\varepsilon^{*}$ implies that $$  \left| x-x_{0} \right| \leq \min\{ \delta_{f},\delta',\delta'' \} \implies \left| g(f(x))-g(f(x_{0}))-L_{1}L_{2}(x-x_{0}) \right| \leq \varepsilon\left| x-x_{0} \right|    $$  This closes the proof. 
>
>**Q.E.D.**

