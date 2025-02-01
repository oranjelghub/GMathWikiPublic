
---

mathLink: auto

---
Date created: 2024-03-14 16:42
Tags: #Type/Theorem  #Type/Proof #Topic/Set_Theory #Topic/Real_Analysis 

Proved by: [[Induction]]
References: _Not applicable_
Justifications: [[Cardinality of a set]], [[Natural numbers]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Unions of at most countable sets are at most countable
> Let $\{ A_{k} \}_{1\leq k\leq n}$ be a family of $n$ countable sets, then the union $\bigcup_{1\leq k\leq n}A_{k}$ is also countable.

>[!quote] Proof: Unions of at most countable sets are at most countable
>We proceed by induction on $n$. We will actually only do the base case as the inductive step is really easy. Let $A_{1}:=A$ and $A_{2}:=B$, those sets are both countable and thus the following bijections exist $$ \begin{align} f:A\to \mathbb{N} \\ g: B\to \mathbb{N} \end{align} $$ Now consider $$ h:A\cup B: x\mapsto \left\{ \begin{align} &2f(x) \hspace{1cm}& &x\in A\backslash B \lor x\in A\cap B \\ &2g(x)+1 \hspace{1cm}& &x\in B\backslash A \end{align}  \right.  $$ This function is well defined as no element of $A$ or/and $B$ could satisfy both conditions. The injectivity of $g$ and $f$ guarantee that the injectivity of $h$, and since all natural numbers are either even or uneven we know that they either $f$ or $g$ will take care of mapping some element in $A\cup B$ to it thanks to their surjectivity. Thus $h$ is a bijections to $\mathbb{N}$ and $A\cup B$ is countable.
>
>**Q.E.D.**



