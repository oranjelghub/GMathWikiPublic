
---

mathLink: auto

---
Date created: 2024-02-01 21:08
Tags: #Type/Theorem  #Topic/Real_Analysis 

Proved by: [[Finite series (Properties)]]
References: _Not applicable_
Justifications: [[Series over finite sets]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Properties of summations over finite sets
> 1.  Given $X=\emptyset$ and some function $f:X\to \mathbb R$, we have $$\sum^{}_{x\in \emptyset}f(x)=0$$
> 2.  Given $X=\{ x_{0} \}$ and some function $f:X\to \mathbb{R}$, we have $$\sum^{}_{x\in X}f(x)=f(x_{0})$$
> 3.  Given $X$ with $\#X=n$ and some function $f:X\to \mathbb{R}$ and a bijection $g:Y\to X$, we have $$\sum^{}_{x\in X}f(x)=\sum^{}_{y\in Y}f(g(y))$$
> 4. Given $n\leq m$ integers and $X=\{ i\in \mathbb{Z}:n\leq i\leq m \}$, we have $$\sum^{n}_{i=n}a_{i}=\sum^{}_{i\in X}a_{i}$$
> 5. Given two disjoint sets $X,Y$ and a function $f:X\cup Y\to \mathbb{R}$, we have $$\sum^{}_{z\in X\cup Y}f(z)=\sum^{}_{x\in X}f(x)+\sum^{}_{y\in Y}f(y)$$
> 6. Given two functions $f,g:X\to \mathbb{R}$ and some constant $c\in \mathbb{R}$, we have $$\sum^{}_{x\in X}(f(x)+g(x))=\sum^{}_{x\in X}f(x)+\sum^{}_{x\in X}g(x)\land \sum^{}_{x\in X}cf(x)=c\sum^{}_{x\in X}f(x)$$
> 7. Given two functions $f,g:X\to \mathbb{R}$ such that $f(x)\leq g(x)$ for all $x\in X$, we have $$\sum^{}_{x\in X}f(x)\leq \sum^{}_{x\in X}g(x)$$
> 8. Given a finite set $X$ and a function $f:X\to \mathbb{R}$, we have $$ \left| \sum^{}_{x\in X}f(x) \right| \leq \sum^{}_{x\in X}\left| f(x) \right|  $$

We won't provide a proof but we quickly mention what the approaches for proving them are. The first 4 are proven by cleverly picking the bijection such that we obtain the desired equality. 5 can be proven by considering $\sigma\cup(\tau\circ\alpha^{-1})$ as shown in the diagram below and using a very slight change in indexing for the definition of a summation over a finite set. 6-8 can be proven by defining a sequence $a_{i}:=(f\circ h)(i)$ and using previous results ([[Finite series (Properties)]])
![[diagram-20240205.svg#invert_B]]