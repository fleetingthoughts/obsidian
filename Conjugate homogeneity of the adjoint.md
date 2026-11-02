---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $T$ is a linear operator on an inner product space $V$ whose adjoint exists and $c \in F$, then $(cT)^* = \overline{c}T^*$.
#### Notes
For all $x, y \in V$, $\langle (cT)(x), y \rangle = c\langle T(x), y \rangle = c\langle x, T^*(y) \rangle = \langle x, \overline{c}T^*(y) \rangle$. By uniqueness of the adjoint, $(cT)^* = \overline{c}T^*$.
