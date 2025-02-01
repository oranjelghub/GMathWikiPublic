
---

mathLink: auto

---
Date created: 2023-11-20 10:21
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Special m bound of a subset of R]], [[Ordering of the real numbers]], [[Least upper bounds]], [[Cauchy sequences]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

This is a really important theorem with a really lengthy proof.

> [!quote] Theorem: Existence of least upper bounds
> Given $E\subseteq \mathbb R$ and $E$ non-empty, if $E$ has an [[Upper bounds|upper bound]] then it must also have a [[Least upper bounds|least upper bound]].

We now attack the proof.

>[!quote]- Proof: Existence of least upper bounds
>Let $E\subset \mathbb R$ with upper bound $M$. We know the least upper bound is unique. Since $E$ is non-empty we can choose $x_0\in E$. Now let $n\geq 1$ be an integer. By the Archimedean property we have that there exist integers $L$ and $K$ such that $\frac{K}{n}\geq M$ and $\frac{L}{n}<x_0$. We thus see that $L\leq K$. We can now now find a $m_n$ such that $L<m_n\leq K$ where $\frac{m_n}{n}$ is an upper bound and $\frac{m_n-1}{n}$ isn't. Furthermore we know this $m_n$ is unique. Now let $N\geq 1$ be an integer and let $n,n'\geq N$. Since $\frac{m_n}{n}$ is an upper bound but $\frac{m_{n'}-1}{n'}$ isn't we have that $\frac{m_n}{n}>\frac{m_{n'}-1}{n'}$. After some algebra we have: $$\frac{m_n}{n}-\frac{m_{n'}}{n'}>\frac{-1}{n'}\geq \frac{-1}{N}$$
>Similarly we have that $\frac{m_{n'}}{n'}$ is a bound but $\frac{m_{n}-1}{n}$ isn't and so we also conclude: $$\frac{m_n}{n}-\frac{m_{n'}}{n'}<\frac{1}{n'}\leq \frac{1}{N}$$
>This altogether implies: $$\left|\frac{m_n}{n}-\frac{m_{n'}}{n'}\right|\leq \frac{1}{N}$$ For all $N$ and $n,n'\geq N$. We now notice that this proves that the sequence $(\frac{m_n}{n})^\infty_{n=1}$ is Cauchy because we have thanks to the Archimedean property that for all positive rational $\varepsilon$ that there is an $N$ such that $\frac{1}{N}<\varepsilon$. Since all the entries of the sequence are rational we can define the real number $S:=\text{LIM}_{n\rightarrow\infty}\;\frac{m_n}{n}$ and we also notice that substracting $1/n$ to the sequence doesn't change anything as this tends to zero. $$S:=\text{LIM}_{n\rightarrow\infty}\;\frac{m_n-1}{n}$$. We now want to show that $S$ is indeed the least upper bound of $E$. First we show it is a bound. Suppose $x\in E$, we have that $x\leq \frac{m_n}{n}$ for all $n$ and this implies $x\leq S$ (A modified version of a property of the real ordering). Now suppose there is another upper bound $y$, we then have that $\frac{m_n-1}{n}\leq y$ as the other term is not a bound. Once again by the modified property of real ordering we have that $S\leq y$. This altogether proves $S$ is the least upper bound of $E$. The least upper bound thus always exists in $\mathbb R$.
>
> **Q.E.D.**



