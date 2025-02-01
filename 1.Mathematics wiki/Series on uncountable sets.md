
---

mathLink: auto

---
Date created: 2024-03-22 15:34
Tags: #Type/Notion #Topic/Real_Analysis 

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: [[Properties of series over infinite sets]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Series on countable sets]], [[Convergent series over uncountable sets must have only countable non-zero entries]], [[Supremum and infimum]]

---  

> [!quote] Notion Series on uncountable
> Let $X$ be a set (possibly uncountable), and let $f:X\to \mathbb{R}$ be a function. We say that the series $\sum^{}_{x\in X}f(x)$ is absolutely convergent if and only if $$  \sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\}  < \infty $$

Note that we haven't defined what the sum is actually equal to. To do this we need the following lemma: [[Convergent series over uncountable sets must have only countable non-zero entries]]. Thus we may define $$ \sum^{}_{x\in X}f(x):=\sum^{}_{x\in  X :f(x)\neq 0}f(x) $$

