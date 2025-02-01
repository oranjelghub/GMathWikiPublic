---
mathLink: auto
Date created: 2024-09-23 14:52
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Mean value theorem]]
References: _Not applicable_
Justifications: [[Antiderivative of a real valued function]], [[Differentiation of real valued functions]] 

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Antiderivatives of real valued functions are unique up to some arbitrary constant
> Let $I$ be a bounded interval and $f:I\to \mathbb{R}$ some function. If $F:I\to \mathbb{R}$ and $G:I\to \mathbb{R}$ are both antiderivatives of $f$, then there exists some constant $C\in \mathbb{R}$ such that $$ F(x)=G(x)+C $$

>[!quote] Proof: Antiderivatives of real valued functions are unique up to some arbitrary constant
>The statement is trivial if $I$ is empty or a singleton. Fix some $x_{0}\in I$, then for any other $x\in I\backslash\{ x_{0} \}$, the function $F-G$ is differentiable on $[x,x_{0}]$ or $[x_{0},x]$. By the mean value theorem this implies $$ (F-G)'(\xi)=\frac{(F-G)(x)-(F-G)(x_{0})}{x-x_{0}} $$And since $F'(x)=f(x)=G'(x)$ we must have $F(x)-G(x)=F(x_{0})-G(x_{0})$. If we fix $$ C=F(x_{0})-G(x_{0}) $$Then for all $x\in I$ $$ F(x)=G(x)+C $$
>
>**Q.E.D.**

