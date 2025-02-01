---
mathLink: auto
Date created: 2024-05-17 16:30
tags:
  - Type/Object
  - Topic/Real_Analysis
cssclasses:
---

---

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Continuous version of squeeze test]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: [[Sequential definition of limsup and liminf of functions at a point]]
Justifications: [[Existence of least upper bounds]], [[Uniqueness of least upper bounds]], [[Limit of a real valued function at a point]], [[Supremum and infimum of sequences]]

---

> [!quote] Definition: Limsup and liminf of functions at a point
> Given some function $f:X\to \mathbb{R}$, $E\subseteq \mathbb{R}$ and some $x_{0}\in \overline E$, we define $$ \begin{align} F^+_{N}&:= \sup\left( f\left( \left[ x_{0}- \frac{1}{N}, x_{0}+ \frac{1}{N} \right]\cap E \right) \right) \\ F^-_{N}&:= \inf\left( f\left( \left[ x_{0}- \frac{1}{N}, x_{0}+ \frac{1}{N} \right]\cap E \right) \right) \end{align} $$ And define also $$ \begin{align} \limsup_{ x_{0} \to x: x\in E }f(x)&:=  \inf(F^+_{N})^\infty_{N=1} \\ \liminf_{ x_{0} \to x: x\in E }f(x)&:=  \sup(F^-_{N})^\infty_{N=1}\end{align} $$

Equivalently, using the monotonicity of $(F^+_{N})^\infty_{N=1}$ and $(F^-_{N})^\infty_{N=1}$ it can be shown that equivalently $$ \begin{align}\lim_{ N \to \infty } F^+_{N}&=\limsup_{ x \to x_{0} : x\in E }f(x)\\ \lim_{ N \to \infty } F^-_{N}&= \liminf_{ x \to x_0:x\in E } f(x)  \end{align} $$
If and only if $\limsup_{ x \to x_{0} : x\in E }f(x)$ and $\liminf_{ x \to x_0:x\in E } f(x)$ are finite obviously.
