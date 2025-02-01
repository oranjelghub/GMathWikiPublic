
---

mathLink: auto

---
Date created: 2024-03-12 16:54
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Induction]], [[Comparison principle of sequences]], [[Limsup and liminf of sequences (Properties)]]
References: _Not applicable_
Justifications: [[Limsup and liminf of sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Root and ratio inequality of positive real sequences
> Given a sequence of positive real numbers $(c_n)^\infty_{n=m}$ we have $$ \liminf_{ n \to \infty } \frac{c_{n+1}}{c_{n}}\leq \liminf_{ n \to \infty } c_{n}^{1/n}\leq \limsup_{ n \to \infty } c_{n}^{1/n}\leq \limsup_{ n \to \infty } \frac{c_{n+1}}{c_{n}}  $$

>[!quote] Proof: Root and ratio inequality of positive real sequences
>The middle inequality follows from properties concerning superior and inferior limits, we thus prove the right one since the left one is pretty similar. Define $L:=\limsup_{ n \to \infty } \frac{c_{n+1}}{c_{n}}$. If $L$ is positively infinite then the proof is done so we can assume it is finite. We also know it can't be negatively infinite as every term of the sequence is positive, also meaning that $L\geq 0$. Now let $\varepsilon>0$, we know that by properties of superior limits that $$ \exists N: \forall n\geq N; \frac{c_{n+1}}{c_{n}}\leq L+\varepsilon $$ Which implies $$ \exists N: \forall n\geq N; c_{n+1}\leq c_{n}(L+\varepsilon) $$ We can extend this result by induction to obtain $$ \forall n\geq N; c_{n}\leq c_{N}(L+\varepsilon)^{n-N} $$ This on it's turn implies that $$ c_{n}^{1/n}\leq (c_{N}(L+\varepsilon))^{-N/n} (L+\varepsilon)$$ Where $\lim_{ n \to \infty  }(c_{N}(L+\varepsilon))^{-N/n}(L+\varepsilon)=L+\varepsilon$, and thus the comparison principle tells us $$ \limsup_{ n \to \infty } c_{n}^{1/n}\leq L+\varepsilon $$ But since the choice of $\varepsilon$ is arbitrary, to avoid contradiction we must have that $$ \limsup_{ n \to \infty } c_{n}^{1/n}\leq L$$
>
>**Q.E.D.**


