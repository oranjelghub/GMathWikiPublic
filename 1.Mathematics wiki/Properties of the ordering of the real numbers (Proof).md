
---

mathLink: auto

---
Date created: 2023-11-15 15:38
Tags: #Type/Proof  #Topic/Real_Analysis 

Proved by: [[Ordering of the real numbers]], [[Field of the real numbers]], [[Closure of the non-negative reals]]
References: _Not applicable_
Justifications: [[Sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

We shall only proof [[Ordering of the real numbers|properties 4,5,6]]

> [!quote]- $x\in \mathbb R^{+}\implies x^{-1}\in \mathbb R^+$
> We know that according to the field properties we have $xx^{-1}=1$ and since $x$ is non-zero positive we must have that $x^{-1}$ is also non-zero. Then since $x$ is positive and $1$ to $x^{-1}$ must also be positive.
> 
> **Q.E.D.**

>[!quote]- $x>y \implies x^{-1}<y^{-1}$
>Let $y$ be positive, so $x^{-1}$ and $y^{-1}$ are also positive, if $x^{-1}\geq y^{-1}$ then we have that $xx^{-1}>yx^{-1}\geq yy^{-1}$ but this implies $1>1$, a contradiction.
>
>**Q.E.D.**

>[!quote]- Given two rational [[Sequences]] $(a_n)^\infty_{n=1}$ and$(b_n)^\infty_{n=1}$ such that $a_n\geq b_n$ for all $n\geq 1$ then $\text{LIM}_{n\rightarrow \infty}\;a_n\geq\text{LIM}_{n\rightarrow \infty}\;b_n$
>If for all $n$ we have that $a_n\geq b_n$ then we know that $a_n-b_n\geq 0$. We then define the sequence $c_n=a_n-b_n$ which according to [[Closure of the non-negative reals]] means there is a positive real number $x$ such that $x=\text{LIM}_{n\rightarrow\infty}\;c_n$ and definition we have $\text{LIM}_{n\rightarrow\infty}\;c_n=\text{LIM}_{n\rightarrow\infty}\;a_n-\text{LIM}_{n\rightarrow\infty}\;b_n$ and since $c_n$ is positive we have that $\text{LIM}_{n\rightarrow\infty}\;a_n\geq \text{LIM}_{n\rightarrow\infty}\;b_n$
>
>**Q.E.D.**


