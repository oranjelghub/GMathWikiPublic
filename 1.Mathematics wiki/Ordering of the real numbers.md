
---

mathLink: auto

---
Date created: 2023-11-13 21:47
Tags: #Type/Notion #Topic/Real_Analysis  

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Field of the real numbers]]
Generalization: [[Ordered sets]]

Properties: [[Closure of the non-negative reals]], [[Bounding of reals by rationals]], [[Archimedean property]], [[Interspersing of reals by rationals]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Positive and negative real numbers]], [[Sequences]], [[Properties of the ordering of the real numbers (Proof)]]

---  

We define an ordering on [[Real numbers]] in a similar fashion to the [[Rational numbers]].

> [!quote] Notion: Ordering the [[Real numbers|real numbers]]
> $$\begin{align}x>y \iff x-y \;\text{is positive}\\
> x<y \iff x-y\;\text{is negative}
> \end{align}$$

And we obviously extend $x\geq y \iff x>y \lor x=y$, and do the same for $\leq$. From this definition we can develop similar properties as the one from the 

Note that we can extend the order of [[Rational numbers]] pretty easily. $$q>q' \land q,q'\in \mathbb Q\iff q>q'\land q,q'\in \mathbb R$$
The ordering of the real numbers has very similar properties than the [[Ordering of the rational numbers]], their proofs also being similar.

>[!quote]- Notion: Properties of the ordering of the real numbers
>1. Given any two real numbers $x$ and $y$ at exactly one of the following is true:
>	1. $x<y$
>	2. $x=y$
>	3. $x>y$
>2. $x<y\iff y>x$
>3. $x<y\implies x+z< y+z$
>4. $x<y\implies xz<yz$ if $z$ is positive
>5. $x$ is positive $\implies x^{-1}$ is positive
>6. $x>y\implies x^{-1}<y^{-1}$
>7. Given two rational [[Sequences]] $(a_n)^\infty_{n=1}$ and$(b_n)^\infty_{n=1}$ such that $a_n\geq b_n$ for all $n\geq 1$ then $\text{LIM}_{n\rightarrow \infty}\;a_n\geq\text{LIM}_{n\rightarrow \infty}\;b_n$

Which we prove here [[Properties of the ordering of the real numbers (Proof)|here]]


