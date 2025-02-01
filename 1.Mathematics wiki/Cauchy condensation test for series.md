
---

mathLink: auto

---
Date created: 2024-02-24 19:19
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Induction]]
References: _Not applicable_
Justifications: [[Infinite series]], [[Infinite series (Properties)]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Cauchy condensation for series
> Let $(a_n)^\infty_{n=1}$ be a decreasing sequence of non-negative real numbers. Then the series $\sum^{\infty}_{n=1}a_{n}$ is convergent if and only if the series $\sum^{\infty}_{k=0}2^ka_{2^k}$ is convergent.

>[!quote]- Proof: Cauchy condensation for series
>To prove the statement we will prove a lemma. First we define $S_{N}:=\sum^{N}_{n=1}a_{n}$ and $T_{K}:=\sum^{K}_{k=0}2^{K}a_{2^{K}}$. We will show as lemma that $$ S_{2^{K+1}-1}\leq T_{K}\leq 2S_{2^{K}} $$ We proceed by induction. The base case $K$ is trivial so now suppose for our induction hypothesis that the statement holds for $K$ we want to show that this implies $$ S_{2^{K+2}-1}\leq T_{K+1}\leq 2S_{2^{K+1}}  $$ We notice that $$ S_{2^{K+1}}=S_{2^{K}}+\sum^{2^{K+1}}_{n=2^{K}+1}a_{n}\leq S_{2^{K}}+\sum^{2^{K+1}}_{n=2^{K}+1}a_{2^{K+1}}=S_{2^K}+2^K a_{2^{K+1}} $$ Implying $2S_{2^{K+1}}\geq 2S_{2^K}+2^{K+1}a_{2^{K+1}}$. We also have that $$ S_{2^{K+2}-1}=S_{2^{K+1}-1} +\sum^{2^{K+2}-1}_{n=2^{K+1}}a_{n}\leq S_{2^{K+1}-1} + \sum^{2^{K+2}-1}_{n=2^{K+1}}a_{2^{K+1}}=S_{2^{K+1}-1}+2^{K+1}a_{2^{K+1}}$$ To end, we also have $T_{K+1}=T_{K}+2^{K+1}a_{2^{K+1}}$. Using the three inequalities we mentioned above we have $$  S_{2^{K+1}-1}\leq T_{K}\leq 2S_{2^{K}}\implies S_{2^{K+1}-1}+2^{K+1}a_{2^{K+1}}\leq T_{K}+2^{K+1}a_{2^{K+1}}\leq 2S_{2^{K}}+2^{K+1}a_{2^{K+1}} \implies          S_{2^{K+2}-1}\leq T_{K+1}\leq 2S_{2^{K+1}}  $$ This closes the induction. Now that the lemma is proven, assume $S_{N}$ is convergent and thus bounded, then so is $S_{2^N}$, meaning that by our lemma $T_{N}$ is bounded. And since it is a increasing sequence, it is convergent. Now reversely, suppose $T_{N}$ is convergent and thus bounded. This implies the existence of a bound $M$ such that $S_{2^{N+1}-1}\leq M$ and since we can show by induction that $N+1\leq 2^{N+1}-1$ we have that this also implies $S_{N+1}\leq M$ and hence $S_{N}$ is bounded. This finishes the proof.
>
>**Q.E.D.**


