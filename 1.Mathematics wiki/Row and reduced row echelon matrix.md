---
mathLink: auto
Date created: 2024-09-01 12:57
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: [[Every matrix is row equivalent to some row reduced echelon form matrix]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Matrices]]

---

> [!quote] Definition: Row echelon form
> A matrix $A\in M_{n\times n}(F)$ is said to be in row echelon form if and only if:
> 1. The first non-zero element of each row is $1$
> 2. The first non-zero element of a row that's lower than some other given row is at least one column further
> 3. The rows of only zeroes are all at the bottom

Furthermore we say that the matrix is in reduced row echelon form if it satisfies the above conditions and all the elements after the first $1$ of each row are equal to $0$.
