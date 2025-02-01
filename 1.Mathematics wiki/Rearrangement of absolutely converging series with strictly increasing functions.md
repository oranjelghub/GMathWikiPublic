
---

mathLink: auto

---
Date created: 2024-03-11 16:30
Tags: #Type/Theorem  #Topic/Real_Analysis 

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Infinite series]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Rearrangement of absolutely converging series with strictly increasing functions
> Let $\sum^{\infty}_{n=0}a_{n}$ be a absolutely converging series of real numbers and let $f:\mathbb{N}\to \mathbb{N}$ be a strictly increasing function then $\sum^{\infty}_{m=0}a_{f(m)}$ is also absolutely convergent.

>[!quote] Proof: Rearrangement of absolutely converging series with strictly increasing functions
>Remember that $n\leq f(n)$, we use this and the fact that $f$ is strictly increasing to assert that $$ \forall N,\alpha\in \mathbb{N}; \left\{ f(n):n\in \mathbb{N}; \alpha\leq n\leq N \right\} \subseteq \left\{ m: m\in \mathbb{N}; \alpha\leq m\leq f(N) \right\}  $$ Since the original series is absolutely convergent we know that for all $\varepsilon>0$ there exists some $K$ such that for all $p,q\geq K$ $$ \left| \sum^{q}_{n=p}|a_{n}| \right|\leq \varepsilon  $$ Then $$ \sum^{q}_{m=p}|a_{f(m)}|=\sum^{}_{n\in \{ f(m):m\in \mathbb{N}; p\leq m\leq q \}}|a_{n}|\leq \sum^{}_{n\in \{ n: n\in \mathbb{N}; p\leq n\leq f(q)\}}|a_{n}|=\left| \sum^{f(q)}_{n=p}|a_{n}| \right|\leq \varepsilon $$
>Which ties up the proof.
>
>**Q.E.D.**


