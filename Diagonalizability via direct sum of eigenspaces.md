---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: A linear operator $T$ on a finite-dimensional vector space $V$ is diagonalizable if and only if $V$ is the direct sum of the eigenspaces of $T$.
#### Notes
- Forward direction ($\Rightarrow$): Assume $T$ is diagonalizable, which yields a basis $\beta$ for $V$ consisting of eigenvectors.
    
- Partition $\beta$ into subsets corresponding to each distinct eigenvalue $\lambda_i$. This partition spans $V$, meaning $V = \sum_{i=1}^k E_{\lambda_i}$.
    
- By the linear independence of eigenvectors from distinct eigenvalues, intersections between these eigenspace sums are trivial, establishing the direct sum $V = \bigoplus_{i=1}^k E_{\lambda_i}$.
    
- Reverse direction ($\Leftarrow$): Assume $V = \bigoplus_{i=1}^k E_{\lambda_i}$ and select an ordered basis $\beta_i$ for each eigenspace.
    
- The direct sum property guarantees that the union $\bigcup_{i=1}^k \beta_i$ constitutes a basis for $V$. Because this basis consists entirely of eigenvectors, $T$ is diagonalizable.
