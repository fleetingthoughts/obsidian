---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.2 The Matrix Representation of A Linear Transformation]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch2
date_created: 2026-07-24
---
Let $V$ be an $n$-dimensional vector space, and let $T: V \rightarrow V$ be a linear transformation. If $W$ is a $T$-invariant subspace of $V$ having dimension $k$, there exists a specific ordered basis $\beta$ for $V$ that forces a distinct, partitioned structural geometry onto the matrix representation. `::` There is a basis $\beta$ such that $[T]_\beta$ has the block upper triangular form $\begin{pmatrix} A & B \\ O & C \end{pmatrix}$, where $A$ is a $k \times k$ matrix and $O$ is the $(n-k) \times k$ zero matrix.
#### Notes
Let $\beta = \{v_1, v_2, \dots, v_n\}$ be a basis for a vector space $V$, and let $T: V \rightarrow V$ be a linear transformation. The matrix representation $[T]_\beta$ is strictly upper triangular if and only if a specific, nested sequential span condition is met by the transformation's mapping. `::` The matrix $[T]_\beta$ is upper triangular if and only if the image of each basis vector remains confined to the span of its predecessors, formally stated as $T(v_j) \in \text{span}(\{v_1, v_2, \dots, v_j\})$ for all $j = 1, 2, \dots, n$.
