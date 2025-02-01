---
mathLink: auto
Date created: 2024-05-06 15:58
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Totally ordered set]], [[Bounds, strict bounds, minimal and maximal elements of a set]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Boundedness of all subsets implies finite set
> Let $X$ be a totally ordered set such that every subset has a minimum and a maximum, then $X$ is finite.

>[!quote] Proof: Boundedness of all subsets implies finite set
>We will proceed by contradiction, so assume this isn't the case. We construct recursively $$ \begin{align} a_{0}&:= \min X \\ a_{n+1}&:= \min X\backslash \{ a_{i}: i\leq n \} \end{align} $$ This sequence is always defined since the set $X\backslash A$ is never empty for some finite set $A$ if $X$ is infinite. It is obvious that $a_{n}<_{X}a_{n+1}$ and that $\{ a_{i}:i\in \mathbb{N} \}\subseteq X$ and thus by our original hypotheses there exists some maximum $\max \{ a_{i}:i\in \mathbb{N} \}\in \{ a_{i}:i\in \mathbb{N} \}$. But notice that this is a contradiction since this implies that there exists some $k$ such that $a_{k}=\max \{ a_{i}:i\in \mathbb{N} \}$, but this means we have $a_{k+1}>_{X}\max \{ a_{i}:i\in \mathbb{N} \}$. Thus $X$ must be finite.
>
>**Q.E.D.**


