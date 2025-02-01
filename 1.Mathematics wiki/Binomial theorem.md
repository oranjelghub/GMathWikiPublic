
---

mathLink: auto

---
Date created: 2024-02-10 11:55
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Induction]]
References: _Not applicable_
Justifications: [[Finite series]], [[Factorial]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem Binomial theorem
> $$ \forall n\in \mathbb{N}\;\forall x,y\in \mathbb{R},\; (x+y)^{n}= \sum^{n}_{k=0}{n \choose k} x^k y^{n-k}=\sum^{n}_{k=0} \frac{n!}{k!(n-k)!} x^{k}y^{n-k}$$

>[!quote]- Proof: Binomial theorem
>We proceed by induction on $n$. For the base case $n=0$ we get $1=1$. Now assume for our induction hypothesis that we have for some $n$ $$(x+y)^{n}= \sum^{n}_{k=0}{n \choose k} x^k y^{n-k}$$ we want to show this implies $$(x+y)^{n+1}= \sum^{n+1}_{k=0}{n+1 \choose k} x^k y^{n-k+1}$$ Notice that we have by our hypothesis $$\begin{align} (x+y)^{n+1}&=(x+y)(x+y)^n\\  &=  (x+y)\sum^{n}_{k=0}{n\choose k}x^{k}y^{n-k} \end{align}$$ Distributing gives us $$\begin{align}    \sum^{n}_{k=0}{n\choose k}x^{k+1}y^{n-k}+\sum^{n}_{k=0}{n\choose k}x^{k}y^{n-k+1}    \end{align}$$ And changing indices $$ \sum^{n+1}_{k=1}{n\choose k-1}x^{k}y^{n-k+1}+\sum^{n}_{k=0}{n\choose k}x^{k}y^{n-k+1}  $$ We now remove the last entry of the first series and the first one of the other series $$ x^{n+1}+y^{n+1}+ \sum^{n}_{k=1}{n\choose k-1}x^{k}y^{n-k+1}+\sum^{n}_{k=1}{n\choose k}x^{k}y^{n-k+1}$$ Combining the two series we get $$x^{n+1}+y^{n+1}+\sum^{n}_{k=1}\left( {n\choose k-1}+{n\choose k} \right) x^{k}y^{n-k+1}$$ One can show with simple algebraic manipulations that ${n\choose k-1}+{n\choose k}={n+1\choose k}$ and thus $$ x^{n+1}+y^{n+1}+\sum^{n}_{k=1}{n+1\choose k}x^k y^{n-k+1} $$ By reinserting the loose $x$ and $y$ we obtain $$\sum^{n+1}_{k=0}{n+1 \choose k} x^k y^{n-k+1}  =(x+y)^{n+1}$$ Proving our induction step and closing the induction.
>
>**Q.E.D.**


