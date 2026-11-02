---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $T$ and $U$ are linear operators on an inner product space $V$ whose adjoints exist, then $(T + U)^* = T^* + U^*$.
#### Notes
For all $x, y \in V$, $\langle (T + U)(x), y \rangle = \langle T(x), y \rangle + \langle U(x), y \rangle = \langle x, T^*(y) \rangle + \langle x, U^*(y) \rangle = \langle x, (T^* + U^*)(y) \rangle$. By uniqueness of the adjoint, $(T + U)^* = T^* + U^*$.
