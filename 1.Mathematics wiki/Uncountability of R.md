---
mathLink: Uncountability of $\mathbb{R}$
Date created: 2024-04-30 16:49
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Well ordering of the natural numbers]], [[Properties of series over infinite sets]], [[Geometric series]]
References: _Not applicable_
Justifications: [[Sets]], [[Power sets]], [[Infinite series]], [[Series on countable sets]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Uncountability of $\mathbb{R}$
> $\mathbb{R}$ has the same cardinality as $\mathcal{P}(\mathbb{N})$ or in other words $\mathbb{R}$ is uncoutable.

>[!quote] Proof: Uncountability of $\mathbb{R}$
>Define the following function $$ f:A\mapsto \sum^{}_{n\in A}10^{-n}$$ where $A\in \mathcal{P}(\mathbb{N})$. Observe that this function is well defined since the series always converges because $\sum^{\infty}_{n=0}10^{-n}$ always converges. We claim that this function forms a bijection. We will simply show it's injectivity and then restrict the range to make it surjective. Now suppose for the sake of contradiction that we have two distinct sets $A\neq B$ such that $f(A)=f(B)$. Since the sets are distinct we can define  $x_{0}:=\min((A\backslash B)\cup (B\backslash A))$. WLOG assume that $x_{0}\in A\backslash B$, this means that for all $x<x_{0}$, $x\in A,B$ or $x\not\in A,B$. Now notice $$ \begin{align} 0&= \sum^{}_{n\in A}10^{-n}-\sum^{}_{n\in B} 10^{-n} \\ &= \sum^{}_{n\in A: n<x_{0}}10^{-n}+10^{-x_{0}}+\sum^{}_{n\in A:n> x_{0}}10^{-n} - \sum^{}_{n\in B: n<x_{0}}10^{-n}-\sum^{}_{n\in B:n> x_{0}}10^{-n} \\ &= 10^{-x_{0}}+\sum^{}_{n\in A:n> x_{0}}10^{-n}-\sum^{}_{n\in B:n> x_{0}}10^{-n} \\ &\geq  10^{-x_{0}}- \sum^{}_{n>x_{0}}10^{-n}\\ &\geq 10^{-x_{0}}- \frac{1}{9}10^{-x_{0}}\\ 0 &> 0 \end{align}  $$ A obvious contradiction, thus we must have $f(A)\neq f(B)$ and our function is a bijection from $\mathcal{P}(\mathbb{N})\to f(\mathcal{P}(\mathbb{N}))$. And since $f(\mathcal{P}(\mathbb{N}))$ is a subset of $\mathbb{R}$, we must have that $\mathbb{R}$ is uncountable.
>
>**Q.E.D.**

