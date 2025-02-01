
---

mathLink: auto

---
Date created: 2023-11-17 12:29
Tags: #Type/Theorem  #Topic/Real_Analysis 

Proved by: _Not applicable_
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Interspersing of reals by rationals
> $$\forall x,y\in \mathbb R: x<y \implies \exists q\in \mathbb Q: x<q<y$$

We can prove this the following way:

>[!quote] Proof: Interspersing of reals by rationals
>Let $x,y$ be real numbers such that $x < y$. Then $y-x > 0$ so we know there exists a positive integer $b$ such that $y-x > 1/b > 0$ (Exercise 5.4.4 Terence Tao analysis 1). Multiplying through by $b$ we have $by - bx > 1$. By Exercise 5.4.3 Terence Tao analysis 1, there is some integer $n$ such that $n \leq bx < n+1$. By $n \leq bx$ we have $n+1 \leq bx+1$. Also from $by - bx > 1$ we have $bx+1 < by$. Combining the inequalities, we have $bx < n+1 \leq bx+1 < by$. Dividing through by b, we have $x < (n+1)/b < y$, so we may take $q:=(n+1)/b$ as the rational number we seek.
>
>**Q.E.D.**



