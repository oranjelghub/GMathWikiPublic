
---

mathLink: auto

---
Date created: 2023-11-15 18:32
Tags: #Type/Theorem  #Topic/Real_Analysis 

Proved by: [[Bounding of reals by rationals]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

The Archimedean property roughly states that no matter how small we take a number, if we multiply it enough we can make it arbitrarily big. The formal theorem goes as follows:

> [!quote] Theorem: Archimedean property
> $$\forall x,\varepsilon \in \mathbb R^+:\exists M\in \mathbb Z:M\varepsilon>x$$

The proof goes as follows:

>[!quote] Proof: Archimedean property
>By [[Bounding of reals by rationals]] we have that $\exists N: \frac{x}{\varepsilon}\leq N$ since $x/\varepsilon$ is positive. Now set $M:=N+1$ and we have $x<M\varepsilon$.
>
>**Q.E.D.**


