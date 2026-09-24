---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 3.2 The Rank of a Matrix and Matrix Inverses]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch3
date_created: 2026-09-23
---
Prove that every matrix has a rank normal form. Let $A$ be an $m \times n$ matrix of rank $r$. By a finite number of elementary row and column operations, $A$ can be transformed into $D = \begin{pmatrix} I_r & O_1 \\ O_2 & O_3 \end{pmatrix}$.
#### Notes
- Handle base cases: $A = O$ is trivial; for $m = 1$, shift a non-zero element to $(1,1)$, scale to 1, and clear the row.
    
- Assume $m > 1$ and proceed by induction on $m$.
    
- Shift a nonzero entry to $(1,1)$, scale to 1, and use type 3 operations to clear the remainder of the first row and column.
    
- Apply the inductive hypothesis to the residual $(m-1) \times (n-1)$ submatrix of rank $r-1$ to achieve the final block form $D$.
