
---

mathLink: auto

---
Date created: 2024-02-01 20:42
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Finite series (Properties)]]
References: _Not applicable_
Justifications: [[Finite series]], [[Series over finite sets]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Finite summations are well-defined
> Let $X$ we a finite set with cardinality $n$ and let $f:X\to \mathbb R$. Then we have that for any bijections from $h$ and $g$ both from $\{ i\in \mathbb N:1\leq i\leq n \}$ to $X$ the following holds $$\sum^{n}_{i=1}f(g(i))=\sum^{n}_{i=1}f(h(i))$$

>[!quote]- Proof: Finite summations are well defined
>We induct on $n$ and start with the base case $n=0$. This gives us $0=0$ by definition of finite series. Now suppose that the following is true $$\sum^{n}_{i=1}f(g(i))=\sum^{n}_{i=1}f(h(i))$$ we want to show that this implies the truth of $$\sum^{n+1}_{i=1}f(g(i))=\sum^{n+1}_{i=1}f(h(i))$$ We do this by putting $x:=g(n+1)$ and write $$\sum^{n+1}_{i=1}f(g(i))=\sum^{n}_{i=1}f(g(i))+f(x)$$ Since $h$ is a bijection we know there exists some $j$ such that $h(j)=x$. We can thus also write $$\begin{align} \sum^{n+1}_{i=1}f(h(i))&=\left( \sum^{j-1}_{i=1} f(h(i)) \right)+f(h(j)) \left( \sum^{n+1}_{i=j+1} f(h(i)) \right) \\ &= \left( \sum^{j-1}_{i=1} f(h(i)) \right)+f(x) \left( \sum^{n}_{i=j} f(h(i+1)) \right) \end{align}$$ Now defining the function $\tilde{h}:\{ i\in \mathbb N:1\leq i\leq n \}\to X:i\mapsto \left\{\begin{align}  &h(i)\hspace{1cm} i<j \\ &h(i+1)\hspace{1cm}i\geq j  \end{align}  \right.$ Allow us to rewrite the whole as $$\sum^{n+1}_{i=1}f(h(i))=\sum^{n}_{i=1}f(\tilde{h}(i))+f(x)$$ To finish the proof it would now only suffice to show that $\sum^{n}_{i=1}f(g(i))=\sum^{n}_{i=1}f(\tilde{h}(i))$ We we restict the range of $g$ by removing the $n+1$ from the domain we end up with a bijection if the range is $X\backslash\{ x \}$, but notice that by definition of $h$ and $\tilde{h}$ we have that $\tilde{h}$ is as well a bijection with the same domain and range as the restricted $g$. Thus the truth of $\sum^{n}_{i=1}f(g(i))=\sum^{n}_{i=1}f(\tilde{h}(i))$ directly follows from the inductive hypothesis that $\sum^{n}_{i=1}f(g(i))=\sum^{n}_{i=1}f(h(i))$ Thus our proof is complete.
>
>**Q.E.D.**
