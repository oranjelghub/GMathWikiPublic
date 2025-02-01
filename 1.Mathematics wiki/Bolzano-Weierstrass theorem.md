
---

mathLink: auto

---
Date created: 2024-02-01 11:50
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis  

Proved by: [[Limsup and liminf of sequences (Properties)]], [[Existence of a convergent subsequence of a sequence with real limit points]], [[Comparison principle of sequences]]
References: _Not applicable_
Justifications: [[Bounded real sequences]], [[Sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Bolzano-Weierstrass theorem
> If $(a_n)^\infty_{n=m}$ is a bounded sequence then there exists at least one convergent subsequence of $(a_n)^\infty_{n=m}$.

>[!quote] Proof: Bolzano-Weierstrass theorem
>Let $L^+:=\limsup_{ n \to \infty }a_{n}$. Since $-M\leq a_{n}\leq M$ for some real $M$, because $(a_n)^\infty_{n=m}$ is bounded, we have by the comparison principle that $-M\leq L^+\leq M$, implying $L^+$ is finite. But $L^+$ being finite implies it is a limit point which on it's turn implies that there exists a convergent subsequences that converges to $L^+$. Thus we are done.
>
>**Q.E.D.**



