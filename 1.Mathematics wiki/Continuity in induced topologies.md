
---

mathLink: auto

---
Date created: 2024-01-15 11:50
Tags: #Type/Theorem  #Type/Proof #Topic/Topology 

Proved by: [[Continuity (Topological)]]
References: _Not applicable_
Justifications: [[Subspace or induced topological spaces]]

Specializations: _Not applicable_
Generalizations: [[Continuity (Topological)]]

---  

> [!quote] Theorem: Continuity in the subspace topology
>Given a continuous function $f:S\to T$ where $S$ and $T$ are topological spaces, every restriction $f|_Q:Q \to R$ where $(Q,\Theta_S)$ and $(R,\Theta_T)$ is continuous.

![[diagram-20231226 (1).svg#invert_B]]

>[!quote]- Proof: Continuity in the subspace topology
>  Let $P\in \Theta_T$, one can easily show that $f^{-1}|_Q(P)=Q\cap f^{-1}(P)$ and since $P$ is open and we are in the subspace topology we have that there exists a open set $U\subset T$ such that $P=R\cap U$. This gives us $$f^{-1}|_Q(P)=Q\cap f^{-1}(R\cap U)=Q\cap f^{-1}(R)\cap f^{-1}(U)$$ And since $Q\subset f^{-1}(R)$ (Otherwise we would have a not well defined function, $f|_Q$ being well defined was an obvious implicit assumption) we have $$f^{-1}|_Q(P)=Q\cap f^{-1}(U)$$ And since $f$ is continuous we know that $f^{-1}(U)$ is open. But since we are in the subspace topology $Q\cap f^{-1}(U)$ is a open set and we have that the restricted preimage of a open set in the restricted range is open.

