---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 3.2 The Rank of a Matrix and Matrix Inverses]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch3
date_created: 2026-09-23
---
Prove if $A$ be an $m \times n$ matrix with rank $m$ and $B$ be an $n \times p$ matrix with rank $n$. The rank of $AB$ equals $m$
#### Notes
$\text{rank}(A) = m$ implies $L_A$ is surjective, and $\text{rank}(B) = n$ implies $L_B$ is surjective. The composition of surjective linear transformations $L_A \circ L_B = L_{AB}$ is also surjective. Therefore, the dimension of the range of $L_{AB}$ is $m$, yielding $\text{rank}(AB) = m$.
