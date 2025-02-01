
---

mathLink: auto

---
Date created: 2023-11-13 16:42
Tags: #Type/Notion  #Topic/Real_Analysis 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Ordering of the real numbers]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Proof of the trichotomy of the real numbers]], [[Real numbers]], [[Boundedness away from zero]]

---  

Since [[Real numbers|real numbers]] are defined through [[Cauchy sequences]] it is a bit trickier to properly define a notion of signedness for them. In our case the following definition works:

> [!quote] Definition: Positive, negative real number
> A real number $x$ is said to be positive if and only if it can be written as $x=\text{LIM}_{n\rightarrow \infty}\;a_n$ for some [[Cauchy sequences|Cauchy sequence]] $(a_n)^\infty_{n=1}$ which is [[Boundedness away from zero|positively bounded away from zero]]. A real number $x$ is said to be negative if and only if it can be written as $x=\text{LIM}_{n\rightarrow \infty}\;a_n$ for some [[Cauchy sequences|Cauchy sequence]] $(a_n)^\infty_{n=1}$ which is [[Boundedness away from zero|negatively bounded away from zero]]. 

From this follows the trichotomy of the real numbers:

>[!quote] Property: Trichotomy of the real numbers
>For every real number $x$ exactly one of the following is true:
>1. $x$ is positive
>2. $x$ is negative
>3. $x$ is zero

Which we prove [[Proof of the trichotomy of the real numbers|here]].

Note also that the notion of positivity and negativity perfectly translates from the [[Rational numbers]] to [[Real numbers]].

Furthermore one can easily show that $x+y$ is positive and $xy$ to if $x$ and $y$ are positive.