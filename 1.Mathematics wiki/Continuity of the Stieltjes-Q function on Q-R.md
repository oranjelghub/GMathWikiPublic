---
mathLink: Continuity of the Stieltjes-$\mathbb{Q}$ function on $\mathbb{R} \backslash \mathbb{Q}$
Date created: 2024-09-22 16:55
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Geometric series]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Stieltjes-Q function]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Continuity of the Stieltjes-$\mathbb{Q}$ function on $\mathbb{R} \backslash \mathbb{Q}$
> Let $\Xi_{\mathbb{Q}}$ be the Stieltjes-$\mathbb{Q}$ function with respect to some arbitrary bijective sequence $(q_n)^\infty_{n=0}$ which maps $\mathbb{N}\to \mathbb{Q}$. Then $\Xi_{\mathbb{Q}}$ is continuous on $\mathbb{R}\backslash \mathbb{Q}$.

>[!quote]- Proof: Continuity of the Stieltjes-$\mathbb{Q}$ function on $\mathbb{R} \backslash \mathbb{Q}$
>We first consider the sequence of functions $(\Xi_{n})^{\infty}_{n=0}$ defined by $$ \Xi_{n}:\mathbb{R}\to \mathbb{R}: x\mapsto\sum_{r\in \mathbb Q: r<x, g(r)\geq 2^{-n}}g(r)  $$We now claim that this function is continuous on $\mathbb{R}\backslash \mathbb{Q}$. To show this notice that there are at most $n$ rationals $p$ that satisfy $$y<p<z \land g(p)\geq 2^{-n}$$Given some arbitrary real numbers $y,z$. Taking some real $x'<x$ yields us $$|\Xi_n(x)-\Xi_n(x')|=\left| \sum_{r\in \mathbb Q: x'\leq r<x, g(r)\geq 2^{-n}}g(r) \right| $$Given our previous discussion, if we fix $z:=x$ and take $y$ close enough to $x$, then the sum $\sum_{r\in \mathbb Q: y\leq r<x, g(r)\geq 2^{-n}}g(r)$ will become an empty sum. In other words there exists a $\delta >0$ such that for all $\varepsilon>0$ $$|x-x'|\leq \delta \implies |\Xi_n(x)-\Xi_n(x')|\leq \varepsilon$$ (If $x'>x$ we can just revert the roles of the previous argument) But this is equivalent to stating that $\Xi_n$ is continuous at $x$, thus $\Xi_n$ is indeed continuous at every irrational $x$. We now proceed to show that $\Xi_{\mathbb{Q}}$ is continuous on $\mathbb{R}\backslash \mathbb{Q}$. So let $x\in \mathbb{R} \backslash \mathbb{Q}$, we notice that for any $n\in \mathbb{N}$ $$|\Xi_{\mathbb{Q}}(x)-\Xi_n(x)|=\sum_{r\in \mathbb Q: r<x, g(r)< 2^{-n}}g(r)$$And since $\sum_{r\in \mathbb Q: r<x, g(r)< 2^{-n}}g(r)\leq\sum^\infty_{k=n+1}2^{-k}=2^{-n}$ It follows that $$|\Xi_{\mathbb{Q}}(x)-\Xi_n(x)|\leq 2^{-n}$$Now by our corollary we know that for all $\varepsilon>0$ there exists some $\delta>0$ such that $|x-x'|\leq \delta \implies | \Xi_n(x)-\Xi_n(x')|\leq \frac{\varepsilon}{3}$ but we also know there exists a $N$ such that $2^{-N}\leq \frac{\varepsilon}{3}$ since $\lim_{n\to \infty}2^{-n}=0$. Combining this information we see that $$\begin{align*} |\Xi_{\mathbb Q}(x')-\Xi_{\mathbb Q}(x)|&\leq |\Xi_{\mathbb Q}(x)- \Xi_N(x)|+|\Xi_N(x)-\Xi_{\mathbb Q}(x')|\\&\leq |\Xi_{\mathbb Q}(x)-\Xi_N(x)|+ |\Xi_N(x)-\Xi_N(x')|+|\Xi_{\mathbb Q}(x')-\Xi_N(x')|\\&\leq 2^{-N} +\frac{\varepsilon}{3} + 2^{-N} \leq \varepsilon  \end{align*}$$In other words, $f$ is continuous at $x$ for every irrational $x$.
>
>**Q.E.D.**

