
---

mathLink: auto

---
Date created: 2023-11-29 15:56
Tags: #Type/Notion #Topic/Real_Analysis 

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Supremum and infimum]], [[Extended real numbers]]

---  

We extend the definition of [[Supremum and infimum]] to the [[Extended real numbers]].

> [!quote] Notion: Supremum and infimum of sets of extended reals
> We define $\sup(E)$ where $E\subseteq \bar {\mathbb R}$ as follows:
> - In the case of $E\subseteq R$: $\sup(E):=\sup_{\mathbb R}(E)$ where $\sup_{\mathbb R}$ denotes the supremum in the sense of [[Supremum and infimum]].
> - If $+\infty\in E$: $\sup(E):=+\infty$
> - If $+\infty \notin E$ but $-\infty \in E$: $\sup(E):=\sup(E\backslash\{-\infty\})$

In the same fashion we can define the infimum or we can be smarter and just define: $$\inf(E):=-\sup(-E)$$
From this definition the following properties emanate:

>[!quote] Notion: Properties of sup and inf of extended reals
>- $\forall x\in E:x\leq\sup(E)\land x\geq\inf(E)$
>- $\forall x:M\in\bar{\mathbb R}\land x\leq M\implies \sup(E)\leq M$ 
>- $\forall x:M\in\bar{\mathbb R}\land x\geq M\implies \inf(E)\geq M$ 

One can verify these properties by partitioning into cases.