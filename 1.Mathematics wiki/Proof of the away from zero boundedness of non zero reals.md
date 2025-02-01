
---

mathLink: auto

---
Date created: 2023-11-15 09:59
Tags: #Type/Proof  

Proved by: [[Cauchy sequences]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  



> [!quote] Proof: Every non zero real has a associated [[Cauchy sequences|cauchy sequence]] which is [[Boundedness away from zero|bounded away from zero]].
>Since we know $x$ is real we have that $x=\text{LIM}_{n\rightarrow \infty}\;b_n$ for some sequence $(b_n)^\infty_{n=1}$. Since $x\neq0$ we know $b_n$ will never be eventually epsilon close to 0. Thus we know there exists at least one epsilon for which $b_n$ is not epsilon close to $0$. Let us fix that specific epsilon. This means that $|b_n-0|>\varepsilon$ for some $n\geq N$ that we denote $n_0$. Now since $b_n$ is also Cauchy we have $|b_n-b_{m}|\leq \frac{\varepsilon}{2}$ for some $m,n\geq N$. From this follows that $|b_{n_0}-b_{n}|\leq \frac{\varepsilon}{2}$ for all $n\geq N$ and we can now see: $|b_{n_0}|>\varepsilon\implies |b_{n_0}-b_{n}+b_{n}|>\varepsilon$. Which according to the triangle inequality gives us $|b_{n_0}-b_{n}+b_{n}|\leq|b_{n_0}-b_{n}|+|b_{n} |\leq \frac{\varepsilon}{2}+|b_n|$. Cleaning up the statement we end up with $\varepsilon<\frac{\varepsilon}{2}+|b_n|$ which clearly implies $|b_n|>\frac{\varepsilon}{2}$. This proves $(b_n)$ is bounded away for $0$ for all $n\geq N$. We now construct the equivalent sequence $a_n$ (which can be easily verified to be equivalent) $a_n:=b_n$ for all $n\geq N$ and $a_n:=\frac{\varepsilon}{2}$. And thus we have $x=\text{LIM}_{n\rightarrow \infty}\;a_n$ where $a_n$ is bounded away from zero and Cauchy.
>
  **Q.E.D.**



