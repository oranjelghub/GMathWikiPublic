
Power [[Sets|sets]] are a specific kind of [[Sets|set]] that we construct axiomatically.

We can take two approaches for this. The classic way is using the following axiom:

$$\forall X:\exists\mathcal{P}(X):\forall Z:Z\in \mathcal{P}(X)\iff \forall w(w\in Z \implies w\in X)$$
This is usually what is classically used in Zermelo-Fraenkel set theory. Essentially this axiom states that there exists a power set which is the set containing all the subsets of a specific set $X$. This notion can also be defined with another axiom proposed by Terence Tao in Analysis I.
$$\forall X:\forall Y: \exists Y^X:f\in Y^X \iff f  \;\text{is a function} \;X\rightarrow Y$$
Using this axiom we can construct the following set (explanation lower down in note): 
$$\forall X:\exists \mathcal{P}(X):\mathcal{P}(X)=\{Y:Y\in X\}$$
All sets constructed by the axiom in terms of functions also have a cardinality off $\text{card}(Y)^{\text{card}(X)}$ whilst the power sets have a cardinality of $2^{\text{card}(X)}$ .


## *Constructing power sets with Terence Tao's axiom*

We can construct the following set using the power set axiom and the axiom of replacement: 
$$\left\{ Y:Y\subseteq X\right\}=\left\{ Y:P(f,Y)\land f\in \{0,1\}^X\right\}$$
With $P$ being the property:
$$P(f,Y):f^{-1}(\{1\})=Y$$

To prove this we first notice that for every $f$ the property $P$ is true for a unique $Y$, since for any set $U$ it's inverse image is unique. Will will prove this as a lemma.

Lemma: A inverse image of a set $U$ under $f$ is unique.
	Suppose for a set $U$ we had another inverse under $f$, so we would have $S$ and $S'$. According to the definition we have that $f^{-1}(U)=\{x\in X:f(x)\in U\}$
	But then every $s$ in $S$ is also in $s'$ by definition and vise versa. Thus the inverse image is unique.

This is thus a valid property, meaning that the set $\left\{ Y:P(f,Y)\land f\in \{0,1\}^X\right\}$ is indeed a valid set according to the power set axiom and the axiom of replacement.

We now have to prove the equality between those two sets. To make the proof easier to write we denote $\left\{ Y:P(f,Y)\land f\in \{0,1\}^X\right\}=\mathcal{R}$ and $\left\{ Y:Y\subseteq X\right\}=\mathcal{P}$. First we proof equality from $\mathcal{R}$ to $\mathcal{P}$.

Suppose we have $Z\in \mathcal{R}$ , then $f^{-1}(\{1\})=Z$ and according to the definition of the inverse image, this implies that every $z\in Z$ is also in the domain of $f$, namely $x$. And thus $Z\subseteq X$ which gives us $Z\in\mathcal{P}$.

Now we prove it but starting from $\mathcal{P}$. Suppose we have $Z \in \mathcal{P}$ then we know that $Z \subseteq X$. This means that for all $f\in \{0,1\}^X$ $f(z)$ is well defined for all $z\in Z$. Now suppose we have the following function $g:X\rightarrow \{0,1\}:\alpha\mapsto \left\{ \begin{align} 1 \hspace{1cm}:\alpha\in Z \\ 0 \hspace{1cm}:\alpha\notin Z      \end{align}\right.$ ,which we notice is indeed in $\{0,1\}^X$. Then we know that according to the definition of $g$ we have that $g^{-1}(\{1\})=Z$ but this means that the $P(g,Z)$ is true and thus $Z$ is indeed in $\mathcal{R}$.

Since $(\forall p \in \mathcal{P}:p \in \mathcal{R})\land(\forall r \in \mathcal{R}:r \in \mathcal{P})$ we have that $\mathcal{P}=\mathcal{R}$ or $\left\{ Y:Y\subseteq X\right\}=\left\{ Y:P(f,Y)\land f\in \{0,1\}^X\right\}$.

**Q.E.D.** 


## *Constructing Terence Tao's axiom using the power set axiom*

We will now assume the first axiom and prove that we can build the following set:
$$\forall X:\forall Y: \exists Y^X:f\in Y^X \iff f  \;\text{is a function} \;X\rightarrow Y$$
Suppose we have two arbitrary sets $X$ and $Y$, then we know their cartesian product is well defined. We also know that the power set of their cartesian product is well defined.
$$\mathcal{P}(X\times Y)=\{A:A\subseteq X\times Y\}$$
We then use the axiom of specification with the property $P$ that states:
$$P(A):\forall x\in X:\exists!y\in Y: (x,y)\in A$$
And thus we can construct the following set:
$$G_\mathcal{P}=\{A\in \mathcal{P}(X\times Y):P(A)\}$$
This gives us a set with all the possible sets that pass the vertical line test and are a subset of $X\times Y$. Since we know every graph has a unique functions associated to it, see: [[Graph (functions)]], we can use the axiom of replacement to replace every graph in $G_\mathcal{P}$ by it's unique functions.
$$Y^X=\{f:P(G,f)\land G\in G_\mathcal{P}\}$$
Where the property $P$ states $f$ is a function from $X\rightarrow Y$ such that $G$ is the graph of $f$. One can easily check this set is exactly the same as the one built by the axiom of Terence Tao.

**Q.E.D.**


#completed 