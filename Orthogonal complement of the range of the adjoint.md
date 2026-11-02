---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $T$ is a linear operator on an inner product space $V$ whose adjoint exists, then $(R(T^*))^\perp = N(T)$, and if $\dim(V) \lt \infty$, then $R(T^*) = (N(T))^\perp$.
#### Notes
For any $x \in V$:

$$\begin{aligned} x \in (R(T^*))^\perp &\iff \langle x, T^*(y) \rangle = 0 \quad \text{for all } y \in V \\ &\iff \langle T(x), y \rangle = 0 \quad \text{for all } y \in V \\ &\iff T(x) = 0 \iff x \in N(T) \end{aligned}$$

When $\dim(V) \lt \infty$, taking orthogonal complements yields $R(T^*) = ((R(T^*))^\perp)^\perp = (N(T))^\perp$.
