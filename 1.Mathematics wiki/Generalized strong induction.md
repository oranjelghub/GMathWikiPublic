---
mathLink: auto
Date created: 2024-04-29 19:54
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Well-ordered set]]
References: _Not applicable_
Justifications: [[Sets]], [[Induction]]

Specializations: [[Strong induction]]
Generalizations: _Not applicable_

---

> [!quote] Theorem: Generalized strong induction
> Let $X$ be a well-ordered set with an ordering relation $\leq_{X}$, and let $P(n)$ be a property pertaining to an element $n \in X$. Suppose that for every $n \in X$, we have the following implication: if $P(m)$ is true for all $m \in X$ with $m <_{X} n$, then $P(n)$ is also true. Then $P(n)$ is true for all $n \in X$.

>[!quote] Proof: Generalized strong induction
>We define the set $$ Q:=\{ n\in X: \exists m<_{X}n \;, P(m)\text{ is false}\} $$ Suppose for the sake of contradiction that generalized strong induction was false, then $Q$ would be non-empty, and since $Q$ is non-empty and $X$is well-ordered we know there exists some $\min Q$ in $Q$. Now we can construct the set $$ Q_{n}:=\{ m\in X: m<_{X}n \land P(m)\text{ is false} \} $$ We notice that $Q_{\min Q}$ is non-empty as well and we thus know there exists some $\min Q_{\min Q}$ in $Q_{\min Q}$. But now notice that for all $k<_{X}\min Q_{\min Q}$, $P(k)$ is true, which by the given implication should imply that $P(\min Q_{\min Q})$ is true as well, which is a contradiction since normally by definition of $\min Q_{\min Q}$ we know that $P(\min Q_{\min Q})$ should be false. Thus the original assumption that $Q$ is non-empty must be wrong and we know that $P(n)$ is true for all $n\in X$.
>
>**Q.E.D.**

