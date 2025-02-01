---
mathLink: auto
Date created: 2024-05-27 18:50
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Squeeze test of sequences]], [[Axiom of choice]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Intermediate value theorem
> Let $a < b$, and let $f : [a, b] → \mathbb{R}$ be a continuous function on $[a, b]$. Let $y$ be a real number between $f (a)$ and $f (b)$, i.e., either $f (a) ≤ y ≤ f (b)$ or $f (a) ≥ y ≥ f (b)$. Then there exists $c ∈ [a, b]$ such that $f (c) = y$.

>[!quote] Proof: Intermediate value theorem
>WLOG assume that $f(a)\leq y\leq f(b)$. The claim is trivial if $y=f(a)$ or $y=f(b)$ so assume this isn't the case, in other words $f(a)<y<f(b)$. We define $$ E:=\{ x\in X: f(x)< y \} $$ $E$ is clearly bounded so we can define $c:=\sup E$. Now define $$ \mathcal{C}_{N}:=\left\{  x\in E: c- \frac{1}{N} \leq f(x) \right\} $$ We know that $\mathcal{C}_{N}$ is never empty by the definition of $c$, thus we can define some choice function $(\chi_n)^\infty_{n=1}$ on $\bigcup_{i=1}^{\infty}\mathcal{C}_{i}$. Thus $$ c-\frac{1}{j}\leq \chi_{j}\leq c $$ And by the squeeze test we obtain $\lim_{ j \to \infty }\chi_{j}=c$ and since $f$ is continuous we have that $\lim_{ j \to \infty }f(\chi_{j})=f(c)$. Now since for all $n$ we have that $f(\chi_{n})<y$ because $\chi_{n}\in E$, we also know that $f(c)\leq y$ by the comparison principle. Since $f(b)>f(c)$ by assumption we know that $b\neq c$ and since $c\in [a,b]$ we have that $c<b$. This means that there exists some $K$ such that for all $k\geq K$ we have $c+ \frac{1}{k}< b$, which by the definition of $c$ means that $c+ \frac{1}{k}\not\in E$ and that $f\left( c+\frac{1}{k} \right)\geq y$. Since $f$ is continuous on $[a,b]$ we may take the limit of $c+ \frac{1}{k}$ as $k\to \infty$ and obtain $f(c)\geq y$. Since $f(c)\leq y$ and $f(c)\geq y$ we know that $f(c)=y$.
>
>**Q.E.D.**

