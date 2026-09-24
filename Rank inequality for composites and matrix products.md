---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 3.2 The Rank of a Matrix and Matrix Inverses]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch3
date_created: 2026-09-23
---
Prove the following: Let $T: V \to W$ and $U: W \to Z$ be linear transformations on finite-dimensional vector spaces, and $A, B$ be matrices such that $AB$ is defined. Then $\text{rank}(UT) \le \text{rank}(U)$, $\text{rank}(UT) \le \text{rank}(T)$, $\text{rank}(AB) \le \text{rank}(A)$, and $\text{rank}(AB) \le \text{rank}(B)$
#### Notes
- Bound by $U$: Observe $R(UT) = U(R(T)) \subseteq R(U)$. Taking dimensions yields $\text{rank}(UT) \le \text{rank}(U)$.
- Bound by $T$: Select ordered bases to represent $U$ and $T$ as matrices $A'$ and $B'$. Apply transpose rank equality to obtain $\text{rank}(A'B') = \text{rank}((A'B')^t) = \text{rank}((B')^t (A')^t) \le \text{rank}((B')^t) = \text{rank}(B')$, concluding $\text{rank}(UT) \le \text{rank}(T)$.
- Apply (1) to left-multiplication operators for $\text{rank}(AB) \le \text{rank}(A)$.
- Apply (2) to left-multiplication operators for $\text{rank}(AB) \le \text{rank}(B)$.
