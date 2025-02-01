
---

mathLink: $\forall n\in\mathbb Z\;\forall e\in E:\frac{m_n}{n}\geq e\land \frac{m_n-1}{n}\ngeq e$

---
Date created: 2023-11-24 16:36
Tags: #Type/Theorem #Type/Proof   #Topic/Real_Analysis 

Proved by: [[Induction]], [[Upper bounds]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

We want to prove the following corollary in order to prove [[Existence of least upper bounds]].

> [!quote] Theorem: Special $m$ bound
> Given $E\subseteq \mathbb R$ and [[Integers]] $L<K$ and $n\geq 1$ such that $\frac{K}{n}$ is a [[Upper bounds|upper bound]] but $\frac{L}{n}$ is not. Then there musts exist a $m$ such that $L<m\leq K$ and $\frac{m}{n}$ is an [[Upper bounds|upper bound]] but $\frac{m-1}{n}$ isn't.

The proof goes as follows:

>[!quote] Proof: Special $m$ bound
>For the the sake of contradiction suppose such $m$ does not exist. This implies that whenever $\frac{m}{n}$ is an upper bound then $\frac{m-1}{n}$ is also an upper bound. We now use induction to attain a contradiction. Let $P(j)$ be the statement $L<K-j\leq K$ and $\frac{K-j}{n}$ bounds and $\frac{K-j-1}{n}$. We know the base case $j=1$ is true thanks to our hypothesis for our contradiction. Now suppose $P(j)$ is true, we have to prove that this implies the truth of $P(j+1)$. We have $L<K-(j+1)\leq K$ and we must show that $\frac{K-j-1}{n}$ bounds and $\frac{K-j-2}{n}$ to. By inductive hypothesis the first one is true, and by our hypothesis for our contradiction the second one is true. Now let $j=K-L-1$, since we just proved by induction this must give us a true statement. This either implies that $\frac{L}{n}$ is also a upper bound, a contradiction.
>
>**Q.E.D.**

One can also easily also show that this $m$ is unique by forcing an obvious contradiction when considering the cases $m<m'$ and $m>m'$.

