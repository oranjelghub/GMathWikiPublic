
---

mathLink: auto

---
Date created: 2024-02-01 12:44
Tags: #Type/Object #Topic/Real_Analysis 

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: [[Series over finite sets (Properties)]], [[Fubini's theorem for finite series]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Cardinality of a set]], [[Finite series]], [[Series on finite sets are well-defined]]

---  

We would like to generalize the process of summing to use any arbitrary set for the indexing.

> [!quote] Definition: Summations over finite sets
> Let $X$ be a finite set with $\# X=n$ and let $f$ be a function $f:X\to\mathbb R$. Using any arbitrary bijection $g:\{ i\in \mathbb N:1\leq i\leq n \}\to X$ we define $$\sum^{}_{x\in X}f(x):=\sum^{n}_{i=1}f(g(i))$$

Notice that we implicitly claim that the choice of bijection doesn't matter. We prove this here: [[Series on finite sets are well-defined]]


