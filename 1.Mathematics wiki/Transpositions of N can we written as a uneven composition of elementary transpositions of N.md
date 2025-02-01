---
mathLink: Transpositions of $\mathbb{N}_{_{\leq n}}$ can we written as a uneven composition of elementary transpositions of $\mathbb{N}_{\leq n}$
Date created: 2024-09-03 12:12
tags:
  - Type/Theorem
  - Topic/Abstract_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Elementary transposing permutations of N]], [[Transposing permutations]], [[Permutations]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Transpositions of $\mathbb{N}_{_{\leq n}}$ can we written as a uneven composition of elementary transpositions of $\mathbb{N}_{\leq n}$
> Let $\tau$ be a transposition and $\sigma$ a permutation of $\mathbb{N}_{\leq n}$ for some $n\in \mathbb{N}$, then there exists some uneven collection of elementary transpositions $(\tau_{e_{i}})_{1\leq i\leq 2k+1}$, with every transposition $\tau_{e_{i}}$ being elementary with respect to ${\huge {\circ}}^{i-1}_{k=1}\tau_{e_{k}} \circ\sigma$, such that $${\huge {\circ}}^{2k+1}_{i=1}\tau_{e_{i}} =\tau $$

>[!quote]- Proof: Transpositions of $\mathbb{N}_{_{\leq n}}$ can we written as a uneven composition of elementary transpositions of $\mathbb{N}_{\leq n}$
>Since $\tau$ is transposition it transposes some $\sigma(i)$ and $\sigma(j)$. Without loss of generality assume that $\sigma(i)<\sigma(j)$. We define for all $1\leq l\leq \sigma(j)-\sigma(i)$ the map $$ \tau_{e_{l}}:{\huge {\circ}}^{l-1}_{i=1}\tau_{e_{i}}(\sigma(k))\mapsto \left\{ \begin{align} &{\huge {\circ}}^{l-1}_{i=1}\tau_{e_{i}}(\sigma(k))& &{\huge {\circ}}^{l-1}_{i=1}\tau_{e_{i}}(\sigma(k))\neq \sigma(i)+l-1,\sigma(i)+l\\&\sigma(i)+l-1&&{\huge {\circ}}^{l-1}_{i=1}\tau_{e_{i}}(\sigma(k))=\sigma(i)+l \\&\sigma(i)+l&&{\huge {\circ}}^{l-1}_{i=1}\tau_{e_{i}}(\sigma(k))=\sigma(i)+l-1\end{align} \right. $$Informally, each of the individual maps just swamps around $\sigma(i)$ and the element that follows. Notice that each $\tau_{e_{l}}$ is a elementary transposition with respect to ${\huge {\circ}}^{l-1}_{i=1}\tau_{e_{i}}\circ\sigma$. Notice now that $$ {\huge {\circ}}^{\sigma(j)-\sigma(i)}_{i=1}\tau_{e_{i}}(\sigma(i))=\sigma(j) $$Whilst $$ {\huge {\circ}}^{\sigma(j)-\sigma(i)}_{i=1}\tau_{e_{i}}(\sigma(j))=\sigma(j)-1 $$Informally, we pushed $\sigma(i)$ forward by continuously swapping it with the next element, until we reached $\sigma(j)$. Similarly, we can do the same with $\sigma(j)-\sigma(i)-1$ maps but in order to switch $\sigma(j)-1$ all the way to $\sigma(i)$'s original position (informally, once again by switching $\sigma(j)-1$ with the previous element $\sigma(j)-\sigma(i)-1$ times). Now composing all these maps gives us $$ {\huge\circ}^{2(\sigma(j)-\sigma(i))-1}_{i=1}\tau_{e_{i}} $$Which we notice, maps $\sigma(i)\to\sigma(j)$, $\sigma(j)\to \sigma(i)$ and for all other $\sigma(k)$ we have $\sigma(k)\to \sigma(k)$. In other words $$  {\huge\circ}^{2(\sigma(j)-\sigma(i))-1}_{i=1}\tau_{e_{i}}=\tau  $$ And since clearly $2(\sigma(j)-\sigma(i))-1$ is uneven we are done. 
>
>**Q.E.D.**
