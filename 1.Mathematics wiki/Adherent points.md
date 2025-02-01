
---

mathLink: auto

---
Date created: 2023-11-14 20:42
Tags: #Type/Object #Topic/Topology 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Closed subsets]]
Generalization: [[Adherent points (Topological)]]

Properties: [[Properties of the closure of a set]]
Sufficiencies: _Not applicable_
Equivalences: [[Sequential adherence]]
Justifications: [[Metric spaces]], [[Open balls]], [[Sets]] 

---  

Adherent points is a notion that pertains to [[Sets]] in [[Metric spaces]] and is defined as follows:

> [!quote] Definition: Adherent point
> Given a subset $Y$ of a metric space $X$, a point $x\in X$ is said to be adherent to $Y$ if and only if:$$\forall r>0: B(x,r)\cap Y\neq \emptyset$$
> Equivalently a point $x$ is adherent if and only if for every real $\varepsilon>0$ there exists some $y\in X$ such that $$ d(x,y)\leq \varepsilon $$

We usually denote the set of all adherent points of a subset $Y$ as $\bar Y$ or $\text{adh}(Y)$. This set is also called the closure of $Y$. $$x\in \bar Y\iff x\;\text{is adherent to}\; Y$$