---
mathLink: continuous $\alpha$-length is finitely additive
Date created: 2024-08-04 17:39
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Induction]], [[Properties of series over infinite sets]]
References: _Not applicable_
Justifications: [[Alpha-length of intervals]]

Specializations: [[Length of bounded intervals is finitely additive]]
Generalizations: _Not applicable_

---

> [!quote] Theorem: $\alpha$-length is finitely additive
> Let $X$ be a closed interval and let $\alpha:X\to \mathbb{R}$ be a continuous $\alpha$-length on $X$, if $I$ is some bounded interval and $P$ is some partition of $I$ then $$ \alpha[I]=\sum^{}_{J\in P}\alpha[J] $$

>[!quote]- Proof: $\alpha$-length is finitely additive
>The claim follows trivially if $I$ is empty or a singleton, so assume $I$ has endpoints $a<b$. We will proceed by induction on the cardinality of $P$. If $\left| P \right|=0$ then $I$ must be empty and the claim follows. Now we assume for our induction hypothesis that for a partition $P_{n}$ of $I$ such that $\left| P_{n} \right|=n$ we have $$ \alpha[I]=\sum^{}_{J\in P_{n}}\alpha[J] $$We now want to show that this holds for some partition $P_{n+1}$ where $\left| P_{n+1} \right|=n+1$. Since $P_{n+1}$ is a partition of $I$ we must have that some interval in $P_{n+1}$ has right-endpoint $b$ (can be proven by contradiction) and left-endpoint $c$. Denote that interval $K$ and assume that(we avoid splitting the proof into a deep imbrication of sub-cases) $K=[c,b]$ , and notice that this implies that $P_{n+1}\backslash \{ K \}$ is also an interval, and we get that  $$ \begin{align} &\alpha[I]&=& \left( \lim_{ x \to a^{+}:x\in X }  \alpha(x) -\lim_{ x \to a^{-}:x\in X  } \alpha(x) \right)  + \left( \lim_{ x \to b^{-}:x\in X } \alpha(x)-\lim_{ x \to a^{+}:x\in X } \alpha(x)  \right) + \left( \lim_{ x \to b^{+}:x\in X }  \alpha(x) -\lim_{ x \to b^{-}:x\in X  } \alpha(x) \right)\\ &&=& \lim_{ x \to b^{+}:x\in X }   \alpha(x)-\lim_{ x \to a^{-}:x\in X } \alpha(x) \\ &\alpha[P_{n+1}\backslash \{ K \}]&=& \left( \lim_{ x \to a^{+}:x\in X }  \alpha(x) -\lim_{ x \to a^{-}:x\in X  } \alpha(x) \right)  + \left( \lim_{ x \to c^{-}:x\in X } \alpha(x)-\lim_{ x \to a^{+}:x\in X } \alpha(x)  \right) + \left( \lim_{ x \to c^{+}:x\in X }  \alpha(x) -\lim_{ x \to c^{-}:x\in X  } \alpha(x) \right) \\ &&=& \lim_{ x \to c^{-}:x\in X }  \alpha(x)-\lim_{ x \to a^{-}:x\in X } \alpha(x) \\ &\alpha[K]&=& \left( \lim_{ x \to c^{+}:x\in X }\alpha(x)-\lim_{ x \to c^{-}:x\in X }\alpha(x)   \right)+\left( \lim_{ x \to b^{-}:x\in X }\alpha(x)-\lim_{ x \to c^{+}:x\in X }\alpha(x)   \right) +\left( \lim_{ x \to b^{+}:x\in X }  \alpha(x) -\lim_{ x \to b^{-}:x\in X  } \alpha(x) \right) \\ &&=& \lim_{ x \to b^{+}:x\in X } \alpha(x)-\lim_{ x \to c^{-}:x\in X }\alpha(x)       \end{align} $$Meaning that $$ \alpha[I]= \alpha[P_{n+1}\backslash K]+\alpha[K] $$But $\left| P_{n+1}\backslash \{ K \} \right|=n$ thus $$ \alpha[I]=\sum^{}_{J\in P_{n+1}\backslash \{ K \} }\alpha[J] +\sum^{}_{J\in \{ K \}}\alpha[J]$$And by the properties of summations over finite sets we conclude $$ \alpha[I]=\sum^{}_{J\in P_{n+1}}\alpha[J] $$Which closes the induction.
>
>**Q.E.D.**
