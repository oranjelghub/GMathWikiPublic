
---

mathLink: auto

---
Date created: 2023-10-21 21:59
Tags: #Type/Proof #Topic/Logic 

Proved by: [[Well ordering of the natural numbers]]
References: _Not applicable_
Justifications: [[Sets]], [[Ordering of the natural numbers]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

Using the [[Well ordering of the natural numbers]] we can prove [[Induction]]. 

> [!quote] $1\in S \land \left( \forall k \in \mathbb{N}: k \in S \implies k+1 \in S  \right) \implies S= \mathbb{N}$
> Suppose to the contrary that $S \neq \mathbb{N}$. Then the [[Sets|set]] $\mathbb{N}\backslash S$ is nonempty, so by the well-ordering principle it has a least element $m$. Since $1\in S$ is given we know that $m>1$. But this implies that $m-1$ is also a natural number. Since $m-1<m$ and since $m$ is the least element in $\mathbb{N}$ such that $m \notin S$, we conclude that $m-1 \in S$. We now use the rest of the given information and define $k := m-1$ in $S$, to infer that $(m-1)+1=m$ belongs to $S$. But this statement contradicts the fact that $m \notin S$. Since $m$ was obtained from the assumption that $\mathbb{N}\backslash S$ is nonempty, we have obtained a contradiction. Therefore we must have $S=\mathbb{N}$.
> 
> **Q.E.D**

---

**_Remark_**: The proof proves an obviously equivalent statement to our definition of [[Induction]].


