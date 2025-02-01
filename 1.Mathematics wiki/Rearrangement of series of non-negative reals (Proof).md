
---

mathLink: auto

---
Date created: 2024-02-26 16:25
Tags: #Type/Proof  #Topic/Real_Analysis 

Proved by: [[Series over finite sets (Properties)]]
References: _Not applicable_
Justifications: [[Rearrangement of series of non-negative reals]], [[Infinite series]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Proof: Rearrangement of series of non-negative reals
> We define $S_{N}:=\sum^{N}_{n=0}a_{n}$ and $T_{M}:=\sum^{M}_{m=0}a_{f(m)}$, we know that both sequences are increasing. Now write $L_{S}:=\sup(S_{N})^\infty_{N=0}$ and $L_{T}:=\sup(T_{M})^{\infty}_{M=0}$. Since we know $S_{N}$ is convergent we know that $L_{S}=\sum^{\infty}_{n=0}a_{n}$, it would thus suffice to show that $L_{S}=L_{T}$ as it would imply the finiteness of $L_{T}$ and thus give us a valid bound for the sequence $T_{M}$ and also a limit. Now fix $M$ and let $Y:=[\![0,M]\!]_{\mathbb{N}}$. And since $f$ is a bijection with the restriction $f:Y\to f(Y)$ we get $$ T_{M}=\sum^{M}_{m=0}a_{f(m)}=\sum^{}_{m\in Y}a_{f(m)}=\sum^{}_{n\in f(Y)}a_{n} $$ Since $(f(m))^{\infty}_{m=0}$ is a finite sequence it is bounded by some $N$ and thus $f(Y)\subseteq [\![0,N]\!]_{\mathbb{N}}$, combining this with the assumption that all $a_{n}$ are non-negative we get $$ T_{M}=\sum^{}_{n\in f(Y)}a_{n}\leq \sum^{}_{n\in [\![0,N]\!]_{\mathbb{N}}} a_{n}=S_{N}$$ Which means $$ T_{M}\leq S_{N}\implies T_{M} \leq L_{S} \implies L_{T}\leq L_{S}$$ We can replicate this argument by starting from $S_N$ this time and considering $f^{-1}$ to obtain $L_{S}\leq L_{T}$ and thus we must have $L_{S}=L_{T}$
> 
> **Q.E.D.**



