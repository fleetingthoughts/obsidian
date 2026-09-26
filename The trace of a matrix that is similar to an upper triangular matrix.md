---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: If an $n \times n$ matrix $A$ is similar to an upper triangular matrix with distinct eigenvalues $\lambda_1, \dots, \lambda_k$ and corresponding multiplicities $m_1, \dots, m_k$, then $\text{tr}(A) = \sum_{i=1}^k m_i \lambda_i$
#### Notes
- Since $A$ is similar to an upper triangular matrix $U$, there exists an invertible matrix $Q$ such that $A = Q U Q^{-1}$.
- The diagonal entries of the upper triangular representation $U$ are exactly the eigenvalues of $A$, with each $\lambda_i$ occurring exactly $m_i$ times.
- Utilize the cyclic property of the trace to demonstrate that similarity preserves the trace: $\text{tr}(A) = \text{tr}(Q U Q^{-1}) = \text{tr}(U Q^{-1} Q) = \text{tr}(U)$.
- Conclude that $\text{tr}(A)$ is the sum of the diagonal entries of $U$, which yields the sum $\sum_{i=1}^k m_i \lambda_i$.
