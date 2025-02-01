
---

mathLink: $\mathbb R$

---
Date created: 2023-11-13 15:40
Tags:  #Type/Object #Topic/Real_Analysis 
 
Types: [[Positive and negative real numbers]]
Examples: _Not applicable_
Construction: [[Set of real numbers]], [[Addition of the real numbers]], [[Multiplication of the real numbers]], [[Subtraction of the real numbers]], [[Division of the real numbers]], [[Ordering of the real numbers]], [[Upper bounds]]
Generalization: [[Field of the real numbers]], [[Fields]]

Properties: [[Cardinality of the real numbers]], [[Least upper bounds]], [[Completeness of the real numbers]]
Sufficiencies: _Not applicable_
Equivalences: [[Real numbers (Dedekind cuts definition)]]
Justifications: [[Cauchy sequences]], [[Equality of the real numbers is well defined]], [[Scaffolding limits are normal limits]]

---  

Giving a informal definition for the reals is very hard, in the sense that an informal definition will usually be **extremely** informal and useless for proofs. We thus immediately skip to an very formal definition, used for constructing all it's properties.

> [!quote] Definition: Real number
> A real number is an object of the form $\text{LIM}_{n\rightarrow \infty}\;a_n$, where $(a_n)^\infty_{n=1}$ is a [[Cauchy sequences|Cauchy sequence]] of [[Rational numbers|rational numbers]].

Where $\text{LIM}_{n\rightarrow \infty}$ denoted the "formal" limit. We then proceed to define a notion of equality:

> [!quote] Definition: Equality of real numbers
> Two real numbers $\text{LIM}_{n\rightarrow \infty}\;a_n$ and $\text{LIM}_{n\rightarrow \infty}\;b_n$ are said to be equal if the [[Cauchy sequences]] $(a_n)^\infty_{n=1}$ and $(b_n)^\infty_{n=1}$ are [[Cauchy sequences|equivalent]].

Note that by definition of the [[Limit of a sequence]] the following holds:

>[!quote] Notion: Scaffolding limits are the same as normal limits
>$$\text{LIM}_{n\rightarrow \infty} a_n=\lim_{n\rightarrow\infty}a_n$$

---

**_Remark_**: As there is no dedicated note for rational or real sequences, it is worth specifically mentioning that the (honestly obvious) [[Metric]] that is used for the [[Metric spaces|metric space]] of these sequences is the following: $$d:\mathbb R^2\rightarrow\mathbb R:(x,y)\mapsto|x-y|$$


