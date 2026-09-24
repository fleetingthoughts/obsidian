---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 3.2 The Rank of a Matrix and Matrix Inverses]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch3
date_created: 2026-09-23
---
Prove every invertible matrix is a product of elementary matrices.
#### Notes
If $A$ is an $n \times n$ invertible matrix, $\text{rank}(A) = n$. By the canonical form theorem, $A$ can be transformed into $I_n$ via elementary operations. This implies there exist elementary matrices $E_1, \dots, E_k$ such that $E_k \dots E_1 A = I_n$. Inverting these elementary matrices (which yields other elementary matrices) provides $A = E_1^{-1} \dots E_k^{-1}$.
