---
mathLink: Stieltjes-$\mathbb{Q}$ function has a non-differentiable area function on the rationals between $0$ and $1$
Date created: 2024-09-22 17:29
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Monotonicity of the Stieltjes-Q function]], [[Continuity of the Stieltjes-Q function on Q-R]], [[Discontinuity of the Stieltjes-Q function on Q]]
References: _Not applicable_
Justifications: [[Area functions of real valued functions]], [[Stieltjes-Q function]], [[Differentiation of real valued functions]], [[Left and right limits of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Stieltjes-$\mathbb{Q}$ function has a non-differentiable area function on the rationals between $0$ and $1$
> Let $F(x)$ be define by $$ F(x):= \int_{0}^{x}\Xi_{\mathbb{Q}}\; dx$$Where $\Xi_{\mathbb{Q}}$ is the Stieltjes-$\mathbb{Q}$ function with respect to some arbitrary bijective sequence $(q_n)^\infty_{n=0}$ which maps $\mathbb{N}\to \mathbb{Q}$. Then $F$ is not-differentiable on $\mathbb{Q}\cap[0,1]$.

>[!quote]- Proof: Stieltjes-$\mathbb{Q}$ function has a non-differentiable area function on the rationals between $0$ and $1$
>Let $q\in \mathbb{Q}\cap[0,1]$, we split into the cases: $q=0$, $q=0$, $0<q<1$. We first handle $0<q<1$, if $F$ were to be differentiable at $q$ then $$ \lim_{ x \to q:x\in (0,q) } \frac{{F(x)-F(q)}}{x-q} = \lim_{ x \to q:x\in (q,1) } \frac{{F(x)-F(q)}}{x-q}$$So we assume for the sake of contradiction that the limits exist and are equal to each other. Since $q\in \mathbb{Q}$ we know $q=q_{n}$ for some $n\in \mathbb{N}$, we know that for all $1>x>q$ the following inequality holds $$ \Xi_{\mathbb{Q}}(q)+2^{-n}\leq \Xi_{\mathbb{Q}}(x) $$We integrate over the inequality get over the interval $[q,x]$ and get $$ (x-q)(\Xi_{\mathbb{Q}}(q)+2^{-n})\leq F(x)-F(q) $$or $$  \Xi_{\mathbb{Q}}(q)+2^{-n}\leq \frac{{F(x)-F(q)}}{x-q}$$Meaning that $$\Xi_{\mathbb{Q}}(q)+2^{-n}\leq  \lim_{ x \to q:x\in (q,1) } \frac{{F(x)-F(q)}}{x-q}  $$Similarly, by the monotonicty of $\Xi_{\mathbb{Q}}$, if $x<q$ then $\Xi_{\mathbb{Q}}(x)<\Xi_{\mathbb{Q}}(q)$. By once again integrating over the inequality, dividing by $q-x$ and taking the left limit, we get $$ \lim_{ x \to q:x\in (0,q) }\frac{F(x)-F(q)}{x-q}\leq \Xi_{\mathbb{Q}}(q)  $$And thus $$\lim_{ x \to q:x\in (q,1) } \frac{{F(x)-F(q)}}{x-q}-\lim_{ x \to q:x\in (0,q) } \frac{{F(x)-F(q)}}{x-q}\geq 2^{-n}$$Contradicting the fact that the limits were supposed to be equal. The cases where $q=1$ and $q=0$ can be proven using similar arguments with the same inequalities used above. Thus $F$ is not differentiable on $\mathbb{Q}$.
>
>**Q.E.D.**

---
**_Remark_**: The inequalities used in the proof don't have their own note, instead they appear (with proof of course) in the proof of some other theorems, which will be mentioned in the *"Proved by"* section.