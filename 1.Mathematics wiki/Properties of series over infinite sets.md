
---

mathLink: auto

---
Date created: 2024-03-31 10:42
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Infinite series (Properties)]], [[Finite series (Properties)]], [[Series over finite sets (Properties)]]
References: _Not applicable_
Justifications: [[Series on uncountable sets]], [[Axiom of choice]], [[Series on countable sets]]

Specializations: [[Infinite series (Properties)]], [[Finite series (Properties)]]
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Absolutely convergent series laws
> Let $X$ be a arbitrary set, and let $f:X\to \mathbb{R}$ and $g:X\to \mathbb{R}$ be functions such that $\sum^{}_{x\in X}f(x)$ and $\sum^{}_{x\in X}g(x)$ are both absolutely convergent.
> 1. Then the series $\sum^{}_{x\in X}f(x)+g(x)$ is also absolutely convergent, and $$ \sum^{}_{x\in X}f(x)+g(x)=\sum^{}_{x\in X}f(x)+ \sum^{}_{x\in X}+g(x) $$
> 2. If $c$ is a real number, then $\sum^{}_{x\in X}cf(x)$ is absolutely convergent, and $$ \sum^{}_{x\in X}cf(x)=c\sum^{}_{x\in X}f(x) $$
> 3. If $X=X_{1}\cup X_{2}$ for some disjoint sets $X_1$ and $X_{2}$, then $\sum^{}_{x\in X_{1}}f(x)$ and $\sum^{}_{x\in X_{2}}f(x)$ are absolutely convergent, and $$ \sum^{}_{x\in X_{1}\cup X_{2}}f(x)=\sum^{}_{x\in X_{1}}f(x)+\sum^{}_{x\in X_{2}}f(x) $$
> 4. Conversely, if $h:X\to \mathbb{R}$ is such that $\sum^{}_{x\in X_{1}}h(x)$ and $\sum^{}_{x\in X_{2}}h(x)$ are absolutely convergent, then $\sum^{}_{x\in X_{1}\cup X_{2}}h(x)$ is also absolutely convergent, and $$ \sum^{}_{x\in X_{1}\cup X_{2}}h(x)=\sum^{}_{x\in X_{1}}h(x)+\sum^{}_{x\in X_{2}}h(x) $$
> 5. If $Y$ is another set, and $\varphi:Y\to X$ is a bijection, then $\sum^{}_{y\in Y}f(\varphi(y))$ is also absolutely convergent, and $$ \sum^{}_{y\in Y}f(\varphi(y))=\sum^{}_{x\in X}f(x) $$

Notice that these results require the axiom of choice whenever $X$ is uncountable.  The first two statements are straight forward to proof (with maybe a slight exception to $1$, where it is easier to simply prove $3$ first), make use of the definitions of absolute convergence for infinite sets and use the know properties for the finite partial sums. We do prove the 3 last ones.

>[!quote]- Proof: Absolutely convergent series laws (3,4,5)
>We will assume $X$ is always countable, since the finite case is trivial and the uncountable case can be reduced to a countable one using choice. We define $$ M(X,f):=\sup\left\{ \sum^{}_{x\in A}\left| f(x) \right|:A\subseteq X, A\;\text{finite}  \right\} $$
>**3)** It is obvious that for all finite $A_{1}\subseteq X_{1}$ and $A_{2}\subseteq X_{2}$, $\sum^{}_{x\in A_{1}}\left| f(x) \right|\leq M(X,f)$ and $\sum^{}_{x\in A_{2}}\left| f(x) \right|\leq M(X,f)$ and thus both sums are absolutely convergent. Now we want to show the equality. First pick some arbitrary finite set $A_{1}\cup A_{2}\subset X_{1}\cup X_{2}$ and define the following bijections: $h_{1}:\mathbb{N}_{0}\to A_{1}$, $h_{2}:\mathbb{N}_{0}\to A_{2}$. We now construct $$ h_{(1,2)}:\mathbb{N}_{0}\to A_{1}\cup A_{2}:n\mapsto \left\{ \begin{align} &h_{1}\left( \frac{n}{2} \right)& &\hspace{1cm}n\text{ is even}\\ &h_{2}\left(\frac{n-1}{2}-1\right)& &\hspace{1cm} n\text{ is odd} \end{align} \right.  $$ One can easily check this forms a bijection. Now we can easily prove by induction that $$ \sum^{2N}_{n=1}f(h_{(1,2)}(n))=\sum^{N}_{n=1}f(h_{1}(n))+f(h_{2}(n)) $$ Now taking the limit as $N$ approaches infinity on both sides and applying the definitions obtains us the wanted equality $$ \sum^{}_{x\in X_{1}\cup X_{2}}f(x)=\sum^{}_{x\in X_{1}}f(x)+\sum^{}_{x\in X_{2}}f(x) $$
>**4)** It is pretty obvious that for any finite set $A_{1}\cup A_{2}\subset X_{1}\cup X_{2}$ that $\sum^{}_{x\in A_{1}\cup A_{2}}|f(x)|\leq M(X_{1},f)+M(X_{2},f)$, and thus the sum $\sum^{}_{x\in X_{1}\cup X_{2}}f(x)$ is absolutely convergent. Using the same argument of $3$ we can prove the equality once again.
>**5)** For every finite $A\subseteq X$ we have that $\sum^{}_{x\in A}f(x)\leq M(X,f)$, but since $A$ is finite we can apply substitution to it and thus $\sum^{}_{y\in \varphi^{-1}(A)}f(\varphi(y))\leq M(X,f)$ and thus $\sum^{}_{y\in Y}f(\varphi(y))$ is absolutely convergent. To prove the equality notice that for any bijection $h:\mathbb{N}\to Y$, $\varphi\circ h$ is also a bijection and thus $$ \sum^{}_{x\in X}f(x)=\sum^{\infty}_{n=0}f(\varphi(h(n)))=\sum^{}_{y\in Y}f(\varphi(y)) $$ 
>
>**Q.E.D.**


