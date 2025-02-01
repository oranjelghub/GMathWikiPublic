
---

mathLink: auto

---
Date created: 2023-12-20 12:28
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Monotonicity of aN+ and aN-]]
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---  



> [!quote] Theorem: Properties of limits superior and inferior
> Given a sequence $(a_n)^\infty_{n=m}$ and its superior and inferior limit $L^+$, $L^-$. If the sequence converges we say it will be equal to $c$.
> 1. $\forall x>L^+ \exists N\geq m:\forall n\geq N, a_{n}<x$
> 2. $\forall x<L^+ \forall N\geq m \exists n\geq N: a_{n}>x$
> 3. $\inf(a_n)^\infty_{n=m}\leq L^- \leq L^+ \leq \sup(a_n)^\infty_{n=m}$
> 4. $c$ is a limit point of $(a_n)^\infty_{n=m}$ $\implies$ $L^- \leq c\leq L^+$
> 5. $L^+$ is finite $\implies$ $L^+$ is a limit point
> 6. $\lim_{ n \to \infty }a_n=c \iff L^-=c=L^+$

Note that all these properties can easily me modified in order to apply to limit inferior instead. The proofs go as follows:

>[!quote]- $\forall x>L^+ \exists N\geq m:\forall n\geq N, a_{n}<x$
> $L^{+}<x$ gives us $\inf(a_{N}^{+})^\infty_{N=m}<x$, this implies that there exists a $N$ such that $a_{N}^{+}<x$ because otherwise we would have a contradiction to the definition of the infimum. Rewriting this gives us: $\sup(a_N)^\infty_{n=N}<x$, which once again implies $\forall n\geq N, a_{n}<x$
> 
> **Q.E.D.**

>[!quote]- $\forall x<L^+ \forall N\geq m \exists n\geq N: a_{n}>x$
>$x<L^{+}\implies x< \inf(a_{N})^{\infty}_{N=m}\implies x< \inf(a_{N})^{\infty}_{N=m}\leq a_{N}^{+}\implies x<\sup(a_n)^\infty_{n=N}$
> Per definition of least upper bound we must have that there exists a entry in this sequence such that $x<a_{n}$. 
>
>**Q.E.D.**

>[!quote]- $\inf(a_n)^\infty_{n=m}\leq L^- \leq L^+ \leq \sup(a_n)^\infty_{n=m}$
> We first prove $L^+\leq \sup(a_n)^\infty_{n=m}$, from which the symmetric proof of $\inf(a_n)^\infty_{n=m}\leq L^-$ follows. By definition we have $$L^+=\inf(a^+_N)$$ and thus $$\forall N, L^+\leq a^+_N$$ Including $N=m$, thus giving us $$L^+\leq a^+_m=\sup(a_n)^\infty_{n=m}$$ We now only need to show that $L^-\leq L^+$. We will proceed by contradiction. Suppose $L^->L^+$, then by the definition of infimum and supremum we know there must exists a $N$ and $M$ such that $$L^+\leq a_N^+< a_M^-\leq L^-$$ But this contradicts the inequality $a_{\beta}^-\leq a_{\alpha}^+$, thus proving that $L^-\leq L^+$ and that the whole inequality holds. 
> 
> **Q.E.D.**

>[!quote]- $c$ is a limit point of $(a_n)^\infty_{n=m}$ $\implies$ $L^- \leq c\leq L^+$
>    We will proceed by contradiction by assuming that $L^+<c$ to show that $c\leq L^+$.(The proof for $L^-\leq c$ is symmetrical). First of all notice that if $L^+=+\infty$ we have an immediate contradiction, so we may suppose $L^+=-\infty$ or $L^+=r$ with $r\in \mathbb R$. By denseness of the reals there exists a $d$ such that $$L^+<d<c$$ If $L^+=-\infty$ we define $d:=c-1$. By the definition of $L^+$ we also have there exists a $M\geq m$ such that for all $\mu \geq M$ we have $$L^+\leq a_\mu <d <c$$ We also have that $c$ is a limit point meaning that $$\forall \varepsilon>0,  \forall N\geq m, \exists n_0\geq N: |c-a_{n_0}|\leq \varepsilon$$ In particular for $\varepsilon = \frac{c-d}{2}>0$ and $N=M$ we have 
>    $$\begin{align} \exists \mu_0\geq M: |c-a_{\mu_0}|&\leq \varepsilon\\ -\varepsilon\leq c-a_{\mu_0}&\leq \varepsilon\\ -\varepsilon\leq 2\varepsilon+d-a_{\mu_0}&\leq \varepsilon\\ -3\varepsilon\leq d-a_{\mu_0}&\leq -\varepsilon<0\\\end{align}$$ But this implies that $a_{\mu_0}>d$, a contradiction. Thus $c$ can not be greater then $L^+$ and we have that $c\leq L^+$.
>    
>    **Q.E.D.**

>[!quote]- $L^+$ is finite $\implies$ $L^+$ is a limit point
>Once again we only prove the statement for $L^+$ as the proof is symmetrical for $L^-$. Given an arbitrary $\varepsilon >0$ we obviously have $$L^+ - \varepsilon < L^+<L^+ + \varepsilon$$ Implying that for every $K$ we have that there exists some $k\geq K$ for which we have $L^+-\varepsilon < a_k$, fix some arbitrary $K$, combining this with the fact that there exists some $N$ for which all $n\geq N$, $a_n< L^+ + \varepsilon $. Now putting $M=\max(K,N)$ implies that $$\exists m\geq M, |a_m-L^+|\leq \varepsilon$$ But since the choice of $\varepsilon$ and $K$ is totally arbitrary we have that $$\forall \varepsilon \;\forall N \;\exists n\geq N:|a_n - L^+|\leq \varepsilon $$
>
>**Q.E.D.**

>[!quote]- $\lim_{ n \to \infty }a_n=c \iff L^-=c=L^+$
>We split the implication. $(\implies)$ Since the sequence is convergent we know that there is a upper bound $M$ for which $-M\leq a_n \leq M$ for all $n\geq m$. We then have $$a_n\leq M \implies \sup(a_n)^\infty_{n=m} \leq M \implies L^+\leq M$$ We do the same to show that $-M\leq L^-$ giving us $$-M\leq L^-\leq L^+\leq M$$ Proving that both must be finite. But since they are finite they are both limit points of the sequence. But notice that a convergent sequence has only 1 limit point which is always it's limit. Thus we must have $L^-=c=L^+$. $(\Longleftarrow)$ Notice that we have for any arbitrary $\varepsilon > 0$ that $L^- -\varepsilon < c < L^+ + \varepsilon$. We thus know there exists a $K$ and a $M$ such that for all $k\geq K$ and $m\geq M$ $$L^- -\varepsilon < a_k \land a_m< L^+ + \varepsilon$$ If we then put $N:= \max(K,M)$ we get that for all $n\geq N$ $$|a_n-c|\leq \varepsilon$$ Since the choice of $N$ is fully dependant on the choice of epsilon, which was arbitrary, we have that $\lim_{n \to \infty}a_n=c$.
>
>**Q.E.D.**


