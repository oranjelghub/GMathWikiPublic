
---

mathLink: auto

---
Date created: 2023-11-24 22:41
Tags: #Type/Unfinished  #Type/Proof  

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---  



> [!quote] Proof:
> Lorem ipsum dolor sit amet



## Proofs

- (1)
	First we note that domains and ranges do match up, we then check if for all $a$'s in the domain we get the same $b$'s in the range. $f(a)=f\circ \imath_{A\rightarrow A}(a) = \imath_{B\rightarrow B}\circ f(a)$ gets us $b=f(a) = \imath_{B\rightarrow B}(b)$ which is also equal to $b=b=b$ and thus these 3 functions are equal.
	
	**Q.E.D.**
- (2)
	In order for sets to be equal we must show that their images match up for the same entries. First we check that domain and range matches up, which is the case. We know check if for arbitrary $x$'s the functions have the same image $\imath_{Y\rightarrow Z} (\imath_{X\rightarrow Y}(x))=\imath_{X\rightarrow Z}(x)$ which, knowing the particular subset relations between the sets, gives us $\imath_{Y\rightarrow Z} (x)=x$ and once again gives us $x=x$, meaning that indeed the two functions are equal.
	
	**Q.E.D.**
- (3)
	In order to show that the functions are equal, we once again just fill in arbitrary $x$'s and see that they all equal, knowing of course that $f$ and it's inverse are bijective.
- (4)
	We have to prove the existence of $h$ and it's uniqueness. We first assert that the following function satisfies $h$'s properties: $h:X\cup Y \rightarrow Z:\alpha_{X\cup Y}\mapsto\left\{\begin{align} f(\alpha_{X\cup Y}) \hspace{1cm} &: \alpha_{X\cup Y} \in X \\ g(\alpha_{X\cup Y}) \hspace{1cm} &: \alpha_{X\cup Y} \in Y \\ \end{align}\right.$ . We now check it does satisfy function equality for it's properties.
	First we have $h\circ \imath_{X\rightarrow X\cup Y}=f$ for arbitrary $\alpha_X \in X$ we get $h( \imath_{X\rightarrow X\cup Y}(\alpha_X))=f(\alpha_X)$ which is equal to $h(\alpha_X)=f(\alpha_X)$ and which according to $h$'s definition is $f(\alpha_X)=f(\alpha_X)$. The exact same can be done for $g$, thus we know that $h$ exists but now we have to prove it's uniqueness. Suppose there was another function $h'$ that satisfied the same properties, then we have that $h\circ \imath_{X\rightarrow X\cup Y}=f=h'\circ \imath_{X\rightarrow X\cup Y}$  for $f$ and for $g$ we have $h\circ \imath_{Y\rightarrow X\cup Y}=g=h'\circ \imath_{Y\rightarrow X\cup Y}$. We then see that $h\circ \imath_{X\rightarrow X\cup Y}=h'\circ \imath_{X\rightarrow X\cup Y}$ for $f$. Now fix $\alpha_X\in X$ which obviously $\alpha_X=\alpha_X$. We now evaluate both functions in that point and see that $h(\alpha_X)=h'(\alpha_X)$ and thus the functions are equal over all $\alpha$'s is $X$. In order to see that they are equal of the full domain we have to conduct the same check for $g$. So $h\circ \imath_{Y\rightarrow X\cup Y}=g=h'\circ \imath_{Y\rightarrow X\cup Y}\implies h\circ \imath_{Y\rightarrow X\cup Y}=h'\circ \imath_{Y\rightarrow X\cup Y}$ , evaluated at $\alpha_Y$ (which is in $Y$) gives us $h(\alpha_Y)=h'(\alpha_Y)$. And thus the functions are also equal over $Y$ meaning that we proved that the functions are equal over their full domain and proving the uniqueness of $h$.
	
	**Q.E.D.**

