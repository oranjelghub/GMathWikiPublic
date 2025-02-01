#### ordering
Okay so turns out we can equip ourselves with a totally different yet synonymous set of [[Peano axioms]] . These actually assume that the trichotomy presented in [[Ordering (binary relation)]] is axiomatic, it is most certainly different and very confusing when doing research so stay careful. Also this might work differently when talking about the real numbers so please consult this page again later.

In this notes we will be considering Terence Tao's Peano axioms and we will not bother treating other approaches to defining basics for the sake of my sanity. Maybe thru time there will come more alternatives to it but in the mean time it is what it is.

#### different math fonts


$$
\begin{align*}
\mathcal{RQSZ} \\
\mathfrak{RQSZ} \\
\mathbb{RQSZ}\\
\mathscr{RQSZ}
\end{align*}$$



#### induction

Extra info about strong [[Induction]] : https://math.stackexchange.com/questions/335479/is-strong-induction-not-actually-stronger-than-normal-induction



#### why do we "prove" axioms

This little section from a post from math stack exchange perfectly sums it up:

**Version 1**

You: Sets $A$ and $B$ are **shmequal** provided $x∈A⇔x∈B$ for all $x$.

Me: That sounds like a fine relation to investigate. Creative name, by the way.

**Version 2**

You: Sets $A$ and $B$ are **equal** provided $x∈A⇔x∈B$ for all $x$.

Me: Now, hold on just a second. By "equal", you mean "identical" or "exactly the same"? I'm not sure I'm ready to accept that this abstract definition captures all that. You would need to show me that the relation $x∈A⇔x∈B$ for all $x$ is reflexive, symmetric, and transitive before I'm willing to concede that this deserves a name like "equal".

In other words, in order for our relationship to capture classical equality its needs to follow the axioms we originally imposed on classical equality. Otherwise this relationship may need another name, as it may still define an equality, but not the classical one.

#### ring confusion

The operations ++ and ⋅⋅ can be _any_ binary operations on the set R�, as long as they satisfy all the ring axioms. They don't have to be the operations we normally call "addition" and "multiplication" on R�, if such operations exist. However, in the context of the ring (R,+,⋅)(�,+,⋅), we usually refer to ++ as "addition" and ⋅⋅ as "multiplication". So when we speak of "associativity of multiplication", for instance, we are actually talking about associativity of the operation ⋅⋅, whatever it happens to be.