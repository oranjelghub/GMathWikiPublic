
---

mathLink: auto

---
Date created: 2023-11-15 17:40
Tags: #Type/Theorem  #Topic/Real_Analysis 

Proved by: [[Bounded rational sequences]], [[Boundedness away from zero]], [[Interspersing of the rational numbers]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

The theorem goes as follows:

> [!quote] Theorem: Bounding of the reals by rationals
> Given $x$ a positive real number, there exists a rational number $q$ and a positive integer $N$ such that: $$q\leq x\leq N$$ $$\forall x\in \mathbb R^{+}:\exists q\in \mathbb Q \land \exists N\in \mathbb Z:q\leq x\leq N$$

And we can prove the theorem the following way: 

>[!quote] Proof: Bounding of reals by rationals
> $x$ is real thus we have $x=\text{LIM}_{n\rightarrow\infty}\;a_n$  and since the sequence is bounded and bounded away from zero we know that there exist rationals such that $q\leq a_n\leq r$. We also know that by interspersing of the rationals that there exists an integer $N$ such that $r\geq N$ and thus $q\leq a_n\leq N$ which by [[Ordering of the real numbers|property 6]] gives us $q\leq x\leq N$ with $q$ and $N$ positive.
> 
> **Q.E.D.**


