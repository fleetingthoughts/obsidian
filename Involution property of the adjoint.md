---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $T$ is a linear operator on an inner product space $V$ whose adjoint exists, then $T^{} = T$.
#### Notes
For all $x, y \in V$, $\langle T^*(x), y \rangle = \overline{\langle y, T^*(x) \rangle} = \overline{\langle T(y), x \rangle} = \langle x, T(y) \rangle$. By uniqueness of the adjoint of $T^*$, $(T^*)^* = T$.
