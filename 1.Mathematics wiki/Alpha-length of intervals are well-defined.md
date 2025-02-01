---
mathLink: $\alpha$-length of intervals are well-defined
Date created: 2024-08-06 14:05
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Monotone bounded sequences converge]]
References: _Not applicable_
Justifications: [[Subsequences]], [[Sequential definition of limit of a function at a point]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Alpha-length of intervals are well-defined
> Let $X$ be a closed interval and let $\alpha:X\to \mathbb{R}$ be a monotone increasing function. Then for any $a\in X$, the following limits exist $$ \begin{align} \lim_{ x \to a^{-}:x\in X  } \alpha(x) \\ \lim_{ x \to a^{+}:x\in X }  \alpha(x) \end{align} $$

>[!quote] Proof: Alpha-length of intervals are well-defined
>We only show the first limit exists, the proof for the other one is similar. We proceed by the sequential definition for limits. Let $(b_n)^\infty_{n=1}$ be a sequence of elements of $X\cap(a,\infty)$ that converges to $a$. We define $$ \sigma :\mathbb{N}^{*}\to \mathbb{N}^{*}: n \mapsto \min\left\{ k\in \mathbb{N}: \left| a-b_{k} \right| \leq \frac{1}{n}\land \forall j<n, \; \sigma(j)\neq k \right\}  $$Clearly this is a well defined function since the set is non-empty and more specifically non-finite. Notice that $\sigma$ is a strictly increasing function and thus we get the decreasing subsequence $(b_{\sigma(n)})^\infty_{n=1}$with $\lim_{ n \to \infty }b_{\sigma(n)}=a$. Since $(b_{\sigma(n)})^\infty_{n=1}$ is decreasing we know that $(\alpha(b_{\sigma(n)}))^\infty_{n=1}$ is also decreasing but also that $(\alpha(b_{\sigma(n)}))^\infty_{n=1}$ is bounded below by $\alpha(a)$. Thus $(\alpha(b_{\sigma(n)}))^\infty_{n=1}$ is also convergent and converges to $\inf_{n\in \mathbb{N}^{*}} \alpha(b_{\sigma(n)})$. Since the choice of $(b_{n})^{\infty}_{n=1}$ is arbitrary we know by the sequential definition that $\lim_{ x \to a^{+}:x\in X}\alpha(x)$ exists.
>
>**Q.E.D.**