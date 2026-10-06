---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.4 Invariant Subspaces and the Cayley-Hamilton Theorem]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-10-04
---
Prove: If $V = W_1 \oplus \dots \oplus W_k$ where each $W_i$ is a $T$-invariant subspace with characteristic polynomial $f_i(t)$, then the characteristic polynomial of $T$ is $f_1(t) \cdots f_k(t)$.
#### Notes
- Establish the base case $k = 2$ by concatenating bases for $W_1$ and $W_2$ to form a block-diagonal matrix $[T]_\beta = \begin{pmatrix} B_1 & O \\ O & B_2 \end{pmatrix}$.
- Compute $\det([T]_\beta - tI) = \det(B_1 - tI) \cdot \det(B_2 - tI) = f_1(t) \cdot f_2(t)$.
- Proceed by induction on $k \ge 2$, grouping $W = W_1 \oplus \dots \oplus W_{k-1}$ so that $V = W \oplus W_k$.
- Apply the base case and the inductive hypothesis to factor the characteristic polynomial entirely.
