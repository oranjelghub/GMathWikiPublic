
---

mathLink: auto

---
Date created: 2024-02-06 13:45
Tags: #Type/Theorem #Type/Proof  #Topic/Real_Analysis 

Proved by: [[Series over finite sets (Properties)]]
References: _Not applicable_
Justifications: [[Finite series]]

Specializations: [[Fubini's theorem for finite series]]
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Summation over a cartesian product
> Given two finite sets $X$,$Y$ and some function $f:X\times Y\to \mathbb{R}$ we have $$\sum^{}_{x\in X} \left( \sum^{}_{y\in Y}f(x,y) \right) =\sum^{}_{(x,y)\in X\times Y}f(x,y)$$

>[!quote] Proof: Summation over a cartesian product
>We induct on the cardinality of $X$. For $n$ the statement is easily shown to be true since we get sums over the empty set and thus $0=0$. Now assume that we have $$\sum^{}_{x\in X} \left( \sum^{}_{y\in Y}f(x,y) \right) =\sum^{}_{(x,y)\in X\times Y}f(x,y)$$ where $X$ has cardinality $n$. Now suppose that $X$ has cardinality $n+1$. We can then write $X=X'\cup \{ x_{0} \}$ where $x_0$ is some element in $X$, thus we also have $X':=X\backslash\{ x_{0} \}$ with $\#X'=n$. By properties of sums over finite sets we have $$\sum^{}_{x\in X} \left( \sum^{}_{y\in Y}f(x,y) \right) = \sum^{}_{x\in X'}\left( \sum^{}_{y\in y}f(x,y) \right) +\sum^{}_{y\in Y}f(x_{0},y)$$ Which by induction hypothesis is equal to $$\sum^{}_{(x,y)\in X'\times Y }f(x,y)+ \sum^{}_{y\in Y}f(x_{0},y)$$ We then use substitution to write $$\sum^{}_{(x,y)\in X'\times Y }f(x,y)+ \sum^{}_{(x,y)\in \{ x_{0} \}\times Y}f(x,y)$$ And since $X=X'\cup \{ x_{0} \}$ $$\sum^{}_{(x,y)\in X'\times Y }f(x,y)+ \sum^{}_{(x,y)\in \{ x_{0} \}\times Y}f(x,y)=\sum^{}_{(x,y)\in X\times Y}f(x,y)$$
>
>**Q.E.D.**




