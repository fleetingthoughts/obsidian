---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.4 Invariant Subspaces and the Cayley-Hamilton Theorem]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-10-04
---
Prove: Let $T$ be a linear operator on a finite-dimensional vector space $V$, and let $W$ be a $T$-invariant subspace of $V$. Then the characteristic polynomial of $T_W$ divides the characteristic polynomial of $T$.
#### Notes
- Select an ordered basis $\gamma$ for $W$ and extend it to an ordered basis $\beta$ for $V$.
- Because $W$ is $T$-invariant, represent $T$ with a block upper-triangular matrix $A = \begin{pmatrix} B_1 & B_2 \\ O & B_3 \end{pmatrix}$, where $B_1 = [T_W]_\gamma$.
- Compute the characteristic polynomial $f(t) = \det(A - tI_n) = \det(B_1 - tI_k) \cdot \det(B_3 - tI_{n-k})$.
- Identify $g(t) = \det(B_1 - tI_k)$ as the characteristic polynomial of $T_W$, proving $g(t)$ divides $f(t)$.
