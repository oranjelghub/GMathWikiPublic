
---

mathLink: auto

---
Date created: 2024-03-18 16:44
Tags: #Type/Theorem  #Type/Proof #Topic/Set_Theory 

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Sets]], [[Axiom of choice]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Existence of infinite subsets of infinite sets with the same cardinality
> Let $X$ be some set, $X$ is infinite if and only if there exists some proper subset $Y\subset X$ where $|Y |= |X |$.

>[!quote] Proof: Existence of infinite subsets of infinite sets with the same cardinality
>We first prove it from left to right. We first conjecturise that every infinite set has a countable subset. Thanks to choice we know that $\prod_{n\in \mathbb{N}}X$ is non-empty and thus we can choose some $$ (x_{n})_{n\in \mathbb{N}}\in \prod_{n\in \mathbb{N}} X$$
>The set $X_{0}:=\{ x_{n}:n\in \mathbb{N} \}$ is then obviously countable and a proper subset of $X$. So since we now that every infinite set has some countable subset we want to show that $|X_{0}|=|X_{0}\backslash\{ x \}|$, as this extends quiet nicely. Notice that our sequence we just invoked is a bijection from $\mathbb{N}\to X_{0}$ (more precisely $f:n\mapsto x_{n}$), thus we have that there exists some $k\in \mathbb{N}$ such that $f(k)=x$. This being set we define the function $$ h:X_{0}\to X_{0}\backslash \{ f(k) \} : h(n)\mapsto \left\{ \begin{align}&f(n)&\hspace{1cm} n<k \\&f(n+1)&\hspace{1cm} n\geq k\end{align} \right. $$ One could easily control this does form a bijection. Thus $|X_{0}|=|X_{0}\backslash\{ x \}|$. Now we can extend the result to $|X_{}|=|X_{}\backslash\{ x \}|$ by the function $$ g:X_{}\to X_{}\backslash \{ x \} : g(x)\mapsto \left\{ \begin{align}&h(x)&\hspace{1cm} x&\in X_{0} \\&x &\hspace{1cm} x&\in X\backslash X_{0}\end{align} \right.  $$ Which once again is easily verified to be a bijection. Thus if $X$ is infinite then it has a proper subset $X\backslash \{ x \}$ which has the same cardinality. On the other hand suppose that $X$ has a proper subset $Y$ with the same cardinality. Then by properties of cardinality we must have $|Y|<|X|$, but notice that any finite cardinality would make this an immediate contradiction to the definition of ordering in $\mathbb{N}$. Thus $X$ must be infinite.
>
>**Q.E.D.**




