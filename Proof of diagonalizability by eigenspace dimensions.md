---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: Let $T$ be a linear operator on an $n$-dimensional vector space such that its characteristic polynomial splits. $T$ is diagonalizable if and only if the multiplicity of each eigenvalue equals the dimension of its eigenspace.
#### Notes
- Forward direction: Diagonalizability forces the sum of all eigenspace dimensions to equal $n$. Since $\dim(E_{\lambda_i}) \le m_i$ and $\sum m_i = n$, this forces $\dim(E_{\lambda_i}) = m_i$ for all $i$.
- Reverse direction: Assume $\dim(E_{\lambda_i}) = m_i$ for all $i$. Select a basis for each eigenspace and take their total union $\beta$.
- Invoke the theorem on eigenvector independence to establish that $\beta$ is a linearly independent set.
- Because $\sum \dim(E_{\lambda_i}) = \sum m_i = n$, the set $\beta$ contains $n$ vectors, forming an eigenvector basis for $V$.
