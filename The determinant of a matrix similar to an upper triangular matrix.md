---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: If an $n \times n$ matrix $A$ is similar to an upper triangular matrix with distinct eigenvalues $\lambda_1, \dots, \lambda_k$ and corresponding multiplicities $m_1, \dots, m_k$, then $\det(A) = (\lambda_1)^{m_1} (\lambda_2)^{m_2} \cdots (\lambda_k)^{m_k}$
#### Notes
- Since $A$ is similar to an upper triangular matrix $U$, there exists an invertible matrix $Q$ such that $A = Q U Q^{-1}$.
    
- The diagonal entries of $U$ are the eigenvalues $\lambda_i$, each appearing with algebraic multiplicity $m_i$.
    
- Apply the multiplicative property of determinants to show similarity preserves the determinant: $\det(A) = \det(Q)\det(U)\det(Q^{-1}) = \det(Q)\det(U)\det(Q)^{-1} = \det(U)$.
    
- Conclude that $\det(A)$ is the product of the diagonal entries of the upper triangular matrix $U$, yielding the product $\prod_{i=1}^k (\lambda_i)^{m_i}$.
