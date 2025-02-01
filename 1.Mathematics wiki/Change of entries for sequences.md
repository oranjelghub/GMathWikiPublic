
---

mathLink: auto

---
Date created: 2023-12-20 13:09
Tags: #Type/Notion #Topic/Real_Analysis 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Limsup and liminf of sequences (Properties)]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Limit points of a sequence]], [[Limsup and liminf of sequences]]

---  

This note describe how notions such as [[Limsup and liminf of sequences]] and [[Limit points of a sequence]] behave when we change some of the entries in different manners in a sequence.

> [!quote] Notion: $(a_n)^\infty_{n=m}\to (a_n)^\infty_{n=m'}$ with $m'\geq m$
> 1. $c$ is a limit point of $(a_n)^\infty_{n=m}$ $\iff$ $c$ is a limit point of $(a_n)^\infty_{n=m'}$
> 2. $\limsup_{n\to \infty}a_{n}=c$ with $(a_n)^\infty_{n=m}$ $\iff$ $\limsup_{n\to \infty}a_{n}=c$ with $(a_n)^\infty_{n=m'}$
> 3. $\liminf_{n\to \infty}a_{n}=c$ with $(a_n)^\infty_{n=m}$ $\iff$ $\liminf_{n\to \infty}a_{n}=c$ with $(a_n)^\infty_{n=m'}$


> [!quote] Notion: $(a_n)^\infty_{n=m}\to (a_{n+k})^\infty_{n=m}$ with $k\in \mathbb Z$
> 1. $c$ is a limit point of $(a_n)^\infty_{n=m}$ $\iff$ $c$ is a limit point of $(a_{n+k})^\infty_{n=m}$
> 2. $\limsup_{n\to \infty}a_{n}=c$ with $(a_n)^\infty_{n=m}$ $\iff$ $\limsup_{n\to \infty}a_{n+k}=c$ with $(a_n+k)^\infty_{n=m}$
> 3. $\liminf_{n\to \infty}a_{n}=c$ with $(a_n)^\infty_{n=m}$ $\iff$ $\liminf_{n\to \infty}a_{n+k}=c$ with $(a_n+k)^\infty_{n=m}$

We won't elaborate on the proofs as most of them are straight forward.