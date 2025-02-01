
---

mathLink: auto

---
Date created: 2023-11-23 12:50
Tags: #Type/Object #Topic/Topology 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Rn]]
Generalization: [[Metric]]

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Cauchy-Schwarz inequality]]

---  

We define the following [[Metric]] on the set $\mathbb R^n$. This metric is called the Euclidian metric.

> [!quote] Definition: Euclidian metric
> $$d:\mathbb R^n \times \mathbb R^n\rightarrow [0,+\infty):((x_i)_{1\leq i\leq n},(y_i)_{1\leq i\leq n})\mapsto \sqrt{\sum^n_{i=1} (x_i-y_i)^2}$$

In order to verify that this does form a metric on $\mathbb R^n$ we verify all the metric axioms.

>[!quote]- Proof: $d(x,y)=0\iff x=y$
>Since $x=y$ we have that the $x_i-y_i$ is always equal to $0$, giving us a sum of zero which is obviously zero. Now we prove it the other way around. Suppose $\sqrt{\sum^n_{i=1} (x_i-y_i)^2}=0$ then $\sum^n_{i=1} (x_i-y_i)^2=0$. Now suppose for the sake of contradiction that $x\neq y$ but that the sum is equal to zero. Then we know $\exists \alpha: x_\alpha \neq y_\alpha$, we then rewrite our sum: $$\sum^n_{i=1} (x_i-y_i)^2=\sum^{\alpha-1}_{i=1} (x_i-y_i)^2+\sum^{n}_{i=\alpha+1} (x_i-y_i)^2+(x_\alpha-y_\alpha)^2$$
>But since $(x_\alpha-y_\alpha)^2> 0\land S_{\alpha-1}\leq 0\land S_{\alpha+1}\leq 0$ we have a contradiction since we say that: $$\sum^{\alpha-1}_{i=1} (x_i-y_i)^2+\sum^{\alpha+1}_{i=1} (x_i-y_i)^2 +(x_\alpha-y_\alpha)^2=0$$.
>
>**Q.E.D.**

>[!quote]- Proof: $d(x,y)=d(y,x)$
>Since the root function forms a bijection for $\mathbb R^+\rightarrow\mathbb R^+$ we have that $a=b\iff \sqrt{a}=\sqrt{b}$. It thus suffices to show that: $\sum^n_{i=1} (x_i-y_i)^2=\sum^n_{i=1} (y_i-x_i)^2$. This is easily shown by noticing that: $$\sum^n_{i=1} (x_i-y_i)^2-\sum^n_{i=1} (y_i-x_i)^2=0$$
>
>**Q.E.D.**

>[!quote]- Proof: $d(x,y)\leq d(x,z)+d(z,y)$
>This is the only harder to prove property.
>We first write $\sum^n_{i=1} (x_i-y_i)^2$ and rewrite it as $\sum^n_{i=1} (x_i-z_i+z_i-y_i)^2$, which is equal to: $$\sum^n_{i=1} (x_i-z_i)^2+\sum^n_{i=1} (z_i-y_i)^2+2\sum^n_{i=1} (x_i-z_i)(z_i-y_i)$$Then by the [[Cauchy-Schwarz inequality]] we have that: $$\sum^n_{i=1} (x_i-z_i)^2+\sum^n_{i=1} (z_i-y_i)^2+2\sum^n_{i=1} (x_i-z_i)(z_i-y_i)\leq\sum^n_{i=1} (x_i-z_i)^2+\sum^n_{i=1} (z_i-y_i)^2+2\sqrt{\sum^n_{i=1} (x_i-z_i)^2}\sqrt{\sum^n_{i=1} (z_i-y_i)^2}$$ This gives us: $$\sum^n_{i=1} (x_i-y_i)^2\leq \left( \sqrt{\sum^n_{i=1} (x_i-z_i)^2}+\sqrt{\sum^n_{i=1} (z_i-y_i)^2}\right)^2$$ Since the root preserves order for positive reals, this gives us: $$\sqrt{\sum^n_{i=1} (x_i-y_i)^2}\leq  \sqrt{\sum^n_{i=1} (x_i-z_i)^2}+\sqrt{\sum^n_{i=1} (z_i-y_i)^2}$$ Which is the statement we were looking for.
>
>**Q.E.D.**

