
---

mathLink: auto

---
Date created: 2023-12-21 00:19
Tags: #Type/Theorem  #Type/Proof #Topic/Topology 

Proved by: [[Continuity (Topological)]]
References: _Not applicable_
Justifications: [[Function composition]], [[Topological spaces]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Continuity is preserved under composition
> Given two continuous functions $f:T_{x}\to T_{y}$ and $g:T_{y}\to T_{z}$ their composition $g\circ f: T_{x}\to T_{z}$ is also continuous.
> 

The proof is very simple and goes as follows:

>[!quote] Proof: Continuity is preserved under composition
>Given $U \subset T_{z}$ with $U$ and open set in the topology of $T_{z}$ we know that it's preimage is open as well. $g^{-1}(U)$ is thus open in $T_{y}$, once again implying (because of continuity) that $f^{-1}(g^{-1}(U))$ is open in $T_{x}$ and notice that $f^{-1}(g^{-1}(U))=(g\circ f)^{-1}(U)$ implying that the inverse image of open sets in $T_{z}$ are open sets in $T_{x}$ under $g\circ f$, implying that the composition is continuous.



