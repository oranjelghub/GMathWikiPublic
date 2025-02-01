
---

mathLink: auto

---
Date created: 2023-12-15 15:34
Tags: #Type/Theorem  #Type/Proof #Topic/Linear_Algebra 

Proved by: [[Linear dependence and independence]], [[Bases of vector spaces]], [[Span of a subset of a vector space]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Steinitz lemma
> Let $V$ be a $F$-vector space. 
> 1. If there is set of $m$ vectors $\{ v_{i} \}_{1\leq i\leq m}$ spanning $V$, then every $W\subseteq V$ with more than $m$ vectors is a set containing linearly dependent vectors.
> 2. If there is set of $n$ linearly independent vectors $\{ v_{i} \}_{1\leq i\leq n}$, then every $W\subseteq V$ with less than $n$ vectors is a set that does not span $V$.

>[!quote] Proof: Sets of linearly independent vectors have smaller cardinality than a basis
>We start with 1. Let $\{ w_{i} \}_{1\leq i\leq k}$ be a set of vectors with $k>m$. Sine $\{ v_{i} \}_{1\leq i\leq m}$ spans $v$ we know that $$ w_{j}=\sum^{m}_{i=1}\lambda_{ij}v_{i} $$We now want to show that $\{ w_{i} \}_{1\leq i\leq k}$ are not linearly independent, i.e. we want to show that $$ \sum^{k}_{j=1}\mu_{j}w_{j}=0 $$ has a non trivial solution. Notice that $$ 0=\sum^{k}_{j=1}\mu_{j}w_{j}=\sum^{m}_{i=1}v_{i}\left( \sum^{k}_{j=1}\mu_{j}\lambda_{ij} \right) $$It is sufficient for every $\left( \sum^{k}_{j=1}\mu_{j}\lambda_{ij} \right)$ to be zero. So this induces a homogeneous system of linear equations in $m$ equations and $k>m$ variables. But since there are more variables than equations we will at the very least have one degree of freedom for the solutions. In other words, there are non trivial solutions, meaning that $\{ w_{i} \}_{1\leq i\leq k}$ are linearly dependent. We continue with 2. We proceed by contradiction and suppose that $\{ w_{j} \}_{1\leq j\leq k}$ spans $V$. Then $$ 0=\sum^{n}_{i=1}\lambda_{i}v_{i} $$should only have the solution $(\lambda_{i})_{1\leq i\leq n}=(0)_{1\leq i\leq n}$. Since we assumed $\{ w_{j} \}_{1\leq j\leq k}$ spans $V$ we can write $$ 0=\sum^{k}_{j=1}w_{j}\sum^{n}_{i=1} \lambda_{i}\mu_{ij}$$We denote $\sum^{n}_{i=1}\lambda_{i}\mu_{ij}=\phi_{j}$, the equation $$ 0=\sum^{k}_{j=1}w_{j}\phi_{j} $$Should still only have solution $\phi_{j}=0$ for all $j$ since this would generate a non trivial solution for $0=\sum^{n}_{i=1}\lambda_{i}v_{i}$ otherwise. On the other hand $=\sum^{k}_{j=1}w_{j}\phi_{j}$ induces a homogeneous system of linear equations in $k$ equations and $n$ variables (where $k<n$). But since there are more variables than equations we will at the very least have one degree of freedom for the solutions. In other words, there are non trivial solutions, which is a contradiction.
>
>**Q.E.D.**

