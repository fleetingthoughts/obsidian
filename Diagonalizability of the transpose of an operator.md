---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: If a square matrix $A$ is diagonalizable, then its transpose $A^t$ is diagonalizable.
#### Notes
- Since $A$ is diagonalizable, there exists an invertible matrix $Q$ and a diagonal matrix $D$ such that $A = Q D Q^{-1}$.
    
- Take the transpose of both sides to obtain $A^t = (Q D Q^{-1})^t = (Q^{-1})^t D^t Q^t$.
    
- Apply standard transpose properties: the transpose of a diagonal matrix is itself ($D^t = D$), and $(Q^{-1})^t = (Q^t)^{-1}$.
    
- Substitute these to yield $A^t = (Q^t)^{-1} D Q^t$, establishing that $A^t$ is similar to a diagonal matrix.
