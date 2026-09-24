---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 3.2 The Rank of a Matrix and Matrix Inverses]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch3
date_created: 2026-09-23
---
Prove for any $m \times n$ matrix $A$, $\text{rank}(A^t) = \text{rank}(A)$.
#### Notes
By the canonical form theorem, there exist invertible matrices $P$ and $Q$ such that $PAQ = D$, where $D$ is a block matrix with $I_r$ in the top-left corner and rank $r = \text{rank}(A)$. Taking transposes yields $Q^t A^t P^t = D^t$. Since $P^t$ and $Q^t$ are invertible and $D^t$ has the same rank $r$ as $D$, invertible multiplication rank invariance gives $\text{rank}(A^t) = \text{rank}(D^t) = r = \text{rank}(A)$.
