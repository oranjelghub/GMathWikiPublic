
---

mathLink: auto

---
Date created: 2023-11-14 12:24
Tags: #Type/Object #Topic/Topology 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Interior points]], [[Open subsets in metric spaces]], [[Adherent points]], [[Closed subsets]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Metric spaces]], [[Sets]]

---  

A open ball is a notion that pertains to [[Metric spaces]] and is defined as follows: 

> [!quote] Definition: Open ball
> Given a metric space $(X,d)$, the open ball $B(x,r)$ with center $x$ and radius $r$ is the set: $$B(x,r):=\{y\in X: d(x,y)<r\}$$

From this definition one can easily notice and show the following two properties:

>[!quote] Notion: Simple properties of open balls
>- $$\bigcup_{r>0}B(x,r)=X$$
>- $$\bigcap_{r>0}B(x,r)=\{x\}$$

We also notice that an open ball in $(X,d)$ is always an [[Open subsets in metric spaces|open subset]] in $X$, hence it's name "open" ball.