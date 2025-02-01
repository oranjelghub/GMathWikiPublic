
---

mathLink: auto

---
Date created: 2023-11-14 13:03
Tags: #Type/Object #Topic/Topology 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Open subsets in metric spaces]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Metric spaces]], [[Sets]], [[Open balls]]

---  

Interior points is a notion that pertains to [[Sets]] in [[Metric spaces]] and is defined as follows:

> [!quote] Definition: Interior points
> Given a metric space $(X,d)$ and a subset $Y$ of $X$, we say a point $x\in X$ is an interior point of $Y$ if and only if: $$\exists r>0: B(x,r)\subset Y$$ 

We usually denote the set of all the interior points of a subset $Y$ as $\text{int}(Y)$ or $Y^°$. This set is usually called the interior of $X$.
$$x\in\text{int}(Y)\iff x\;\text{is an interior point of }\;Y$$
Evidently we have that $\text{int}(Y)\subseteq Y$.

--- 
**_Remark_**: Defining an interior point to require a Ball that is a subset or a set that is equal to the original subset is an entirely equivalent definition. A short mathematical explanation:
$$\begin{align}B(x,r_1)&=Y\subset X \\
\exists r_2:0<r_2<r_1\implies\exists B(x,r_2):B(x,r_2)&\subset B(x,r_1)\implies \exists B(x,r_2):B(x,r_2)\subset Y 

\end{align}$$
