
---

mathLink: auto

---
Date created: 2024-02-06 17:37
Tags: #Type/Theorem  #Topic/Real_Analysis 

Proved by: [[Series over cartesian products]], [[Series over finite sets (Properties)]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Fubini's theorem for finite series
> Let $X,Y$ be finite sets and let $f:X\times Y\to \mathbb{R}$. Then $$ \sum^{}_{x\in X}\left( \sum^{}_{y\in Y}f(x,y) \right) =\sum^{}_{y\in Y}\left( \sum^{}_{x\in X}f(x,y) \right)  $$

>[!quote] Proof: Fubini's theorem
> $$ \begin{align} \sum^{}_{x\in X}\left( \sum^{}_{y\in Y}f(x,y) \right) &= \sum^{}_{(x,y)\in X\times Y}f(x,y )\\ &=\sum^{}_{(y,x)\in Y\times X}f(x,y)\\ &= \sum^{}_{y\in Y}\left( \sum^{}_{x\in X}f(x,y) \right)
\end{align} $$


