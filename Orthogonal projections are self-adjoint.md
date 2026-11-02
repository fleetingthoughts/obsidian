---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $V$ is an inner product space with $V = W \oplus W^\perp$ and $T: V \to V$ is the orthogonal projection onto $W$ along $W^\perp$, then $T^* = T$.
#### Notes
- Given arbitrary $x, y \in V$, decompose $x = x_1 + x_2$ and $y = y_1 + y_2$ with $x_1, y_1 \in W$ and $x_2, y_2 \in W^\perp$, so $T(x) = x_1$ and $T(y) = y_1$.
- Compute $\langle T(x), y \rangle$ using $\langle x_1, y_2 \rangle = 0$:
    $$\begin{aligned} \langle T(x), y \rangle &= \langle x_1, y_1 + y_2 \rangle \\ &= \langle x_1, y_1 \rangle + \langle x_1, y_2 \rangle \\ &= \langle x_1, y_1 \rangle \end{aligned}$$
- Compute $\langle x, T(y) \rangle$ using $\langle x_2, y_1 \rangle = 0$:
    $$\begin{aligned} \langle x, T(y) \rangle &= \langle x_1 + x_2, y_1 \rangle \\ &= \langle x_1, y_1 \rangle + \langle x_2, y_1 \rangle \\ &= \langle x_1, y_1 \rangle \end{aligned}$$
- Conclude $\langle T(x), y \rangle = \langle x, T(y) \rangle$ for all $x, y \in V$, so $T^* = T$ by uniqueness of the adjoint.
