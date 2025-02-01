
## *Exponentiation in $\mathbb{N}$*

We first recursively define the operation with the following two operations:
$$0^0:=1 \hspace{1cm} (1)$$
$$m^{S(n)}:=m^n\times m \hspace{1cm} (2)$$


## *Exponentiation to a natural number*

We recursively define exponentiation for [[Natural numbers|natural number]] exponents. We define:
$$\begin{align} 
x^0&:=1\\
0^0&:=1\\
x^{S(n)}&:=x^n \times x
\end{align}$$

#### *Properties*

- $x^nx^m=x^{n+m}$, $(x^n)^m=x^{mn}$, $(xy)^n=x^ny^n$
- Suppose $n>0$, then $x^n=0 \iff x=0$
- $x\geq y\geq 0\implies x^n\geq y^n \geq 0$ and if $n>0$ then $x> y\geq 0\implies x^n> y^n \geq 0$
- $|x|^n=|x^n|$


## *Exponentiation to a [[Integers|integer]] number*

We can obviously extend this notion of exponentiation to the integers by giving this additional definition:
$$x^{-n}:=1/x^n$$


#### *Properties*

- $x^nx^m=x^{n+m}$, $(x^n)^m=x^{mn}$, $(xy)^n=x^ny^n$
- $x\geq y> 0\implies x^n\geq y^n > 0$ if $n$ is positive and $x\geq y>0 \implies 0<x^n\leq y^n$
- If $x,y>0$ and $n \neq 0$ and $x^n=y^n \implies x=y$
- $|x|^n=|x^n|$

#completed 
