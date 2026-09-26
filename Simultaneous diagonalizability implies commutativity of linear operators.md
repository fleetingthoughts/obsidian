---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: If $T$ and $U$ are simultaneously diagonalizable operators, then $T$ and $U$ commute (i.e., $TU = UT$).
#### Notes
- Since $T$ and $U$ are simultaneously diagonalizable, there exists an ordered basis $\beta$ such that $[T]_\beta = D_1$ and $[U]_\beta = D_2$ are diagonal matrices.
- Diagonal matrices of the same dimension commute under multiplication, so $D_1 D_2 = D_2 D_1$.
- Compute the matrix representation of the composition: $[TU]_\beta = \([T]_\beta$ $[U]_\beta$ = D_1 D_2).
- Substitute commutativity: $D_1 D_2 = D_2 D_1 = ([U]_\beta$ $[T]_\beta = [UT]_\beta)$
- Because their matrix representations with respect to $\beta$ are identical, the operators themselves are identical, yielding $TU = UT$.
