
Union, intersection and difference are 3 operations over [[Sets|sets]] that form a [[Boolean algebra|Boolean algebra]]. 

## *Pairwise union*

Pairwise union is axiomatically defined in [[Sets|set]] theory as such:

Given any two sets $A$, $B$, there exists a set $A ∪ B$, called the union $A ∪ B$ of $A$ and $B$, whose elements consists of all the elements which belong to $A$ or $B$ or both. In other words, for any object $x$, $x \in A ∪ B \iff (x ∈ A \lor x \in B)$.

![[union-of-sets-using-venn-diagram.png|250]]


#### *Lemma's and properties*
- If $A$, $B$, $A'$ are sets, and $A$ is equal to $A'$ , then $A ∪ B$ is equal to $A' ∪ B$       $$A=A' \iff A\cup B=A' \cup B \hspace{1cm}(1)$$ 
- If $a$ and $b$ are objects, then $\{a, b\} = \{a\}∪\{b\}$, (more about singletons in this note [[Sets]]). $$\{a, b\} = \{a\}∪\{b\} \hspace{1cm} (2)$$

##### Proofs

- (1)
	First we assert that since $A=A'\iff (\forall a \in A:a \in A')\land(\forall a' \in A':a' \in A)$ . We also know that the union of $A$ and $B$ is defined as follows: $x \in A ∪ B \iff (x ∈ A \lor x \in B)$. But notice that if $x$ turns out to be in $A$ then it must be in $A'$ to by the definition of set equality. This implies that $(x\in A \land x\in A')\lor x\in B$ which also implies that $x\in A' \lor x \in B$ , but this is just the definition of $A'\cup B$ which was derived out of $A \cup B$'s definition. This thus means that $A\cup B=A'\cup B$. We in theory also need to prove that $A\cup B=A' \cup B\implies A=A'$ . For this we just imagine a  $y$ in any of the union sets, suppose the $y$ is not $B$, then it must be from $A$ or $A'$ . But if $A \neq A'$ then we would lose set equality between the unions as $y$ could be an element that is only in 1 of the sets.
	
	**Q.E.D.** 
	The same argument can be used to proof that $A\cup B=A\cup B' \iff B=B'$ 
- (2)
	Suppose that $x$ is an element of $\{a,b\}$. Then by Axiom we see that $x=a$ or $x=b$. If $x=a$ then $x$ is in $\{a\}$. Thus by Axiom we see that $x \in \{a\}\cup\{b\}$On the other hand if $x=b$ then $x \in \{b\}$ and $x \in \{a\}\cup\{b\}$. Now suppose $x$ is an element of $x \in \{a\}\cup\{b\}$. Then $x=a$ or $x=b$. If $x\in \{a\}$ then $x=a$ so $x\in \{a,b\}$. And if $x\in \{b\}$ then $x=b$ so again $x\in \{a,b\}$.
	
	**Q.E.D.**


#### *Algebra*

- Union is commutative: $$A∪B = B ∪ A \hspace{1cm}(1)$$
- Union is associative: $$(A ∪ B)∪ C = A ∪(B ∪ C)\hspace{1cm}(2)$$


##### Proofs

- (1)
	For any arbitrary $x$ in $A \cup B$ $x$ is either in $A$,$B$ or both by definition. But for each of these cases, $x$ will also be in $B \cup A$. And thus we have equality of sets and $A\cup B= B\cup A$.
	
	**Q.E.D.**
- (2)
	By the definition of set equality, we need to show that every element $x$ of $(A ∪ B) ∪ C$ is an element of $A ∪ (B ∪ C)$, and vice versa. So suppose first that $x$ is an element of $(A∪B)∪C$. By Axiom of pairwise union, this means that at least one of $x ∈ A∪B$ or $x ∈ C$ is true. We now divide into two cases. If $x ∈ C$, then by Axiom of pairwise union again $x ∈ B ∪ C$, and so by Axiom of pairwise union again we have $x ∈ A ∪ (B ∪ C)$. Now suppose instead $x ∈ A ∪ B$, then by Axiom of pairwise union again $x ∈ A$ or $x ∈ B$. If $x ∈ A$ then $x ∈ A ∪ (B ∪ C)$ by Axiom of pairwise union, while if $x ∈ B$ then by consecutive applications of Axiom of pairwise union we have $x ∈ B ∪ C$ and hence $x ∈ A ∪ (B ∪ C)$. Thus in all cases we see that every element of $(A ∪ B) ∪ C$ lies in $A ∪ (B ∪ C)$. A similar argument shows that every element of $A∪(B∪C)$ lies in $(A∪B)∪C$, and so $(A∪B)∪C = A∪(B∪C)$ as desired.
	
	**Q.E.D.**





## *Union or arbitrary union*

Union is an operation axiomatically defined with the axiom of union.

Given any set $A$ consisting of only sets there is a set $B$ such that, for any element $c$, $c$ is a member of $B$ if and only if there is a set $D$ such that $c$ is a member of $D$ and $D$ is a member of $A$.
$$x\in\bigcup A\iff \exists S(x\in S \land S \in A) $$
A consequence of this axiom and the axiom of replacement is the following definition.
$$\bigcup_{\alpha\in I} A_{\alpha}:=\bigcup\{A_\alpha:\alpha\in I\}$$
Here we usually refer to $I$ as the index set and $\alpha$ as the labels. The set $A_\alpha$ is then called the family of sets and is indexed by the labels $\alpha \in I$. We can define intersection in the same fashion
## *Intersection*

The intersection of two sets $S_1$ and $S_2$ is defined as: $$S_1 \cap S_2=\{ x \in S_1 :x\in S_2\}$$
Two sets are said to be disjoint if: $$A\cap B= \emptyset$$
![[intersection-of-sets-using-Venn-diagram.png|250]]

We can also define arbitrary intersection thanks to the axiom of specification, in the same fashion than union. We first choose a arbitrary $\beta$ in $I$ (choice of beta doesn't matter).
$$\bigcap_{\alpha\in I}A_\alpha:=\{x\in A_\beta:x\in A_\alpha \;\text{for all} \;\alpha \in I\}$$
And from that follows:
$$y \in \bigcap_{α∈I} A_α \iff (y ∈ A_α \;\text{for all}\; α ∈ I)$$

Why doesn't the choice of $\beta$ matter ? Since we are building a set with elements that are present in each $A$ set the choice of $\beta$ doesn't matter. If $x$ is in $\bigcap_{\alpha\in I}A_\alpha$ then we know it is in any $A_\alpha$ meaning the actual choice of $\beta$ does not matter. One could say it does matter for elements that are not in every $A$ set, but the point is that we are voluntarily trying to filter those out.


## *Difference*

Given any two sets we define their difference as: $$A\backslash B=\{  x\in A:x\notin B \}$$
![[difference-of-sets-using-Venn-diagram.png|250]]


## Boolean algebra of sets

Let $A$,$B$,$C$ be sets and let $X$ be a set who's subsets are $A$,$B$ and $C$.

- [[Bounds, strict bounds, minimal and maximal elements of a set|Minimal element]]: we have $A ∪ ∅ = A$ and $A ∩ ∅ = ∅$. 
- [[Bounds, strict bounds, minimal and maximal elements of a set|Maximal element]]: we have $A ∪ X$ = $X$ and $A ∩ X$ = $A$. 
- Identity: we have $A ∩ A = A$ and $A ∪ A = A$. 
- Commutativity: we have $A ∪ B = B ∪ A$and $A ∩ B = B ∩ A$. 
- Associativity: we have $(A∪B)∪C = A∪(B∪C)$ and $(A∩B)∩C = A ∩ (B ∩ C)$. 
- Distributivity: we have $A ∩ (B ∪ C)=(A ∩ B) ∪ (A ∩ C)$ and $A ∪ (B ∩ C)=(A ∪ B) ∩ (A ∪ C)$. 
- Partition: we have $A ∪ (X\backslash A) = X$ and $A ∩ (X\backslash A) = ∅$.  
- De Morgan laws: we have $X\backslash(A ∪ B)=(X\backslash A) ∩ (X\backslash B)$ and $X\backslash (A ∩ B)=(X\backslash A) ∪ (X\backslash B)$.

All this laws are know as the laws of Boolean algebra


#### *Proof*

It's lengthy and boring to prove all of them, but basically we always try to apply the definition of set equality by stating that any arbitrary element of a set, regardless of its origin, is also an element of the other set. This basic technique can be used for literally every property.


## *Subsets through union and intersection*

The remarkable logic equivalence is the following: $$A\cup B=B \iff A\subseteq B$$$$A\cap B =A \iff A \subseteq B$$
#### *Proof*

Straight forward, just use the basic definitions of set equality, subsets and union/intersection and the implication will reveal itself easily.




#completed 