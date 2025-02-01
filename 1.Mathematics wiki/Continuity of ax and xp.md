---
mathLink: Continuity of $a^x$ and $x^p$
Date created: 2024-05-22 10:32
tags:
  - Type/Theorem
  - Type/Proof
cssclasses:
---

---

Proved by: [[Equivalence between the sequential and the classic definition of continuity of real valued functions]], [[Real exponentiation]], [[Continuous version of squeeze test]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Sequential definition of continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Continuity of $a^x$ and $x^p$
> Suppose $a\in \mathbb{R}^{+}$ and $p\in \mathbb{R}$, then the functions $f(x):= a^{x}$ and $g(x):=x^{p}$ are both continuous on $\mathbb{R}$.

>[!quote]- Proof: Continuity of $f:\mathbb{R}\to \mathbb{R}: x\mapsto a^x$
>We will prove this making use of the sequential definition of continuity. Let $(y_{n})^\infty_{n=0}$ be some sequence converging to some $x_{0}$, then we have $$\forall K\; \exists N\geq 0: \forall n\geq N, \left| y_{n}-x_{0} \right|\leq \frac{1}{K} $$ Now de define the function $\sigma: \mathbb{N}\to \mathbb{N}$ by $\sigma(1):=1$ and $\sigma(k):= \min\left\{ N\in \mathbb{N}: \forall n\geq N, \left| y_{n}-x_{0} \right|\leq \frac{1}{k}   \right\}$. Notice that is it well-defined and increasing and induces a subsequence $(y_{\sigma(k)})^\infty_{k=1}$, which, since $(y_n)^\infty_{n=1}$ is convergent, implies that $\lim_{ n \to \infty }y_{n}=\lim_{ k \to \infty }y_{\sigma(k)}$. Thus we have $$\begin{align} \forall K\;\forall k\geq K, \left|  y_{\sigma(k)}-x_{0}\right|\leq \frac{1}{K} \end{align}$$ Which implies $$ \begin{align} \forall K\;\forall k\geq K, \frac{1}{a^{\frac{1}{k}}}\leq \frac{a^{y_{\sigma(k)}}}{a^{x_{0}}} \leq a^{\frac{1}{k}}\end{align} $$ And by limit laws we have that $\lim_{ k \to \infty }a^{y_{\sigma(k)}}=a^{x_{0}}$. By well defined-ness of real exponentiation this also implies that $\lim_{ n \to \infty }a^{y_{n}}=a^{x_{0}}$, and since the original choice of sequence is arbitrary we are done.
>
>**Q.E.D.**

>[!quote]- Continuity of $f:(0,+\infty)\to \mathbb{R}: x\mapsto x^{p}$
>We first prove that $\lim_{ x \to 1:x\in (0,+\infty) }x^{p}=1$, in order to prove that we show that for any integer $n$, $\lim_{ x \to 1:x\in (0,+\infty) }x^n=1$. If $n=0$ the claim is trivial, if $n$ is positive then the claim follows by induction on the limit laws regarding the product of functions and if $n$ is negative then it basically falls under the same case as when $n$ is positive. Which proves $\lim_{ x \to 1:x\in (0,+\infty) }x^n=1$ for any integer $n$. Now we notice that $$ \lfloor p \rfloor \leq p\leq \lfloor p \rfloor +1 $$ and thus since $x$ is always positive we have that $$ x^{\lfloor p \rfloor }\leq x^{p}\leq x^{\lfloor  p\rfloor 	+1} $$ Applying the continuous version of the squeeze theorem we have that $\lim_{ x \to 1:x\in (0,+\infty) }x^{p}=1$ for all real numbers $p$. Now we use this to prove that $\lim_{ x \to x_0:x\in (0,+\infty) }x^{p}=x_{0}^{p}$. Take some arbitrary sequence $(a_n)^\infty_{n=0}$ that converges to $x_{0}$. Then we have that $$ \forall \delta>0 \exists N:\forall n\geq N, \left| a_{n}-x_{0} \right| \leq \delta x_{0} $$ We now define the sequence $(\alpha_n)^\infty_{n=0}$ by $\alpha_{n}:=\frac{a_{n}}{x_{0}}$ (which is possible since $x_{0}$ is always non-zero) and thus write $$ \forall \delta>0 \exists N: \forall n\geq N, \left| x_{0}\alpha_{n}-x_{0} \right| \leq \delta x_{0} $$ Or in other words, $\alpha_{n}$ converges to $1$. Since we showed that $\lim_{ x \to 1:x\in (0,+\infty) }x^{p}=1$ we know that $$ \forall \varepsilon >0\exists N:\forall n\geq N, \left| \alpha_{n}^{p}-1 \right| \leq \frac{\varepsilon}{x_{0}^{p}}$$ But by the definition of $\alpha_{n}$ this implies that $$ \forall \varepsilon>0 \exists N: \forall n\geq N, \left| a_{n}^{p}-x_{0}^{p} \right|\leq \varepsilon  $$ In other words, every arbitrary sequence $(a_n)^\infty_{n=1}$ that converges to $x_{0}$, induces a convergent sequence $(f(a_{n}))^\infty_{n=0}$ which converges to $f(x_{0})$. In other words $f$ is continuous over the domain $(0,+\infty)$ by the sequential definition.
>
>**Q.E.D.**

