
---

mathLink: auto

---
Date created: 2024-03-10 18:13
Tags: #Type/Proof  #Topic/Real_Analysis 

Proved by: [[Rearrangement of series of non-negative reals]]
References: _Not applicable_
Justifications: [[Infinite series]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Proof: Rearrangement of absolutely converging series
> We write $\bar{L}:=\sum^{\infty}_{n=0}|a_{n}|$ which we can since the series is absolutely convergent. As a matter of fact we also have $\bar{L}=\sum^{\infty}_{n=0}a_{f(n)}$ since we proved this is the case for non-negative series. Now write $L=\sum^{\infty}_{m=0}|a_{m}|$, we want to prove that $L=\sum^{\infty}_{m=0}a_{f(m)}$. To prove this we want to show that for every positive $\varepsilon$ there exists some $M$ such that for all $M'\geq M$ we have that $$ \left| L-\sum^{M'}_{m=0}a_{f(m)} \right| \leq \varepsilon $$ First notice that we can find a $N_{1}$ such that for all $p,q\geq N_{1}$ we have $$ \left| \sum^{q}_{n=p}|a_{n}| \right|  \leq \frac{\varepsilon}{2}$$ Which also means there is some $N\geq N_{1}$ such that for all $k\geq N$ $$ \left| L-\sum^{k}_{n=0}a_{n} \right| \leq \frac{\varepsilon}{2} $$ Now notice that since $(f^{-1}(n))^N_{n=0}$ is a finite sequence that there exists some $M$ such that $f^{-1}(n)\leq M$ for all $0\leq n\leq N$. This implies that for all $M'\geq M$ $$ \left\{ n: n\in \mathbb{N}, n\leq N \right\} \subseteq  \left\{  f(m):m\in \mathbb{N}, m\leq M'\right\}  $$ Meaning that we can write $$ \sum^{M'}_{m=0}a_{f(m)}=\sum^{}_{n\in\{ f(m):m\in \mathbb{N}, m\leq M' \}}a_{n}=\sum^{N}_{n=0}a_{n}+\sum^{}_{n\in X}a_{n} $$ where $X$ is the set $$ X:= \left\{  f(m):m\in \mathbb{N}, m\leq M'\right\}\backslash \left\{ n:n\in \mathbb{N}, n\leq N \right\} $$ Now since $X$ is finite it is also bounded and thus there exists some $q$ such that $$ X \subseteq \left\{ n\in \mathbb{N}: N+1\leq n\leq q \right\}  $$ Using this knowledge we get the following $$ \left| L-\sum^{M'}_{m=0}a_{f(m)} \right| =  \left|  \left( \sum^{N}_{n=0}a_{n}+\sum^{}_{n\in X}a_{n} \right) -L\right| \leq \left| \sum^{N}_{n=0}a_{n}-L \right| + \left| \sum^{}_{n\in X}a_{n} \right| \leq \left| \sum^{N}_{n=0}a_{n}-L \right| + \sum^{}_{n\in X}|a_{n}| \leq\left| \sum^{N}_{n=0}a_{n}-L \right| + \sum^{q}_{N+1}|a_{n}| $$ And by our choice of $N$ we then get $$ \forall \varepsilon \exists M:\forall M'\geq M; \left| L-\sum^{M'}_{m=0}a_{f(m)} \right|\leq \varepsilon $$ Thus proving that the rearanged series converges absolutely and more pricesily to the same limit as the normal series.
> 
> **Q.E.D.**



