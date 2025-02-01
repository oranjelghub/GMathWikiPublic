
---

mathLink: auto

---
Date created: 2023-11-13 17:11
Tags: #Type/Proof #Topic/Real_Analysis 

Proved by: [[Bounded rational sequences]], [[Boundedness away from zero]]
References: _Not applicable_
Justifications: [[Positive and negative real numbers]], [[Cauchy sequences]],

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

This is the proof for the [[Positive and negative real numbers|trichotomy of the real numbers]].

> [!quote] Proof: Trichotomy of the real numbers
> First and foremost we prove that at least one of the three statements is true.
> Given a real number $x$we know it is either equal or not equal to zero. If $x$ is equal to zero we already prove that tat least one of the properties of the trichotomy holds, so we may assume that $x$ is non zero. Then we know that $x$ can be written as $\text{LIM}_{n\rightarrow \infty}\;a_n$ and that there is an equivalent Cauchy sequence which is bounded away from zero, which means: $$\exists c>0\in \mathbb Q:\forall n:|b_n|\geq c$$ Now since $a_n$ is Cauchy, so is $b_n$ and thus we know that form some $N$ and for all $j\geq N$ we have: $$|b_j-b_N|<\frac{c}{2}$$ 
> We now split in three different cases depending of the sign of $b_N$ (which is possible in the first place thanks to the trichotomy of the rationals).
> - Suppose $b_N$ is positive. We then notice that $|b_N-b_j|<\frac{c}{2}\implies b_N-b_j<\frac{c}{2}\implies b_j>b_N-\frac{c}{2}$. And since $|b_n|\geq c\implies b_N\geq c$ we have $b_j>b_N-\frac{c}{2}\geq \frac{c}{2}\implies b_j> \frac{c}{2}$ for all $j\geq N$. To finalize this case we must also account for all the entries before $N$, we thus construct the equivalent sequence $c_n$ defined as $b_n$ if $n\geq N$ and otherwise $\frac{c}{2}$ if $n<N$. This sequence is thus positively bounded away from zero and $x$ is positive.
> - Suppose $b_N$ is negative. This case is almost entirely symmetric to the previous one and for the sake of length won't be developed.
> - $b_N$ can not be $0$ as $b_n$ is defined as a bounded away from zero sequence.
> 
 We thus know at least one of the three statements is true. We know show that only 1 can be true at all times. We will prove the three cases by contradiction each.  Suppose $x$ is zero and positive. Then we know that $|b_i|\leq\varepsilon$ for all rational $\varepsilon>0$, but since $x$ is positive we know that there exists a $c>0\in \mathbb Q$ such that it is bounded away positively from zero which means $c<b_i$ but this contradicts if we choose $\varepsilon = \frac{c}{2}$ which we are allowed to do. In a very similar fashion we disprove that $x$ can be zero and negative. We are now only left to prove that $x$ can not be positive and negative. Suppose for the sake of contradiction that $x$ is both. Then there exist $c,d>0$ such that $b_i>c\land a_i<-d$ which we can combine in the statement $a_n-b_n>c+d$ and since $b_n$ is negative for all $n$ and $a_n$ positive we have that $0<a_n-b_n>c+d\implies |a_n-b_n|>c+d$ but this would mean the sequences aren't actually equivalent since there is no $n\geq N$ such that $|a_n-b_n|<\frac{c+d}{2}$ and thus we have a contradiction and the trichotomy is proven. 
 **Q.E.D.**
 
 



