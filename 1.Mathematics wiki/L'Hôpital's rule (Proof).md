---
mathLink: auto
Date created: 2024-07-12 23:11
tags:
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---  

Proved by: [[Newton's approximation]], [[Limit laws for real valued functions]], [[Rolle's theorem]], [[Sequential definition of limit of a function at a point]], [[Axiom of choice]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Differentiation of real valued functions]], [[L'Hôpital's rule]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote]- Proof: L'Hôpital's rule (I)
> We first argue the existence of some $\delta$ such that $g$ is non-zero on $\left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \}$. Since $g$ is differentiable at $x_{0}$ with derivative $g'(x_{0})\neq 0$ we have by Newton's approximation that $$ \forall \varepsilon \exists \delta: \forall x\in X\backslash\{ x_{0} \},\; \left| x-x_{0} \right|\leq \delta \implies \left| g(x)-g'(x_{0})(x-x_{0}) \right| \leq \varepsilon \left| x-x_{0} \right|    $$Now fix some $\varepsilon<g'(x_{0})$, notice that by the triangle inequality $$ \left| g'(x_{0})(x-x_{0}) \right| -\left| g(x) \right| \leq \left| g(x)-g'(x_{0})(x-x_{0}) \right|  $$Thus $$ \left| x-x_{0} \right| \left( \left| g'(x_{0}) \right| -\varepsilon \right) \leq \left| g(x) \right|  $$But notice that $\left| x-x_{0} \right| \left( \left| g'(x_{0}) \right| -\varepsilon \right)>0$, thus there exists some $\delta$ such that $g$ is non-zero on $\left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \}$. This being said, we can say that $$ \frac{f'(x_{0})}{g'(x_{0})}=\frac{\lim_{ x \to x_0:x\in \left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \} }  \frac{f(x)-f(x_{0})}{x-x_{0}}}{\lim_{ x \to x_0:x\in \left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \} } \frac{g(x)-g(x_{0})}{x-x_{0}} }$$And since both limits exist and $\frac{g(x)-g(x_{0})}{x-x_{0}}$ is non-zero on $\left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \}$, we may combine the limits and obtain $$ \lim_{ x \to x_0:x\in \left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \} } \frac{\frac{f(x)-f(x_{0})}{x-x_{0}}}{\frac{g(x)-g(x_{0})}{x-x_{0}}}= \lim_{ x \to x_0:x\in \left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \} } \frac{f(x)}{g(x)}=\frac{f'(x_{0})}{g'(x_{0})}$$As desired.
> 
> **Q.E.D.**

>[!quote]- Proof: L'Hôpital's rule (II)
>First we show that indeed $$ \forall x\in [a,b]\backslash\{ c \},\; g(x)\neq 0 $$We proceed by contradiction. Assume this isn't the case, then there exists some $z\in[a,b]\backslash\{ c \}$ such that $g(z)=0$. Assume WLOG that $c<z$, since $g$ is continuous on $[c,z]$ and differentiable on $(c,z)$, we may apply Rolle's theorem to argue the existence of some $\hat{z}$ such that $g'(\hat{z})=0$. But this directly contradicts the fact that $g'$ is non-zero on $[a,b]\backslash \{ c \}$, thus the assumption that such a $z$ must exist must be wrong and we have that $g(x)\neq 0$ for all $x$ in $[a,b]\backslash\{ c \}$. We now want to show that $$ \lim_{ x \to c:x\in [a,b]\backslash \{ c \} } \frac{f(x)}{g(x)}=L $$To do this we will consider the left and right limit. We want $$\lim_{ x \to c:x\in (c,b] } \frac{f(x)}{g(x)}=L=\lim_{ x \to c:x\in [a,c) } \frac{f(x)}{g(x)}$$We shall only prove the right limit is equal to $L$, as the proof for the left limit is symmetric. By the sequential definition it suffices to show that for any sequence $x_{n}$ that converges to $c$ and consists of elements of $(c,b]$, the sequence satisfies $$ \lim_{ n \to \infty } \frac{f(x_{n})}{g(x_{n})}=L $$To show this, fix such a sequence and consider the function $$ h_{n}:[c,x_{n}]\to \mathbb{R}: x\mapsto f(x)g(x_{n})-g(x)f(x_{n}) $$Observe that $h_{n}$ is continuous on $[c,x_{n}]$ and is differentiable on $(c,x_{n})$ with derivative $h'_{n}=f'(x)g(x_{n})-g'(x)f(x_{n})$. We also have that $h_{n}(c)=0=h_{n}(x_{n})$, thus we may apply Rolle's theorem to argue that the set $E_{n}$, defined as $$ E_{n}:=  \left\{ y\in (c,x_{n}): h_{n}'(y)=0 \right\}  $$Is non-empty for every $n$. Thus we may define some choice function $c_{n}$ on $\bigcup_{n\in \mathbb{N}}E_{n}$. Now notice that since $0=f'(c_{n})g(x_{n})-g'(c_{n})f(x_{n})$ we have $$ \frac{f(x_{n})}{g(x_{n})}=\frac{f'(c_{n})}{g'(c_{n})} $$But since $c\leq c_{n}\leq x_{n}$ we know that $c_{n}\to c$ as $n\to \infty$. Thus $\frac{f'(c_{n})}{g'(c_{n})}\to L$ as $n\to \infty$, directly implying that $\frac{f(x_{n})}{g(x_{n})}\to L$ as $n\to \infty$. Meaning that indeed $$ \lim_{ x \to c:x\in (c,b] } \frac{f(x)}{g(x)}=L $$And generally after symmetrically proving the same for the lefty limit $$  \lim_{ x \to c:x\in [a,b]\backslash \{ c \} } \frac{f(x)}{g(x)}=L  $$
>
>**Q.E.D.**

