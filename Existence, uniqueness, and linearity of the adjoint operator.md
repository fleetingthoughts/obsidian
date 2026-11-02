---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: Let $V$ be a finite-dimensional inner product space and $T$ be a linear operator on $V$. Then there exists a unique function $T^*: V \to V$ such that $\langle T(x), y \rangle = \langle x, T^*(y) \rangle$ for all $x, y \in V$, and $T^*$ is linear.
#### Notes
- Fix $y \in V$ and define $g_y: V \to F$ by $g_y(x) = \langle T(x), y \rangle$; for all $x_1, x_2 \in V$ and $c \in F$, $g_y$ is a linear functional:   $$\begin{aligned} g_y(cx_1 + x_2) &= \langle T(cx_1 + x_2), y \rangle \\ &= c\langle T(x_1), y \rangle + \langle T(x_2), y \rangle \\ &= cg_y(x_1) + g_y(x_2) \end{aligned}$$
- By the Riesz representation theorem, for each $y \in V$ there exists a unique vector $y' \in V$ such that $g_y(x) = \langle x, y' \rangle$ for all $x \in V$; define $T^*: V \to V$ by $T^*(y) = y'$, so $\langle T(x), y \rangle = \langle x, T^*(y) \rangle$.
- To prove $T^*$ is linear, let $y_1, y_2 \in V$ and $c \in F$, and compute for arbitrary $x \in V$:
    $$\begin{aligned} \langle x, T^*(cy_1 + y_2) \rangle &= \langle T(x), cy_1 + y_2 \rangle \\ &= \overline{c}\langle T(x), y_1 \rangle + \langle T(x), y_2 \rangle \\ &= \overline{c}\langle x, T^*(y_1) \rangle + \langle x, T^*(y_2) \rangle \\ &= \langle x, cT^*(y_1) + T^*(y_2) \rangle \end{aligned}$$
- Since $x \in V$ is arbitrary, conclude $T^*(cy_1 + y_2) = cT^*(y_1) + T^*(y_2)$.
- To prove uniqueness, if $U: V \to V$ satisfies $\langle T(x), y \rangle = \langle x, U(y) \rangle$ for all $x, y \in V$, then $\langle x, T^*(y) - U(y) \rangle = 0$ for all $x \in V$, forcing $T^*(y) = U(y)$.
