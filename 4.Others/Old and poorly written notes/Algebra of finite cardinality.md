
---

mathLink: auto

---
Date created: 2023-12-21 21:55
Tags: #Type/Unfinished 

%%For Definition/Example of a notion/object%%

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

%%For Proposition/Theorem of a notion/object including both`statement`/`proof` regarding `object`/`notion` it links to %%

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---  



> [!quote] Definition
> Lorem ipsum dolor sit amet



Cardinality arithmetic*

- Let $X$ be a finite set, and let $x$ be an object which is not an element of $X$. Then $X \cup \{x\}$ is finite and $\#(X \cup \{x\}) = \#(X)+1$. 
	Suppose $X$ has cardinality $n$ which means there exists a bijection $f$, then we notice the following bijection: $g:X\cup \{x\}\rightarrow\{1\leq i\leq n+1\}:\alpha\mapsto \left\{\begin{align} f(\alpha) &\hspace{1cm}\alpha\in X\\ n+1&\hspace{1cm}\alpha\in \{x\} \end{align}\right.$. And thus $X\cup\{x\}$ has cardinality $n+1$.
	
	**Q.E.D.**
- Let $X$ and $Y$ be finite sets. Then $X \cup Y$ is finite and $\#(X\cup Y ) ≤ \#(X) + \#(Y )$. If in addition $X$ and $Y$ are disjoint (i.e., $X \cap Y = \emptyset$), then $\#(X \cup Y ) = \#(X) + \#(Y )$.
- Let $X$ be a finite set, and let $Y$ be a subset of $X$. Then $Y$ is finite, and $\#(Y ) ≤ \#(X)$. If in addition $Y \neq X$  (i.e., $Y$ is a proper subset of $X$), then we have $\#(Y ) < \#(X)$. 
- If $X$ is a finite set, and $f : X \rightarrow Y$ is a function, then $f(X)$ is a finite set with $\#(f(X)) ≤ \#(X)$. If in addition $f$ is one-to-one, then $\#(f(X)) = \#(X)$. 
- Let $X$ and $Y$ be finite sets. Then Cartesian product $X \times Y$ is finite and $\#(X \times Y ) = \#(X) * \#(Y )$.
	Suppose $X$ has cardinality $n$ and $Y$ has cardinality $m$. We can then construct the following bijection: $g:\{1\leq i\leq mn\}\rightarrow X\times Y:\alpha\mapsto \left\{\begin{align} (x_\alpha,y_1) &\hspace{1cm}\alpha\leq n\\ (x_{\alpha-n},y_2)&\hspace{1cm}n< \alpha\leq2n\\ \vdots\\ (x_{\alpha-(m-1)n},y_m)&\hspace{1cm} (m-1)n<\alpha\leq mn\end{align}\right.$ And thus $\#(X \times Y ) = \#(X) * \#(Y )$ .
	
	**Q.E.D.**
	Note that we can simply extend this notion to $n$ fold cartesian products by considering the fact that we can define a $n$ tuple in terms of $n$ nested ordered pairs.
- Let $X$ and $Y$ be finite sets. Then the set $Y^ X$ is finite and $\#(Y^X) = \#(Y )^{\#(X)}$ .
	First we note that $\#(Y )^{\#(X)}$ is essentially the cardinality of $Y^{\#X}$ and thus we can prove the statement by defining the following cardinality:
	$\Omega:Y^ X\rightarrow Y^{\#X}:f\mapsto(f(x_1),...,f(x_{\#X}))$.
	
	**Q.E.D.**

