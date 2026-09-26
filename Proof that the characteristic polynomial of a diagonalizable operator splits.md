---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: The characteristic polynomial of any diagonalizable linear operator on a vector space $V$ over a field $F$ splits over $F$.
#### Notes
- Choose an ordered basis $\beta$ such that the matrix representation is a diagonal matrix $D = \text{diag}(\lambda_1, \dots, \lambda_n)$.
- Construct the characteristic polynomial as $f(t) = \det(D - tI_n)$.
- Evaluate the determinant of the resulting diagonal matrix to obtain $f(t) = (\lambda_1 - t)\cdots(\lambda_n - t)$.
- Factor out $(-1)^n$ to yield $f(t) = (-1)^n (t - \lambda_1)\cdots(t - \lambda_n)$, demonstrating that the polynomial splits.
