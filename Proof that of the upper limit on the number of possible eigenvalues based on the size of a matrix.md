---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.1 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-19
---
Prove that the characteristic polynomial of an $n \times n$ matrix has a degree of $n$ and that the matrix has at most $n$ distinct eigenvalues?
#### Notes
- Proceed by induction on $n$.
- Expand $\det(A - tI_n)$ along the first row. The main diagonal product term $(A_{11} - t)\det(A_{11}' - tI_{n-1})$ strictly yields $(-1)^n t^n$.
- Demonstrate all other cofactor expansion terms have a degree of at most $n-2$.
- Apply the algebraic property that a degree $n$ polynomial possesses at most $n$ distinct zeros, upper-bounding the eigenvalue count.
