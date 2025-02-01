
---

mathLink: auto

---
Date created: 2024-03-22 15:43
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Finite series (Properties)]], [[At most countable unions of at most countable sets are at most countable]]
References: _Not applicable_
Justifications: [[Series on uncountable sets]], [[Axiom of choice]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Convergent series over uncountable sets must have only countable non-zero entries
> Let $X$ be a set (which could be uncountable), and let $f:X\to \mathbb{R}$ be a function such that the series $\sum^{}_{x\in X}f(x)$ is absolutely convergent. Then the set $\left\{ x\in X: f(x)\neq 0 \right\}$ is at most countable.

>[!quote]- Proof: Convergent series over uncountable sets must have only countable non-zero entries
>First of all the statement is quiet trivial if $X$ is countable or finite thus assume $X$ is uncountable. Since the series is absolutely convergent we define $$ M:=    \sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}  $$ We also introduce $$ X_{n}:= \left\{ x\in X: \left| f(x) \right|  > \frac{1}{n} \right\}  $$ We now conjecurize that each set $X_{n}$ has cardinality at most $Mn$. To prove this we proceed by contradiction. Suppose $\left| X_{n} \right|>Mn$, then picking some bijection $g:\mathbb{N}\to X_{n}$ we have$$ \sum^{\left| X_{n} \right| }_{n=0}\left| f(g(n))\right| \geq \sum^{\left| X_{n} \right| }_{n=0} \frac{1}{n}=\frac{\left|X_{n}\right|}{n}> M $$ A contradiction. Now we did assume $X_{n}$ was finite, but this assumption is not necessary, since if it was infinite then it must have some finite subset of cardinality higher then $Mn$, then the contradiction follows from considering the sum over that subset. Since the choice of $n$ is arbitrary we have that all $X_{n}$ are finite with cardinality at most $Mn$. Using the fact that countable unions of at most countable sets are at most countable (proof requires choice) we have that $\bigcup_{n\in \mathbb{N}}X_{n}$ is at most countable. We now state that $$ \left\{ x\in X:f(x)\neq 0 \right\} = \bigcup_{n\in \mathbb{N}}X_{n} $$ which is easily verified. Thus $\left\{ x\in X:f(x)\neq 0 \right\}$ is also at most countable.
>
>**Q.E.D.**

