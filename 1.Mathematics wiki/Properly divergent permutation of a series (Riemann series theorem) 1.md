---
mathLink: auto
Date created: 2024-04-28 13:13
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Arbitrary increase or decrease of a sequence implies proper divergence]], [[Divergence of the series of positive or negative entries of a conditionally convergent series]], [[Induction]], [[Existence of a unique increasing bijection from the natural numbers to one of its inifnite subsets]]
References: _Not applicable_
Justifications: [[Infinite series]], [[Well ordering of the real numbers]], [[Limsup and liminf of sequences]]

Specializations: _Not applicable_
Generalizations: [[Riemann series theorem]]

---

> [!quote] Theorem: Properly divergent permutation of a series (Riemann series theorem)
> Let $\sum^{\infty}_{n=0}a_{n}$ be a conditionally convergent series that is not absolutely convergent, then there exists a permutation $\sigma:\mathbb{N}\to \mathbb{N}$ such that $$\limsup_{ N \to \infty } \sum^{N}_{n=0}a_{\sigma(n)}=+\infty=\liminf_{ N \to \infty }\sum^{N}_{n=0}a_{\sigma(n)} $$ In other words $\sum^{\infty}_{n=0}a_{\sigma(n)}$ properly diverges to $+\infty$. The same theorem holds for $-\infty$.

>[!quote]- Proof: Properly divergent permutation of a series (Riemann series theorem)
>We will prove that this holds for $+\infty$, the other case being symmetric. Let $f^+$ be the unique increasing bijection from $\mathbb{N}$ to $A^+:=\{ n\in \mathbb{N} : a_{n}\geq 0\}$ and $f^-$ the unique bijection from $\mathbb{N}$ to $A^-:=\{ n\in \mathbb{N} :a_{n}<0\}$. Now since the series $\sum^{\infty}_{n=0}a_{f^+(n)}$ grows arbitrarily big, specifically we have that $$ \exists N: \sum^{N-1}_{n=0}a_{f^+(n)}>1-a_{f^-(0)} $$ More generally, we can define the following natural number recursively whilst everything is well defined $$ \left\{ \begin{align} M_{0}&:=\min\left\{  N\in \mathbb{N}: \sum^{N-1}_{n=0}a_{f^+(n)}>1-a_{f^-(0)} \right\} \\ M_{n}&:= \min\left\{  N\in \mathbb{N}: \sum^{N-1}_{n=M_{n-1}} a_{f^+(n)}>1-a_{f^-(n)} \right\}   \end{align} \right.  $$ We can then define the following function $$\sigma: \mathbb{N}\to \mathbb{N}: n\mapsto \left\{ \begin{align} &f^+(n)& \hspace{1cm} &0\leq n<M_{0} \\ &f^+(n-k-1)& \hspace{1cm} &\exists k\in \mathbb{N}: M_{k}+k<n<M_{k+1}+k+1\\ &f^-(k)& \hspace{1cm} &\exists k\in \mathbb{N}: n=M_{k}+k     \end{align} \right. $$ This function is well defined because one could verify at least one of these statements is always true and whenever there exists some $k$ that helps us satisfy condition $2$ or $3$ this $k$ is unique. We now claim that $\sigma$ is indeed a permutation on $\mathbb{N}$. The injectivity follows from splitting the into cases and using the fact that both $f^+$ and $f^-$ are injective. Surjectivity can be proven as follows. Take some $j\in \mathbb{N}$, we either have $j\in A^-$ (in which case $\sigma\left(M_{{f^{-}}^{-1}(j)}+{f^{-}}^{-1}(j)\right)=j$) or $j\in A^+$. In the case of $j\in A^+$ we consider ${f^{-}}^{-1}(j)$. Unless $0\leq {f^{-}}^{-1}(j)<M_{0}$ (in which case $\sigma({f^{-}}^{-1}(j))=j$) we define $l:= \max \{ a\in \mathbb{N}: M_{a}<{f^{-}}^{-1}(j)+1 \}$ and notice that this implies $$ M_{l}+l<{f^{-}}^{-1}(j)+l+1<M_{l+1}+l+1 $$ And thus $\sigma \left( {f^{-}}^{-1}(j)+l+1 \right)=j$ and we have that $\sigma$ is indeed surjective and thus also bijective. One could now proof through induction that $$ \sum^{M_{k}+k}_{n=0}a_{\sigma(n)}>n+1 $$ And thus the partial sums get arbitrarily big, implying the proper divergence to $+\infty$ of $\sum^{\infty}_{n=0}a_{\sigma(n)}$
>
>**Q.E.D.**


