---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: If an invertible linear operator $T$ on a finite-dimensional vector space is diagonalizable, then $T^{-1}$ is diagonalizable.
#### Notes
- Since $T$ is diagonalizable, there exists a basis $\beta$ consisting entirely of eigenvectors of $T$.
    
- For any $v \in \beta$ with corresponding eigenvalue $\lambda$, $T(v) = \lambda v$. Invertibility guarantees $\lambda \neq 0$.
    
- Applying $T^{-1}$ to both sides and dividing by $\lambda$ yields $T^{-1}(v) = \lambda^{-1} v$.
    
- Thus, every vector in $\beta$ is also an eigenvector of $T^{-1}$, meaning $T^{-1}$ has a basis of eigenvectors and is diagonalizable.
