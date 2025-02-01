
---

mathLink: auto

---
Date created: 2023-11-13 12:08
Tags: #Type/Object #Topic/Real_Analysis 

Types: _Not applicable_
Examples: [[Harmonic sequence]]
Construction: [[Real numbers]]
Generalization: [[Functions]], [[Sequences]]

Properties: [[Bounded rational sequences]], [[Cauchyness is transitive across equivalence]], [[Boundedness away from zero]], [[Convergence of sequences]]
Sufficiencies: _Not applicable_
Equivalences: [[Limit definition for sequential equivalence]]
Justifications: [[Sequences]], [[Metric spaces]], 

---  

> [!quote] Definition: Cauchy sequence
> Given a [[Metric spaces|metric space]] $(X,d)$, a [[Sequences|sequence]] is said to be Cauchy if and only if for every [[Real numbers|real]]$^1$ $\varepsilon>0$ there exists a $N\in \mathbb Z$ such that for all $m,n\geq N$ we have that $d(x_n,x_m)\leq\varepsilon$.

We now develop an equivalence between Cauchy sequences.

> [!quote] Definition: Equivalent Cauchy sequences
> Given a metric space $(X,d)$ and two Cauchy sequences $(a_n)^\infty_{n=m}$ and $(b_n)^\infty_{n=q}$ defined in that metric space, we say the two sequences are equivalent if and only if for every  [[Real numbers|real]]$^1$ $\varepsilon>0$ there exists a $N\in \mathbb Z$ such that for all $n\geq N$ we have $d(a_n,b_n)\leq\varepsilon$.

This equivalence does indeed from an [[Equivalence relations|equivalence relation]], which we prove [[Equivalence of Cauchy sequences is an equivalence relation|here]].

Also notice that every Cauchy sequence [[Convergence of sequences|converges]]

---

**_Remark_**$^1$: We can substitute [[Real numbers|real]] by [[Rational numbers|rational]] if the former hasn't been developed yet and then proceed to prove that it makes no difference whether our definition ranges over [[Real numbers]] or the [[Rational numbers]]. 
