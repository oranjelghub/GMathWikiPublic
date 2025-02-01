---
mathLink: auto
Date created: 2024-04-30 17:38
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Sets]], [[Functions]], [[Cardinality of a set]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Infinite donut lemma
> Let $A\subseteq B\subseteq C$ be sets and suppose there exists some injection $f:C\to A$, then $\left| A \right|=\left| B  \right|$

>[!quote] Proof: Infinite donut lemma
>Define $D_{0}:= B\backslash A$ and $D_{n+1}:=f(D_{n})$. Define the function $g:A\to B$ by putting $$ x\mapsto \left\{ \begin{align} &x& \hspace{1cm} x\not\in \bigcup_{i\in \mathbb{N_{0}}}D_{i} \\ f&^{-1}(x)& \hspace{1cm} x\in \bigcup_{i\in \mathbb{N_{0}}}D_{i} \end{align} \right.  $$We claim that $g$ is a bijection. Before that, notice that this function is well defined, since first of all only one of the two cases is possible at one time but also because $f^{-1}(x)$ is always defined since $x$ is in the image of some set under $f$. First we prove $g$ is injective. Suppose we have some $x,y\in A$ such that $x\neq y$, notice that we can split into 4 cases depending on their membership status regarding $D_{\mathbb{N}_{0}}:=\bigcup_{i\in \mathbb{N}_{0}}D_{i}$. If both $x,y \not\in D_{\mathbb{N}_{0}}$ is is pretty obvious that $g(x)\neq g(y)$. If only one of them is in $D_{\mathbb{N}_{0}}$ (WLOG assume it is $x$), then we know $f^{-1}(x)\in D_{k-1}$ for some $k\in \mathbb{N}$ and since $y \notin D_{\mathbb{N}_{0}}$ we once again know that $g(x)\neq g(y)$. Now we have the last case, suppose $x,y\in D_{\mathbb{N}_{0}}$, then it is pretty obvious that $f^{-1}(x)\neq f^{-1}(y)$ in order to avoid contradiction, and thus $g(x)\neq g(y)$. Thus $g$ is injective. Now to show it is surjective take some $b\in B$, we either have $b\not\in D_{\mathbb{N}_{0}}$ or $b\in D_{\mathbb{N}_{0}}$. In the case $b\not\in D_{\mathbb{N}_{0}}$ we obviously have $g(b)=b$. In the case $b\in D_{\mathbb{N}_{0}}$ we know that $b=g(f(b))$. Thus $b$ always has some predecessor and we have that $g$ is surjective and thus bijective. 
>
>**Q.E.D.**



