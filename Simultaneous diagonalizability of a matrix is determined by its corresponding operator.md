---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: If $T$ and $U$ are simultaneously diagonalizable linear operators on a finite-dimensional vector space $V$, then the matrices $[T]_\beta$ and $[U]_\beta$ are simultaneously diagonalizable for any ordered basis $\beta$.
#### Notes
- By definition, there exists an ordered basis $\gamma$ such that $[T]_\gamma$ and $[U]_\gamma$ are diagonal matrices.
- Let $\beta$ be any ordered basis for $V$, and let $Q$ be the change of coordinate matrix from $\gamma$ to $\beta$.
- The representations are related by similarity: $[T]_\gamma = Q^{-1}[T]_\beta Q$ and $[U]_\gamma = Q^{-1}[U]_\beta Q$.
- Since $[T]_\gamma$ and $[U]_\gamma$ are diagonal, $[T]_\beta$ and $[U]_\beta$ are simultaneously diagonalizable via the invertible matrix $Q$.
