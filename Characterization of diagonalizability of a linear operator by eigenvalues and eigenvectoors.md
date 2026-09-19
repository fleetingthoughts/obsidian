---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.1 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch5
date_created: 2026-09-19
---
State and prove an equivalent condition to the diagonalizability of both a linear operator and a matrix
#### Notes
**Theorem 5.1**: A linear operator $T$ on a finite-dimensional vector space $V$ is diagonalizable if and only if there exists an ordered basis $\beta$ for $V$ consisting of eigenvectors of $T$. Furthermore, if $T$ is diagonalizable, $\beta = \{v_1, v_2, \dots, v_n\}$ is an ordered basis of eigenvectors of $T$, and $D = [T]_\beta$, then $D$ is a diagonal matrix and $D_{jj}$ is the eigenvalue corresponding to $v_j$ for $1 \le j \le n$.

**Corollary to Theorem 5.1**: A matrix $A \in M_{n \times n}(F)$ is diagonalizable if and only if there exists an ordered basis for $F^n$ consisting of eigenvectors of $A$. Furthermore, if $\{v_1, v_2, \dots, v_n\}$ is an ordered basis for $F^n$ consisting of eigenvectors of $A$ and $Q$ is the $n \times n$ matrix whose $j$th column is $v_j$ for $j = 1, 2, \dots, n$, then $D = Q^{-1}AQ$ is a diagonal matrix such that $D_{jj}$ is the eigenvalue corresponding to $v_j$. Hence $A$ is diagonalizable if and only if it is similar to a diagonal matrix.
