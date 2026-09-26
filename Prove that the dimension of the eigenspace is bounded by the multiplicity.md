---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: Let $T$ be a linear operator on a finite-dimensional vector space. For any eigenvalue $\lambda$ with algebraic multiplicity $m$, $\dim(E_\lambda) \le m$.
#### Notes
- Let $p = \dim(E_\lambda)$. Choose a basis for $E_\lambda$ and extend it to a complete ordered basis $\beta$ for $V$.
- Form the block upper triangular matrix representation $A = [T]_\beta$ where the top-left block is $\lambda I_p$.
- Compute the characteristic polynomial $f(t) = \det(A - tI_n) = \det((\lambda - t)I_p) \cdot \det(C - tI_{n-p}) = (\lambda - t)^p g(t)$.
- Since $(\lambda - t)^p$ strictly divides the characteristic polynomial, the algebraic multiplicity $m$ must be at least $p$
